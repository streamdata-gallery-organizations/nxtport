---
name: NxtPort
x-slug: nxtport
description: NxtPort opens the gates to the Port of the future. This project is a
  milestone in the digitalization of logistics and cargo.
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28835-www-nxtport-eu.jpg
x-kinRank: "7"
x-alexaRank: "3933231"
tags: NxtPort
created: "2018-08-30"
modified: "2018-08-30"
url: https://raw.githubusercontent.com/streamdata-gallery-organizations/nxtport/master/_listings/nxtport/apis.md
specificationVersion: "0.14"
apis:
- name: Bel Air API (staging) - Retrieving supported metrics
  x-api-slug: metrics-get
  description: "The platform allows you to retrieve supported metrics by sending a
    HTTP GET to /metrics. \nThe string-values for the attribute id can be used as
    a metricId path parameter in the City Layer operations. \nThe attribute granularity
    indicates how fine grained temporal pages should be split up when querying individual
    sources (and can be ignored here)."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28835-www-nxtport-eu.jpg
  humanURL: https://www.nxtport.eu
  baseURL: https://api-stg.nxtport.eu//belair/v1
  tags: Technology, SaaS, Enterprise, Shipping, Data, General Data, Relative Data,
    Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/nxtport/master/_listings/nxtport/metrics-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/nxtport/master/_listings/nxtport/metrics-get-openapi.md
- name: Bel Air API (staging) - Retrieve available layers
  x-api-slug: layers-get
  description: "This operation lists the currently available city layers. \nThe returned
    strings can then be used as a layerId path parameter in the /layers operations
    included in this API."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28835-www-nxtport-eu.jpg
  humanURL: https://www.nxtport.eu
  baseURL: https://api-stg.nxtport.eu//belair/v1
  tags: Technology, SaaS, Enterprise, Shipping, Data, General Data, Relative Data,
    Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/nxtport/master/_listings/nxtport/layers-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/nxtport/master/_listings/nxtport/layers-get-openapi.md
- name: Bel Air API (staging) - Retrieve the city layer data for the specified layer,
    metric and date.
  x-api-slug: layerslayeridmetriciddate-get
  description: 'This operation retrieves city layer data for the specified layer,
    metric and date combination. The date is passed in the following format: YYYYMMDD.
    The values for the layerId and metricId can be fetched from the /layers and /metrics
    operations.'
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28835-www-nxtport-eu.jpg
  humanURL: https://www.nxtport.eu
  baseURL: https://api-stg.nxtport.eu//belair/v1
  tags: Technology, SaaS, Enterprise, Shipping, Data, General Data, Relative Data,
    Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/nxtport/master/_listings/nxtport/layerslayeridmetriciddate-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/nxtport/master/_listings/nxtport/layerslayeridmetriciddate-get-openapi.md
- name: Bel Air API (staging) - Retrieve the city layer data for the specified layer,
    metric and date.
  x-api-slug: layerslayeridmetriciddatehour-get
  description: 'This operation retrieves city layer data for the specified layer,
    metric and date combination. The date is passed in the following format: YYYYMMDD.
    The values for the layerId and metricId can be fetched from the /layers and /metrics
    operations.'
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28835-www-nxtport-eu.jpg
  humanURL: https://www.nxtport.eu
  baseURL: https://api-stg.nxtport.eu//belair/v1
  tags: Technology, SaaS, Enterprise, Shipping, Data, General Data, Relative Data,
    Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/nxtport/master/_listings/nxtport/layerslayeridmetriciddatehour-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/nxtport/master/_listings/nxtport/layerslayeridmetriciddatehour-get-openapi.md
- name: Big Belly API (staging) - Publish Device
  x-api-slug: devices-post
  description: Publish the fill level for all Big Belly devices.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28835-www-nxtport-eu.jpg
  humanURL: https://www.nxtport.eu
  baseURL: https://api-stg.nxtport.eu//bigbelly/v1
  tags: Technology, SaaS, Enterprise, Shipping, Data, General Data, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/nxtport/master/_listings/nxtport/devices-post-openapi.md
- name: NxtPort Consignment API (live) - Returns the file with corresponding blnumbers
    and staynumber.
  x-api-slug: nxtportdocumentblnumbersnstaynumber-get
  description: Returns the file with corresponding blnumbers and staynumber..
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28835-www-nxtport-eu.jpg
  humanURL: https://www.nxtport.eu
  baseURL: https://api.nxtport.eu//Consignment/v1
  tags: Technology, SaaS, Enterprise, Shipping, Data, General Data, Relative Data,
    Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/nxtport/master/_listings/nxtport/nxtportdocumentblnumbersnstaynumber-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/nxtport/master/_listings/nxtport/nxtportdocumentblnumbersnstaynumber-get-openapi.md
- name: NxtPort Consignment API (live) - Returns the file with corresponding blnumbers
    and containernumber.
  x-api-slug: nxtportdocumentblnumbercncontainernumber-get
  description: Returns the file with corresponding blnumbers and containernumber..
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28835-www-nxtport-eu.jpg
  humanURL: https://www.nxtport.eu
  baseURL: https://api.nxtport.eu//Consignment/v1
  tags: Technology, SaaS, Enterprise, Shipping, Data, General Data, Relative Data,
    Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/nxtport/master/_listings/nxtport/nxtportdocumentblnumbercncontainernumber-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/nxtport/master/_listings/nxtport/nxtportdocumentblnumbercncontainernumber-get-openapi.md
- name: NxtPort Consignment API (live) - Returns the file with corresponding blnumbers
    and senderID.
  x-api-slug: nxtportdocumentblnumberagagent-get
  description: Returns the file with corresponding blnumbers and senderid..
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28835-www-nxtport-eu.jpg
  humanURL: https://www.nxtport.eu
  baseURL: https://api.nxtport.eu//Consignment/v1
  tags: Technology, SaaS, Enterprise, Shipping, Data, General Data, Relative Data,
    Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/nxtport/master/_listings/nxtport/nxtportdocumentblnumberagagent-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/nxtport/master/_listings/nxtport/nxtportdocumentblnumberagagent-get-openapi.md
- name: T-mining Secure Container Release API (live) - Create release
  x-api-slug: apiv1releases-post
  description: Serves to create a Container together with its PickupRight that gets
    automatically transferred to the consignee.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28835-www-nxtport-eu.jpg
  humanURL: https://www.nxtport.eu
  baseURL: https://api.nxtport.eu//blockchain
  tags: Technology, SaaS, Enterprise, Shipping, Data, General Data, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/nxtport/master/_listings/nxtport/apiv1releases-post-openapi.md
- name: T-mining Secure Container Release API (live) - Block
  x-api-slug: apiv1releasesid-delete
  description: |-
    Blocking a release is done by a delete. This will revoke the PickupRight from the consignee. The Container and its PickupRight are deleted. Afterwards it is still possible to release again.
     The following conditions apply for this to work:
    * the container must have been released, i.e. there must be a vallid PickupRight   for the Container
    * the PickupRight should not be transferred to another Organization than the one that got the relesase initially
    * the PickupRight should not yet be assigned (to a driver / skipper)
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28835-www-nxtport-eu.jpg
  humanURL: https://www.nxtport.eu
  baseURL: https://api.nxtport.eu//blockchain
  tags: Technology, SaaS, Enterprise, Shipping, Data, General Data, Relative Data,
    Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/nxtport/master/_listings/nxtport/apiv1releasesid-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/nxtport/master/_listings/nxtport/apiv1releasesid-delete-openapi.md
- name: T-mining Secure Container Release API (live) - List Containers
  x-api-slug: apiv1containers-get
  description: Get all containers currently in the database. Only Containers accessible
    by the user will be reported.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28835-www-nxtport-eu.jpg
  humanURL: https://www.nxtport.eu
  baseURL: https://api.nxtport.eu//blockchain
  tags: Technology, SaaS, Enterprise, Shipping, Data, General Data, Relative Data,
    Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/nxtport/master/_listings/nxtport/apiv1containers-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/nxtport/master/_listings/nxtport/apiv1containers-get-openapi.md
- name: T-mining Secure Container Release API (live) - Create a new Container
  x-api-slug: apiv1containers-post
  description: |-
    Create a new container.
    If all goes well, a 200 status code is returned.
    If the create fails, a 500 status code is returned.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28835-www-nxtport-eu.jpg
  humanURL: https://www.nxtport.eu
  baseURL: https://api.nxtport.eu//blockchain
  tags: Technology, SaaS, Enterprise, Shipping, Data, General Data, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/nxtport/master/_listings/nxtport/apiv1containers-post-openapi.md
- name: T-mining Secure Container Release API (live) - Get container events
  x-api-slug: apiv1containersidevents-get
  description: Get the list of Events related to a container
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28835-www-nxtport-eu.jpg
  humanURL: https://www.nxtport.eu
  baseURL: https://api.nxtport.eu//blockchain
  tags: Technology, SaaS, Enterprise, Shipping, Data, General Data, Relative Data,
    Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/nxtport/master/_listings/nxtport/apiv1containersidevents-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/nxtport/master/_listings/nxtport/apiv1containersidevents-get-openapi.md
- name: T-mining Secure Container Release API (live) - Release
  x-api-slug: apiv1containersidrelease-put
  description: Release a container to an organization.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28835-www-nxtport-eu.jpg
  humanURL: https://www.nxtport.eu
  baseURL: https://api.nxtport.eu//blockchain
  tags: Technology, SaaS, Enterprise, Shipping, Data, General Data, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/nxtport/master/_listings/nxtport/apiv1containersidrelease-put-openapi.md
- name: T-mining Secure Container Release API (live) - List PickupRights
  x-api-slug: apiv1pickup-rights-get
  description: Get all PickupRights that are assigned / transferred to the users's
    Organization.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28835-www-nxtport-eu.jpg
  humanURL: https://www.nxtport.eu
  baseURL: https://api.nxtport.eu//blockchain
  tags: Technology, SaaS, Enterprise, Shipping, Data, General Data, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/nxtport/master/_listings/nxtport/apiv1pickup-rights-get-openapi.md
- name: T-mining Secure Container Release API (live) - Request
  x-api-slug: apiv1pickup-rightsidrequest-get
  description: |-
    When a driver needs to pickup a container, he should send a request to get
    authorization for the pickup. This will return a **temporary pincode**.
    If no authorization is given, http status 403 is returned
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28835-www-nxtport-eu.jpg
  humanURL: https://www.nxtport.eu
  baseURL: https://api.nxtport.eu//blockchain
  tags: Technology, SaaS, Enterprise, Shipping, Data, General Data, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/nxtport/master/_listings/nxtport/apiv1pickup-rightsidrequest-get-openapi.md
- name: T-mining Secure Container Release API (live) - Transfer
  x-api-slug: apiv1pickup-rightsidtransfer-put
  description: Transfer the PickupRight to another Organization (a subcontractor).
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28835-www-nxtport-eu.jpg
  humanURL: https://www.nxtport.eu
  baseURL: https://api.nxtport.eu//blockchain
  tags: Technology, SaaS, Enterprise, Shipping, Data, General Data, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/nxtport/master/_listings/nxtport/apiv1pickup-rightsidtransfer-put-openapi.md
- name: T-mining Secure Container Release API (live) - Assign
  x-api-slug: apiv1pickup-rightsidassign-put
  description: Assign the PickupRight to a truck driver.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28835-www-nxtport-eu.jpg
  humanURL: https://www.nxtport.eu
  baseURL: https://api.nxtport.eu//blockchain
  tags: Technology, SaaS, Enterprise, Shipping, Data, General Data, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/nxtport/master/_listings/nxtport/apiv1pickup-rightsidassign-put-openapi.md
- name: T-mining Secure Container Release API (live) - Revoke Assignment
  x-api-slug: apiv1pickup-rightsidrevoke-assignment-put
  description: Revoke the current PickupRight assignment. This must be used in case
    you did an assign of a PickupRight to a driver and you want to cancel this. This
    action is only possible as long as the PickupRight is not exercised.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28835-www-nxtport-eu.jpg
  humanURL: https://www.nxtport.eu
  baseURL: https://api.nxtport.eu//blockchain
  tags: Technology, SaaS, Enterprise, Shipping, Data, General Data, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/nxtport/master/_listings/nxtport/apiv1pickup-rightsidrevoke-assignment-put-openapi.md
- name: T-mining Secure Container Release API (live) - Revoke Transfer
  x-api-slug: apiv1pickup-rightsidrevoke-transfer-put
  description: Revoke the current PickupRight transfer. This must be used in case
    you did a transfer of a PickupRight to another Organization and you want to cancel
    this. This action is only possible as long as the PickupRight is not assigned.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28835-www-nxtport-eu.jpg
  humanURL: https://www.nxtport.eu
  baseURL: https://api.nxtport.eu//blockchain
  tags: Technology, SaaS, Enterprise, Shipping, Data, General Data, Relative Data,
    Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/nxtport/master/_listings/nxtport/apiv1pickup-rightsidrevoke-transfer-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/nxtport/master/_listings/nxtport/apiv1pickup-rightsidrevoke-transfer-put-openapi.md
- name: T-mining Secure Container Release API (live) - Create pickup
  x-api-slug: apiv1pickups-post
  description: When the driver has picked up the container, a request should be sent
    to the server to record (create) the pickup. The server will record the datetime
    of the pickup.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28835-www-nxtport-eu.jpg
  humanURL: https://www.nxtport.eu
  baseURL: https://api.nxtport.eu//blockchain
  tags: Technology, SaaS, Enterprise, Shipping, Data, General Data, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/nxtport/master/_listings/nxtport/apiv1pickups-post-openapi.md
- name: T-mining Secure Container Release API (live) - Record delivery
  x-api-slug: apiv1deliveries-post
  description: When the driver has delivered the container, a request should be sent
    to the server to record (create) the delivery. Note that a delivery is associated
    with a PickupRight, because the driver who gets a PickupRight, will automatically
    get a right to deliver the container. For that reason, the PickupRight must be
    reported.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28835-www-nxtport-eu.jpg
  humanURL: https://www.nxtport.eu
  baseURL: https://api.nxtport.eu//blockchain
  tags: Technology, SaaS, Enterprise, Shipping, Data, General Data, Relative Data,
    Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/nxtport/master/_listings/nxtport/apiv1deliveries-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/nxtport/master/_listings/nxtport/apiv1deliveries-post-openapi.md
- name: T-mining Secure Container Release API (live) - Get Coordinates
  x-api-slug: apiv1coordinates-get
  description: Get the coordinates of the location with the given name and type.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28835-www-nxtport-eu.jpg
  humanURL: https://www.nxtport.eu
  baseURL: https://api.nxtport.eu//blockchain
  tags: Technology, SaaS, Enterprise, Shipping, Data, General Data, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/nxtport/master/_listings/nxtport/apiv1coordinates-get-openapi.md
- name: T-mining Secure Container Release API (live) - Get all coordinates
  x-api-slug: apiv1coordinates-get
  description: Get the coordinates of all known locations.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28835-www-nxtport-eu.jpg
  humanURL: https://www.nxtport.eu
  baseURL: https://api.nxtport.eu//blockchain
  tags: Technology, SaaS, Enterprise, Shipping, Data, General Data, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/nxtport/master/_listings/nxtport/apiv1coordinates-get-openapi.md
- name: T-mining Secure Container Release API (live) - List
  x-api-slug: apiv1locations-get
  description: List all Locations with their details. Locations have a type, name
    and the ISRS Locode.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28835-www-nxtport-eu.jpg
  humanURL: https://www.nxtport.eu
  baseURL: https://api.nxtport.eu//blockchain
  tags: Technology, SaaS, Enterprise, Shipping, Data, General Data, Relative Data,
    Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/nxtport/master/_listings/nxtport/apiv1locations-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/nxtport/master/_listings/nxtport/apiv1locations-get-openapi.md
- name: T-mining Secure Container Release API (live) - Create
  x-api-slug: apiv1locations-post
  description: Create a new Location
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28835-www-nxtport-eu.jpg
  humanURL: https://www.nxtport.eu
  baseURL: https://api.nxtport.eu//blockchain
  tags: Technology, SaaS, Enterprise, Shipping, Data, General Data, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/nxtport/master/_listings/nxtport/apiv1locations-post-openapi.md
- name: T-mining Secure Container Release API (live) - Details
  x-api-slug: apiv1locationsid-get
  description: Get details of 1 location.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28835-www-nxtport-eu.jpg
  humanURL: https://www.nxtport.eu
  baseURL: https://api.nxtport.eu//blockchain
  tags: Technology, SaaS, Enterprise, Shipping, Data, General Data, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/nxtport/master/_listings/nxtport/apiv1locationsid-get-openapi.md
- name: T-mining Secure Container Release API (live) - List
  x-api-slug: apiv1container-types-get
  description: List all ContainerTypes
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28835-www-nxtport-eu.jpg
  humanURL: https://www.nxtport.eu
  baseURL: https://api.nxtport.eu//blockchain
  tags: Technology, SaaS, Enterprise, Shipping, Data, General Data, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/nxtport/master/_listings/nxtport/apiv1container-types-get-openapi.md
- name: T-mining Secure Container Release API (live) - List
  x-api-slug: apiv1organizations-get
  description: List all registered organizations.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28835-www-nxtport-eu.jpg
  humanURL: https://www.nxtport.eu
  baseURL: https://api.nxtport.eu//blockchain
  tags: Technology, SaaS, Enterprise, Shipping, Data, General Data, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/nxtport/master/_listings/nxtport/apiv1organizations-get-openapi.md
- name: T-mining Secure Container Release API (live) - Register organization
  x-api-slug: apiv1organizations-post
  description: Register an Organization with a name. The name must be unique, so if
    one registers an Organization with a name that is already in use, an error will
    occur.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28835-www-nxtport-eu.jpg
  humanURL: https://www.nxtport.eu
  baseURL: https://api.nxtport.eu//blockchain
  tags: Technology, SaaS, Enterprise, Shipping, Data, General Data, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/nxtport/master/_listings/nxtport/apiv1organizations-post-openapi.md
- name: T-mining Secure Container Release API (live) - List
  x-api-slug: apiv1users-get
  description: List all users registered.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28835-www-nxtport-eu.jpg
  humanURL: https://www.nxtport.eu
  baseURL: https://api.nxtport.eu//blockchain
  tags: Technology, SaaS, Enterprise, Shipping, Data, General Data, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/nxtport/master/_listings/nxtport/apiv1users-get-openapi.md
- name: T-mining Secure Container Release API (live) - Register user
  x-api-slug: apiv1users-post
  description: |-
    Register information of a user. Note that the "real" (human) user should have
    an account on the blockchain (upfront). This account is represented by an address on the chain, which is based on the public key of the user. Registering therefore means defining user **properties** like a username, which can then be used to refer to users in a more human-friendly way then by using the account addresses. User registration should be done by the user who owns an account on the chain. As a result of registration, a User contract is created on the chain, which contains the user properties, and which is owned by the user account. From then on, one can use the username to refer to a user on the web/mobile app.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28835-www-nxtport-eu.jpg
  humanURL: https://www.nxtport.eu
  baseURL: https://api.nxtport.eu//blockchain
  tags: Technology, SaaS, Enterprise, Shipping, Data, General Data, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/nxtport/master/_listings/nxtport/apiv1users-post-openapi.md
- name: T-mining Secure Container Release API (live) - Create an Event
  x-api-slug: apiv1events-post
  description: |-
    Used to create an event for a container at a specific location and time.
    Each event is defined by a type.
    Currently a limited number of events (pickup and availability) are supported, but this may be extended with e.g. passage events.
    There are 2 ways to refer to a Container: by means of its id as defined in the Blockchain (this requires recording these ids in your app), or by means of a combination of the blNumber and isoNumber. Similarly, locations can be specified in 2 ways: by means of their id as defined in the Blockchain or by means of their name. In the latter case the name must be defined in a mapping   file for the Organization you - as a user- belong to. Also note that the container may not yet be known in the Blockchain at the time
    an availability event is created!
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28835-www-nxtport-eu.jpg
  humanURL: https://www.nxtport.eu
  baseURL: https://api.nxtport.eu//blockchain
  tags: Technology, SaaS, Enterprise, Shipping, Data, General Data, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/nxtport/master/_listings/nxtport/apiv1events-post-openapi.md
- name: UN Location Codes API (live) - Get Countries
  x-api-slug: countries-get
  description: Get a list of all the countries. The API will return the complete list
    of the existing countries with their country name and 2-character country code
    in JSON format. The example output for a HTTP Status code 200 contains a subset
    of the possible outcome.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28835-www-nxtport-eu.jpg
  humanURL: https://www.nxtport.eu
  baseURL: https://api.nxtport.eu//unlocodes/v1
  tags: Technology, SaaS, Enterprise, Shipping, Data, General Data, Relative Data,
    Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/nxtport/master/_listings/nxtport/countries-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/nxtport/master/_listings/nxtport/countries-get-openapi.md
- name: UN Location Codes API (live) - Get Countries Countrycode
  x-api-slug: countriescountrycode-get
  description: Get the details of 1 specific country, specified by the country code
    in the query parameter. Both the country name and country code are returned in
    a JSON object. The example response in case of HTTP Status Code 200 contains the
    result when requested for countryCode BE.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28835-www-nxtport-eu.jpg
  humanURL: https://www.nxtport.eu
  baseURL: https://api.nxtport.eu//unlocodes/v1
  tags: Technology, SaaS, Enterprise, Shipping, Data, General Data, Relative Data,
    Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/nxtport/master/_listings/nxtport/countriescountrycode-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/nxtport/master/_listings/nxtport/countriescountrycode-get-openapi.md
- name: UN Location Codes API (live) - Get Countries Code Subdivisions
  x-api-slug: countriescountrycodesubdivisions-get
  description: Get a list of all the subdivisions of a certain country, specified
    by the country code in the query parameter. The example response contains a subset
    of the output when requested for BE.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28835-www-nxtport-eu.jpg
  humanURL: https://www.nxtport.eu
  baseURL: https://api.nxtport.eu//unlocodes/v1
  tags: Technology, SaaS, Enterprise, Shipping, Data, General Data, Relative Data,
    Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/nxtport/master/_listings/nxtport/countriescountrycodesubdivisions-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/nxtport/master/_listings/nxtport/countriescountrycodesubdivisions-get-openapi.md
- name: UN Location Codes API (live) - Get Countries Country Code Subdivisions Code
  x-api-slug: countriescountrycodesubdivisionssubdivisioncode-get
  description: Get the details of 1 specific subdivision, based on the countryCode
    and subdivisionCode in the query parameters.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28835-www-nxtport-eu.jpg
  humanURL: https://www.nxtport.eu
  baseURL: https://api.nxtport.eu//unlocodes/v1
  tags: Technology, SaaS, Enterprise, Shipping, Data, General Data, Relative Data,
    Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/nxtport/master/_listings/nxtport/countriescountrycodesubdivisionssubdivisioncode-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/nxtport/master/_listings/nxtport/countriescountrycodesubdivisionssubdivisioncode-get-openapi.md
- name: UN Location Codes API (live) - Get Locations
  x-api-slug: locations-get
  description: This api will return a (paged) list of locations that match the search
    parameters (query parameters) ordered by the name without diacritics.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28835-www-nxtport-eu.jpg
  humanURL: https://www.nxtport.eu
  baseURL: https://api.nxtport.eu//unlocodes/v1
  tags: Technology, SaaS, Enterprise, Shipping, Data, General Data, Relative Data,
    Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/nxtport/master/_listings/nxtport/locations-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/nxtport/master/_listings/nxtport/locations-get-openapi.md
- name: UN Location Codes API (live) - Get Locations Latitude Longitude Radius
  x-api-slug: locationslatitudelongituderadius-get
  description: This api will return locations in a certain radius of a point, ordered
    by distance , not necessarily in the same country
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28835-www-nxtport-eu.jpg
  humanURL: https://www.nxtport.eu
  baseURL: https://api.nxtport.eu//unlocodes/v1
  tags: Technology, SaaS, Enterprise, Shipping, Data, General Data, Relative Data,
    Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/nxtport/master/_listings/nxtport/locationslatitudelongituderadius-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/nxtport/master/_listings/nxtport/locationslatitudelongituderadius-get-openapi.md
- name: UN Location Codes API (live) - Get Locations Locode
  x-api-slug: locationslocode-get
  description: Get the details of 1 location based on the locode.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28835-www-nxtport-eu.jpg
  humanURL: https://www.nxtport.eu
  baseURL: https://api.nxtport.eu//unlocodes/v1
  tags: Technology, SaaS, Enterprise, Shipping, Data, General Data, Relative Data,
    Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/nxtport/master/_listings/nxtport/locationslocode-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/nxtport/master/_listings/nxtport/locationslocode-get-openapi.md
- name: Vessel Stay API (live) - Get Stay
  x-api-slug: staysimonumber-get
  description: Get a single stay by IMO number.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28835-www-nxtport-eu.jpg
  humanURL: https://www.nxtport.eu
  baseURL: https://api.nxtport.eu//sa/v1
  tags: Technology, SaaS, Enterprise, Shipping, Data, General Data, Relative Data,
    Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/nxtport/master/_listings/nxtport/staysimonumber-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/nxtport/master/_listings/nxtport/staysimonumber-get-openapi.md
- name: VGM API (live) - Get VERMAS Files
  x-api-slug: nxtportdocumentbookingnumbercontainernumber-get
  description: Returns the VERMAS files with the according booking number and container
    number
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28835-www-nxtport-eu.jpg
  humanURL: https://www.nxtport.eu
  baseURL: https://api.nxtport.eu//VGM/v1
  tags: Technology, SaaS, Enterprise, Shipping, Data, General Data, Relative Data,
    Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/nxtport/master/_listings/nxtport/nxtportdocumentbookingnumbercontainernumber-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/nxtport/master/_listings/nxtport/nxtportdocumentbookingnumbercontainernumber-get-openapi.md
- name: Port+ Portdirectory API (live) - Get Companies
  x-api-slug: companies-get
  description: Get companies where name contains input.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28835-www-nxtport-eu.jpg
  humanURL: https://www.nxtport.eu
  baseURL: https://api.nxtport.eu//portdirectory/v1
  tags: Technology, SaaS, Enterprise, Shipping, Data, General Data, Relative Data,
    Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/nxtport/master/_listings/nxtport/companies-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/nxtport/master/_listings/nxtport/companies-get-openapi.md
- name: Port+ Portdirectory API (live) - Get Companies
  x-api-slug: companiesid-get
  description: Get a company by its id.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28835-www-nxtport-eu.jpg
  humanURL: https://www.nxtport.eu
  baseURL: https://api.nxtport.eu//portdirectory/v1
  tags: Technology, SaaS, Enterprise, Shipping, Data, General Data, Relative Data,
    Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/nxtport/master/_listings/nxtport/companiesid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/nxtport/master/_listings/nxtport/companiesid-get-openapi.md
- name: Port+ Portdirectory API (live) - Get Companies Name Name
  x-api-slug: companiesnamename-get
  description: Get a company by its name.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28835-www-nxtport-eu.jpg
  humanURL: https://www.nxtport.eu
  baseURL: https://api.nxtport.eu//portdirectory/v1
  tags: Technology, SaaS, Enterprise, Shipping, Data, General Data, Relative Data,
    Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/nxtport/master/_listings/nxtport/companiesnamename-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/nxtport/master/_listings/nxtport/companiesnamename-get-openapi.md
- name: Port+ Portdirectory API (live) - Get Companies Pcs Pcs
  x-api-slug: companiespcspcs-get
  description: Get a company by its pcs code.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28835-www-nxtport-eu.jpg
  humanURL: https://www.nxtport.eu
  baseURL: https://api.nxtport.eu//portdirectory/v1
  tags: Technology, SaaS, Enterprise, Shipping, Data, General Data, Relative Data,
    Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/nxtport/master/_listings/nxtport/companiespcspcs-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/nxtport/master/_listings/nxtport/companiespcspcs-get-openapi.md
- name: Port+ Portdirectory API (live) - Get Companies Vat Vat
  x-api-slug: companiesvatvat-get
  description: Get a company by its vat.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28835-www-nxtport-eu.jpg
  humanURL: https://www.nxtport.eu
  baseURL: https://api.nxtport.eu//portdirectory/v1
  tags: Technology, SaaS, Enterprise, Shipping, Data, General Data, Relative Data,
    Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/nxtport/master/_listings/nxtport/companiesvatvat-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/nxtport/master/_listings/nxtport/companiesvatvat-get-openapi.md
- name: Portcall+ API (sandbox) - Get Expected Vessels
  x-api-slug: vesselsexpected-get
  description: Get all the expected vessels of BEANR and BEZEE
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28835-www-nxtport-eu.jpg
  humanURL: https://www.nxtport.eu
  baseURL: https://api-sb.nxtport.eu//PortCallPlus/v1
  tags: Technology, SaaS, Enterprise, Shipping, Data, General Data, Relative Data,
    Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/nxtport/master/_listings/nxtport/vesselsexpected-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/nxtport/master/_listings/nxtport/vesselsexpected-get-openapi.md
- name: Portcall+ API (sandbox) - Get Vessels In Port
  x-api-slug: vesselsinport-get
  description: Get all the in-port vessels of BEANR and BEZEE
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28835-www-nxtport-eu.jpg
  humanURL: https://www.nxtport.eu
  baseURL: https://api-sb.nxtport.eu//PortCallPlus/v1
  tags: Technology, SaaS, Enterprise, Shipping, Data, General Data, Relative Data,
    Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/nxtport/master/_listings/nxtport/vesselsinport-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/nxtport/master/_listings/nxtport/vesselsinport-get-openapi.md
x-common:
- type: x-api-gallery
  url: http://npr.api.gallery.streamdata.io
- type: x-api-stack
  url: http://nxtport.stack.network
- type: x-email
  url: mail@nxtport.eu
- type: x-email
  url: development@nxtport.eu
- type: x-email
  url: privacy@nxtport.eu
- type: x-github
  url: https://github.com/NxtPort
- type: x-openapi
  url: https://github.com/NxtPort/nxtport.github.io/tree/master/api
- type: x-twitter
  url: https://twitter.com/NxtPortNews
- type: x-website
  url: https://www.nxtport.eu
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---