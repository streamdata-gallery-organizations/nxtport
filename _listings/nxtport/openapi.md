swagger: "2.0"
x-collection-name: NxtPort
x-complete: 1
info:
  title: Portcall+ API (sandbox)
  description: portplus-api
  version: 1.0.0
host: api-sb.nxtport.eu
basePath: /PortCallPlus/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /metrics:
    get:
      summary: Retrieving supported metrics
      description: "The platform allows you to retrieve supported metrics by sending
        a HTTP GET to /metrics. \nThe string-values for the attribute id can be used
        as a metricId path parameter in the City Layer operations. \nThe attribute
        granularity indicates how fine grained temporal pages should be split up when
        querying individual sources (and can be ignored here)."
      operationId: getMetrics
      x-api-path-slug: metrics-get
      responses:
        200:
          description: OK
      tags:
      - MEtrics
  /layers:
    get:
      summary: Retrieve available layers
      description: "This operation lists the currently available city layers. \nThe
        returned strings can then be used as a layerId path parameter in the /layers
        operations included in this API."
      operationId: getLayers
      x-api-path-slug: layers-get
      responses:
        200:
          description: OK
      tags:
      - Layers
  /layers/{layerId}/{metricId}/{date}:
    get:
      summary: Retrieve the city layer data for the specified layer, metric and date.
      description: 'This operation retrieves city layer data for the specified layer,
        metric and date combination. The date is passed in the following format: YYYYMMDD.
        The values for the layerId and metricId can be fetched from the /layers and
        /metrics operations.'
      operationId: getLayerDateByLayerMetricDate
      x-api-path-slug: layerslayeridmetriciddate-get
      parameters:
      - in: path
        name: date
        description: TODO
      - in: path
        name: layerId
        description: TODO
      - in: path
        name: metricId
        description: TODO
      responses:
        200:
          description: OK
      tags:
      - Layers
      - Metrics
  /layers/{layerId}/{metricId}/{date}/{hour}:
    get:
      summary: Retrieve the city layer data for the specified layer, metric and date.
      description: 'This operation retrieves city layer data for the specified layer,
        metric and date combination. The date is passed in the following format: YYYYMMDD.
        The values for the layerId and metricId can be fetched from the /layers and
        /metrics operations.'
      operationId: getLayerDateByLayerMetricDateHour
      x-api-path-slug: layerslayeridmetriciddatehour-get
      parameters:
      - in: path
        name: date
        description: TODO
      - in: path
        name: hour
        description: TODO
      - in: path
        name: layerId
        description: TODO
      - in: path
        name: metricId
        description: TODO
      responses:
        200:
          description: OK
      tags:
      - Layers
  /devices:
    post:
      summary: Publish Device
      description: Publish the fill level for all Big Belly devices.
      operationId: Publish_Devices
      x-api-path-slug: devices-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Devices
  /nxtportdocument/{blnumber}/sn/{stayNumber}:
    get:
      summary: Returns the file with corresponding blnumbers and staynumber.
      description: Returns the file with corresponding blnumbers and staynumber..
      operationId: NxtportdocumentByBlnumberSnByStayNumberGet
      x-api-path-slug: nxtportdocumentblnumbersnstaynumber-get
      parameters:
      - in: path
        name: blnumber
        description: blnumber
      - in: header
        name: Ocp-Apim-Subscription-Key
      - in: path
        name: stayNumber
        description: staynumber
      responses:
        200:
          description: OK
      tags:
      - Returns
      - File
      - Corresponding
      - Blnumbers
      - Staynumber
  /nxtportdocument/{blnumber}/cn/{containerNumber}:
    get:
      summary: Returns the file with corresponding blnumbers and containernumber.
      description: Returns the file with corresponding blnumbers and containernumber..
      operationId: NxtportdocumentByBlnumberCnByContainerNumberGet
      x-api-path-slug: nxtportdocumentblnumbercncontainernumber-get
      parameters:
      - in: path
        name: blnumber
        description: blnumber
      - in: path
        name: containerNumber
        description: containernumber
      - in: header
        name: Ocp-Apim-Subscription-Key
      responses:
        200:
          description: OK
      tags:
      - Returns
      - File
      - Corresponding
      - Blnumbers
      - Containernumber
  /nxtportdocument/{blnumber}/ag/{agent}:
    get:
      summary: Returns the file with corresponding blnumbers and senderID.
      description: Returns the file with corresponding blnumbers and senderid..
      operationId: NxtportdocumentByBlnumberAgByAgentGet
      x-api-path-slug: nxtportdocumentblnumberagagent-get
      parameters:
      - in: path
        name: agent
        description: agent
      - in: path
        name: blnumber
        description: blnumber
      - in: header
        name: Ocp-Apim-Subscription-Key
      responses:
        200:
          description: OK
      tags:
      - Returns
      - File
      - Corresponding
      - Blnumbers
      - SenderID
  /api/v1/releases/:
    post:
      summary: Create release
      description: Serves to create a Container together with its PickupRight that
        gets automatically transferred to the consignee.
      operationId: postApiV1Releases
      x-api-path-slug: apiv1releases-post
      parameters:
      - in: query
        name: api_token
        description: authentication token of user making the request
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Release
  /api/v1/releases/{id}:
    delete:
      summary: Block
      description: |-
        Blocking a release is done by a delete. This will revoke the PickupRight from the consignee. The Container and its PickupRight are deleted. Afterwards it is still possible to release again.
         The following conditions apply for this to work:
        * the container must have been released, i.e. there must be a vallid PickupRight   for the Container
        * the PickupRight should not be transferred to another Organization than the one that got the relesase initially
        * the PickupRight should not yet be assigned (to a driver / skipper)
      operationId: deleteApiV1Releases
      x-api-path-slug: apiv1releasesid-delete
      parameters:
      - in: query
        name: api_token
        description: authentication token of user making the request
      - in: path
        name: id
        description: original id of the release as defined in the client system and
          passed during the creation
      responses:
        200:
          description: OK
      tags:
      - Block
  /api/v1/containers:
    get:
      summary: List Containers
      description: Get all containers currently in the database. Only Containers accessible
        by the user will be reported.
      operationId: getApiV1Containers
      x-api-path-slug: apiv1containers-get
      parameters:
      - in: query
        name: api_token
        description: authentication token of user making the request
      responses:
        200:
          description: OK
      tags:
      - List
      - Containers
    post:
      summary: Create a new Container
      description: |-
        Create a new container.
        If all goes well, a 200 status code is returned.
        If the create fails, a 500 status code is returned.
      operationId: postApiV1Containers
      x-api-path-slug: apiv1containers-post
      parameters:
      - in: query
        name: api_token
        description: authentication token of user making the request
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - New
      - Container
  /api/v1/containers/{id}/events:
    get:
      summary: Get container events
      description: Get the list of Events related to a container
      operationId: getApiV1ContainersEvents
      x-api-path-slug: apiv1containersidevents-get
      parameters:
      - in: query
        name: api_token
        description: authentication token of user making the request
      - in: path
        name: id
        description: id of the Container
      responses:
        200:
          description: OK
      tags:
      - Container
      - Events
  /api/v1/containers/{id}/release:
    put:
      summary: Release
      description: Release a container to an organization.
      operationId: putApiV1ContainersRelease
      x-api-path-slug: apiv1containersidrelease-put
      parameters:
      - in: query
        name: api_token
        description: authentication token of user making the request
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: id of the Container
      responses:
        200:
          description: OK
      tags:
      - Release
  /api/v1/pickup_rights/:
    get:
      summary: List PickupRights
      description: Get all PickupRights that are assigned / transferred to the users's
        Organization.
      operationId: getApiV1PickupRights
      x-api-path-slug: apiv1pickup-rights-get
      parameters:
      - in: query
        name: api_token
        description: authentication token of user making the request
      responses:
        200:
          description: OK
      tags:
      - List
      - PickupRights
  /api/v1/pickup_rights/{id}/request:
    get:
      summary: Request
      description: |-
        When a driver needs to pickup a container, he should send a request to get
        authorization for the pickup. This will return a **temporary pincode**.
        If no authorization is given, http status 403 is returned
      operationId: getApiV1PickupRightsRequest
      x-api-path-slug: apiv1pickup-rightsidrequest-get
      parameters:
      - in: query
        name: api_token
        description: authentication token of user making the request
      - in: path
        name: id
        description: id of the PickupRight
      responses:
        200:
          description: OK
      tags:
      - Request
  /api/v1/pickup_rights/{id}/transfer:
    put:
      summary: Transfer
      description: Transfer the PickupRight to another Organization (a subcontractor).
      operationId: putApiV1PickupRightsTransfer
      x-api-path-slug: apiv1pickup-rightsidtransfer-put
      parameters:
      - in: query
        name: api_token
        description: authentication token of user making the request
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: id of the PickupRight (as reported by List PickupRights)
      responses:
        200:
          description: OK
      tags:
      - Transfer
  /api/v1/pickup_rights/{id}/assign:
    put:
      summary: Assign
      description: Assign the PickupRight to a truck driver.
      operationId: putApiV1PickupRightsAssign
      x-api-path-slug: apiv1pickup-rightsidassign-put
      parameters:
      - in: query
        name: api_token
        description: authentication token of user making the request
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: id of the PickupRight as reported by List PickupRights
      responses:
        200:
          description: OK
      tags:
      - Assign
  /api/v1/pickup_rights/{id}/revoke_assignment:
    put:
      summary: Revoke Assignment
      description: Revoke the current PickupRight assignment. This must be used in
        case you did an assign of a PickupRight to a driver and you want to cancel
        this. This action is only possible as long as the PickupRight is not exercised.
      operationId: putApiV1PickupRightsRevokeAssignment
      x-api-path-slug: apiv1pickup-rightsidrevoke-assignment-put
      parameters:
      - in: query
        name: api_token
        description: authentication token of user making the request
      - in: path
        name: id
        description: id of the PickupRight as reported by List PickupRights
      responses:
        200:
          description: OK
      tags:
      - Revoke
      - Assignment
  /api/v1/pickup_rights/{id}/revoke_transfer:
    put:
      summary: Revoke Transfer
      description: Revoke the current PickupRight transfer. This must be used in case
        you did a transfer of a PickupRight to another Organization and you want to
        cancel this. This action is only possible as long as the PickupRight is not
        assigned.
      operationId: putApiV1PickupRightsRevokeTransfer
      x-api-path-slug: apiv1pickup-rightsidrevoke-transfer-put
      parameters:
      - in: query
        name: api_token
        description: authentication token of user making the request
      - in: path
        name: id
        description: id of the PickupRight as reported by List PickupRights
      responses:
        200:
          description: OK
      tags:
      - Revoke
      - Transfer
  /api/v1/pickups:
    post:
      summary: Create pickup
      description: When the driver has picked up the container, a request should be
        sent to the server to record (create) the pickup. The server will record the
        datetime of the pickup.
      operationId: postApiV1Pickups
      x-api-path-slug: apiv1pickups-post
      parameters:
      - in: query
        name: api_token
        description: authentication token of user making the request
      responses:
        200:
          description: OK
      tags:
      - Pickup
  /api/v1/deliveries:
    post:
      summary: Record delivery
      description: When the driver has delivered the container, a request should be
        sent to the server to record (create) the delivery. Note that a delivery is
        associated with a PickupRight, because the driver who gets a PickupRight,
        will automatically get a right to deliver the container. For that reason,
        the PickupRight must be reported.
      operationId: postApiV1Deliveries
      x-api-path-slug: apiv1deliveries-post
      parameters:
      - in: query
        name: api_token
        description: authentication token of user making the request
      responses:
        200:
          description: OK
      tags:
      - Record
      - Delivery
  /api/v1/coordinates/:
    get:
      summary: Get Coordinates
      description: Get the coordinates of the location with the given name and type.
      operationId: getApiV1Coordinates
      x-api-path-slug: apiv1coordinates-get
      parameters:
      - in: query
        name: api_token
        description: authentication token of user making the request
      - in: query
        name: name
        description: name of the location
      - in: query
        name: type
        description: type of the Location, can be Quay, Depot, Warehouse, InlandTerminal,
          Checkpoint
      responses:
        200:
          description: OK
      tags:
      - Coordinates
  /api/v1/coordinates:
    get:
      summary: Get all coordinates
      description: Get the coordinates of all known locations.
      operationId: getApiV1Coordinates
      x-api-path-slug: apiv1coordinates-get
      parameters:
      - in: query
        name: api_token
        description: authentication token of user making the request
      responses:
        200:
          description: OK
      tags:
      - Coordinates
  /api/v1/locations:
    get:
      summary: List
      description: List all Locations with their details. Locations have a type, name
        and the ISRS Locode.
      operationId: getApiV1Locations
      x-api-path-slug: apiv1locations-get
      parameters:
      - in: query
        name: api_token
        description: authentication token of user making the request
      responses:
        200:
          description: OK
      tags:
      - List
    post:
      summary: Create
      description: Create a new Location
      operationId: postApiV1Locations
      x-api-path-slug: apiv1locations-post
      parameters:
      - in: query
        name: api_token
        description: authentication token of user making the request
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Create
  /api/v1/locations/{id}:
    get:
      summary: Details
      description: Get details of 1 location.
      operationId: getApiV1Locations
      x-api-path-slug: apiv1locationsid-get
      parameters:
      - in: query
        name: api_token
        description: authentication token of user making the request
      - in: path
        name: id
        description: id of the location
      responses:
        200:
          description: OK
      tags:
      - Details
  /api/v1/container_types:
    get:
      summary: List
      description: List all ContainerTypes
      operationId: getApiV1ContainerTypes
      x-api-path-slug: apiv1container-types-get
      parameters:
      - in: query
        name: api_token
        description: authentication token of user making the request
      responses:
        200:
          description: OK
      tags:
      - List
  /api/v1/organizations:
    get:
      summary: List
      description: List all registered organizations.
      operationId: getApiV1Organizations
      x-api-path-slug: apiv1organizations-get
      parameters:
      - in: query
        name: api_token
        description: authentication token of user making the request
      responses:
        200:
          description: OK
      tags:
      - List
    post:
      summary: Register organization
      description: Register an Organization with a name. The name must be unique,
        so if one registers an Organization with a name that is already in use, an
        error will occur.
      operationId: postApiV1Organizations
      x-api-path-slug: apiv1organizations-post
      parameters:
      - in: query
        name: api_token
        description: authentication token of user making the request
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Register
      - Organization
  /api/v1/users:
    get:
      summary: List
      description: List all users registered.
      operationId: getApiV1Users
      x-api-path-slug: apiv1users-get
      parameters:
      - in: query
        name: api_token
        description: authentication token of user making the request
      responses:
        200:
          description: OK
      tags:
      - List
    post:
      summary: Register user
      description: |-
        Register information of a user. Note that the "real" (human) user should have
        an account on the blockchain (upfront). This account is represented by an address on the chain, which is based on the public key of the user. Registering therefore means defining user **properties** like a username, which can then be used to refer to users in a more human-friendly way then by using the account addresses. User registration should be done by the user who owns an account on the chain. As a result of registration, a User contract is created on the chain, which contains the user properties, and which is owned by the user account. From then on, one can use the username to refer to a user on the web/mobile app.
      operationId: postApiV1Users
      x-api-path-slug: apiv1users-post
      parameters:
      - in: query
        name: api_token
        description: authentication token of user making the request
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Register
      - User
  /api/v1/events/:
    post:
      summary: Create an Event
      description: |-
        Used to create an event for a container at a specific location and time.
        Each event is defined by a type.
        Currently a limited number of events (pickup and availability) are supported, but this may be extended with e.g. passage events.
        There are 2 ways to refer to a Container: by means of its id as defined in the Blockchain (this requires recording these ids in your app), or by means of a combination of the blNumber and isoNumber. Similarly, locations can be specified in 2 ways: by means of their id as defined in the Blockchain or by means of their name. In the latter case the name must be defined in a mapping   file for the Organization you - as a user- belong to. Also note that the container may not yet be known in the Blockchain at the time
        an availability event is created!
      operationId: postApiV1Events
      x-api-path-slug: apiv1events-post
      parameters:
      - in: query
        name: api_token
        description: authentication token of user making the request
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Event
  /countries:
    get:
      summary: Get Countries
      description: Get a list of all the countries. The API will return the complete
        list of the existing countries with their country name and 2-character country
        code in JSON format. The example output for a HTTP Status code 200 contains
        a subset of the possible outcome.
      operationId: getCountries
      x-api-path-slug: countries-get
      responses:
        200:
          description: OK
      tags:
      - Countries
  /countries/{countryCode}:
    get:
      summary: Get Countries Countrycode
      description: Get the details of 1 specific country, specified by the country
        code in the query parameter. Both the country name and country code are returned
        in a JSON object. The example response in case of HTTP Status Code 200 contains
        the result when requested for countryCode BE.
      operationId: getCountry
      x-api-path-slug: countriescountrycode-get
      parameters:
      - in: path
        name: countryCode
        description: 2-character country code
      responses:
        200:
          description: OK
      tags:
      - Countries
      - Countrycode
  /countries/{countryCode}/subdivisions:
    get:
      summary: Get Countries Code Subdivisions
      description: Get a list of all the subdivisions of a certain country, specified
        by the country code in the query parameter. The example response contains
        a subset of the output when requested for BE.
      operationId: getCountrySubdivisions
      x-api-path-slug: countriescountrycodesubdivisions-get
      parameters:
      - in: path
        name: countryCode
        description: 2-character country code
      responses:
        200:
          description: OK
      tags:
      - Countries
      - Countrycode
      - Subdivisions
  /countries/{countryCode}/subdivisions/{subdivisionCode}:
    get:
      summary: Get Countries Country Code Subdivisions Code
      description: Get the details of 1 specific subdivision, based on the countryCode
        and subdivisionCode in the query parameters.
      operationId: getCountrySubdivision
      x-api-path-slug: countriescountrycodesubdivisionssubdivisioncode-get
      parameters:
      - in: path
        name: countryCode
        description: 2-character country code
      - in: path
        name: subdivisionCode
        description: 3-character subdivision code
      responses:
        200:
          description: OK
      tags:
      - Countries
      - Countrycode
      - Subdivisions
      - Subdivisioncode
  /locations:
    get:
      summary: Get Locations
      description: This api will return a (paged) list of locations that match the
        search parameters (query parameters) ordered by the name without diacritics.
      operationId: searchLocations
      x-api-path-slug: locations-get
      parameters:
      - in: query
        name: code
        description: 3-character location code
      - in: query
        name: country
        description: 2-character country code
      - in: query
        name: page
        description: the page number to allow paging (needs to be an integer > 0)
      - in: query
        name: searchterm
        description: Part of the name of the location without diacritics
      - in: query
        name: size
        description: the page size to allow paging (needs to be an integer 0 < pagesize
          < 1000)
      - in: query
        name: subdiv
        description: 3-character subdivision code
      responses:
        200:
          description: OK
      tags:
      - Locations
  /locations/{latitude}/{longitude}/{radius}:
    get:
      summary: Get Locations Latitude Longitude Radius
      description: This api will return locations in a certain radius of a point,
        ordered by distance , not necessarily in the same country
      operationId: locations_getinNeighbourhood
      x-api-path-slug: locationslatitudelongituderadius-get
      parameters:
      - in: path
        name: latitude
        description: the latitude of the specified point
      - in: path
        name: longitude
        description: the longitude of the specified point
      - in: query
        name: page
        description: the page number to allow paging (needs to be an integer > 0)
      - in: path
        name: radius
        description: the radius in km (max 75km)
      - in: query
        name: size
        description: the page size to allow paging (needs to be an integer 0 < pagesize
          < 1000)
      responses:
        200:
          description: OK
      tags:
      - Locations
      - Latitude
      - Longitude
      - Radius
  /locations/{locode}:
    get:
      summary: Get Locations Locode
      description: Get the details of 1 location based on the locode.
      operationId: locations_getByCountryAndLocode
      x-api-path-slug: locationslocode-get
      parameters:
      - in: path
        name: locode
        description: 5-character location code (country code + location code)
      responses:
        200:
          description: OK
      tags:
      - Locations
      - Locode
  /stays/{imoNumber}:
    get:
      summary: Get Stay
      description: Get a single stay by IMO number.
      operationId: Stays By ImoNumber
      x-api-path-slug: staysimonumber-get
      parameters:
      - in: path
        name: imoNumber
      responses:
        200:
          description: OK
      tags:
      - Shipping
      - Stays
  /nxtportdocument/{bookingnumber}/{containernumber}:
    get:
      summary: Get VERMAS Files
      description: Returns the VERMAS files with the according booking number and
        container number
      operationId: NxtportdocumentByBookingnumberByContainernumberGet
      x-api-path-slug: nxtportdocumentbookingnumbercontainernumber-get
      parameters:
      - in: path
        name: bookingnumber
        description: bookingnumber
      - in: path
        name: containernumber
        description: containernumber
      - in: header
        name: Ocp-Apim-Subscription-Key
      responses:
        200:
          description: OK
      tags:
      - Shipping
      - VERMAS
      - Files
  /companies:
    get:
      summary: Get Companies
      description: Get companies where name contains input.
      operationId: Company_GetCompaniesOverviewContainingName
      x-api-path-slug: companies-get
      parameters:
      - in: query
        name: name
        description: Name of the company
      responses:
        200:
          description: OK
      tags:
      - Companies
  /companies/{id}:
    get:
      summary: Get Companies
      description: Get a company by its id.
      operationId: Company_GetCompanyById
      x-api-path-slug: companiesid-get
      parameters:
      - in: path
        name: id
        description: Format - uuid
      responses:
        200:
          description: OK
      tags:
      - Companies
  /companies/name/{name}:
    get:
      summary: Get Companies Name Name
      description: Get a company by its name.
      operationId: Company_GetCompanyByName
      x-api-path-slug: companiesnamename-get
      parameters:
      - in: path
        name: name
        description: Name of the company
      responses:
        200:
          description: OK
      tags:
      - Companies
      - Name
      - Name
  /companies/pcs/{pcs}:
    get:
      summary: Get Companies Pcs Pcs
      description: Get a company by its pcs code.
      operationId: Company_GetCompanyByPcs
      x-api-path-slug: companiespcspcs-get
      parameters:
      - in: path
        name: pcs
        description: Pcs code of the company
      responses:
        200:
          description: OK
      tags:
      - Companies
      - Pcs
      - Pcs
  /companies/vat/{vat}:
    get:
      summary: Get Companies Vat Vat
      description: Get a company by its vat.
      operationId: Company_GetCompanyByVat
      x-api-path-slug: companiesvatvat-get
      parameters:
      - in: path
        name: vat
        description: Vat of the company
      responses:
        200:
          description: OK
      tags:
      - Companies
      - Vat
      - Vat
  /vessels/expected:
    get:
      summary: Get Expected Vessels
      description: Get all the expected vessels of BEANR and BEZEE
      operationId: Vessels_Expected
      x-api-path-slug: vesselsexpected-get
      responses:
        200:
          description: OK
      tags:
      - Shipping
      - Vessels
      - Ports
  /vessels/in-port:
    get:
      summary: Get Vessels In Port
      description: Get all the in-port vessels of BEANR and BEZEE
      operationId: Vessels_InPort
      x-api-path-slug: vesselsinport-get
      responses:
        200:
          description: OK
      tags:
      - Shipping
      - Vesses
      - Ports