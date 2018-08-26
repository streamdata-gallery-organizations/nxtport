---
swagger: "2.0"
x-collection-name: NxtPort
x-complete: 0
info:
  title: Port+ Portdirectory API Get Companies Vat Vat
  description: Get a company by its vat.
  version: 1.0.0
host: api.nxtport.eu
basePath: /portdirectory/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
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
x-streamrank:
  polling_total_time_average: 0
  polling_size_download_average: 0
  streaming_total_time_average: 0
  streaming_size_download_average: 0
  change_yes: 0
  change_no: 0
  time_percentage: 0
  size_percentage: 0
  change_percentage: 0
  last_run: ""
  days_run: 0
  minute_run: 0
---