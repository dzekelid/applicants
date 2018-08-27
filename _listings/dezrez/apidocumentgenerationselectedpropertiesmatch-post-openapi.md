---
swagger: "2.0"
x-collection-name: Dezrez
x-complete: 0
info:
  title: Dezrez Generates a correspondence to a single applicant, sending them user
    selected property roles
  version: 1.0.0
  description: Generates a correspondence to a single applicant, sending them user
    selected property roles.
host: api.dezrez.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/documentgeneration/singlepropertymatch:
    post:
      summary: Generates a correspondence to multiple applicants, sending them all
        the same property role
      description: Generates a correspondence to multiple applicants, sending them
        all the same property role.
      operationId: DocumentGeneration_SendPropertyToApplicantListBygeneratePackDetails
      x-api-path-slug: apidocumentgenerationsinglepropertymatch-post
      parameters:
      - in: body
        name: generatePackDetails
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Generates
      - Correspondence
      - To
      - Multiple
      - Applicants
      - ""
      - Sending
      - Them
      - ""
      - Same
      - Property
      - Role
  /api/documentgeneration/singlelettingspropertymatch:
    post:
      summary: Generates a correspondence to multiple applicants, sending them all
        the same letting property role
      description: Generates a correspondence to multiple applicants, sending them
        all the same letting property role.
      operationId: DocumentGeneration_SendLettingsPropertyToApplicantListBygeneratePackDetails
      x-api-path-slug: apidocumentgenerationsinglelettingspropertymatch-post
      parameters:
      - in: body
        name: generatePackDetails
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Generates
      - Correspondence
      - To
      - Multiple
      - Applicants
      - ""
      - Sending
      - Them
      - ""
      - Same
      - Letting
      - Property
      - Role
  /api/documentgeneration/printablepropertylist:
    post:
      summary: Generates a printable property list, it is targetless so there is no
        reference to applicants or owners
      description: Generates a printable property list, it is targetless so there
        is no reference to applicants or owners.
      operationId: DocumentGeneration_PrintablePropertyListBygeneratePackDetails
      x-api-path-slug: apidocumentgenerationprintablepropertylist-post
      parameters:
      - in: body
        name: generatePackDetails
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Generates
      - Printable
      - Property
      - List
      - ""
      - It
      - Is
      - Targetless
      - So
      - There
      - Is
      - "No"
      - Reference
      - To
      - Applicants
      - Owners
  /api/documentgeneration/multipropertymatch:
    post:
      summary: Generates a correspondence to multiple applicants, sending them a filtered
        set of the matching property roles
      description: Generates a correspondence to multiple applicants, sending them
        a filtered set of the matching property roles.
      operationId: DocumentGeneration_SendAutoMatchedPropertiesToApplicantListBygeneratePackDetails
      x-api-path-slug: apidocumentgenerationmultipropertymatch-post
      parameters:
      - in: body
        name: generatePackDetails
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Generates
      - Correspondence
      - To
      - Multiple
      - Applicants
      - ""
      - Sending
      - Them
      - Filtered
      - Set
      - Of
      - Matching
      - Property
      - Roles
  /api/documentgeneration/multilettingspropertymatch:
    post:
      summary: Generates a correspondence to multiple letting applicants, sending
        them a filtered set of the matching letting property roles
      description: Generates a correspondence to multiple letting applicants, sending
        them a filtered set of the matching letting property roles.
      operationId: DocumentGeneration_SendAutoMatchedLettingsPropertiesToApplicantListBygeneratePackDetails
      x-api-path-slug: apidocumentgenerationmultilettingspropertymatch-post
      parameters:
      - in: body
        name: generatePackDetails
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Generates
      - Correspondence
      - To
      - Multiple
      - Letting
      - Applicants
      - ""
      - Sending
      - Them
      - Filtered
      - Set
      - Of
      - Matching
      - Letting
      - Property
      - Roles
  /api/documentgeneration/selectedpropertiesmatch:
    post:
      summary: Generates a correspondence to a single applicant, sending them user
        selected property roles
      description: Generates a correspondence to a single applicant, sending them
        user selected property roles.
      operationId: DocumentGeneration_SendSelectedPropertiesToApplicantBygeneratePackDetails
      x-api-path-slug: apidocumentgenerationselectedpropertiesmatch-post
      parameters:
      - in: body
        name: generatePackDetails
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Generates
      - Correspondence
      - To
      - Single
      - Applicant
      - ""
      - Sending
      - Them
      - User
      - Selected
      - Property
      - Roles
  /api/documentgeneration/selectedlettingspropertiesmatch:
    post:
      summary: Generates a correspondence to a single letting applicant, sending them
        user selected property roles
      description: Generates a correspondence to a single letting applicant, sending
        them user selected property roles.
      operationId: DocumentGeneration_SendSelectedLettingsPropertiesToApplicantBygeneratePackDetails
      x-api-path-slug: apidocumentgenerationselectedlettingspropertiesmatch-post
      parameters:
      - in: body
        name: generatePackDetails
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Generates
      - Correspondence
      - To
      - Single
      - Letting
      - Applicant
      - ""
      - Sending
      - Them
      - User
      - Selected
      - Property
      - Roles
  /api/documentgeneration/salesapplicantwelcomepack:
    post:
      summary: Generates a correspondence to a an sales applicant
      description: Generates a correspondence to a an sales applicant.
      operationId: DocumentGeneration_SalesApplicantWelcomePackBygeneratePackDetails
      x-api-path-slug: apidocumentgenerationsalesapplicantwelcomepack-post
      parameters:
      - in: body
        name: generatePackDetails
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Generates
      - Correspondence
      - To
      - Sales
      - Applicant
  /api/documentgeneration/lettingsapplicantwelcomepack:
    post:
      summary: Generates a correspondence to a an lettings applicant
      description: Generates a correspondence to a an lettings applicant.
      operationId: DocumentGeneration_LettingsApplicantWelcomePackBygeneratePackDetails
      x-api-path-slug: apidocumentgenerationlettingsapplicantwelcomepack-post
      parameters:
      - in: body
        name: generatePackDetails
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Generates
      - Correspondence
      - To
      - Lettings
      - Applicant
  /api/documentgeneration/vendorwelcomepack:
    post:
      summary: Generates a correspondence to a an lettings applicant
      description: Generates a correspondence to a an lettings applicant.
      operationId: DocumentGeneration_VendorWelcomePackBygeneratePackDetails
      x-api-path-slug: apidocumentgenerationvendorwelcomepack-post
      parameters:
      - in: body
        name: generatePackDetails
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Generates
      - Correspondence
      - To
      - Lettings
      - Applicant
  /api/group/basicapplicantheatmap:
    get:
      summary: Return the lat and longs for every applicant in the system
      description: Return the lat and longs for every applicant in the system.
      operationId: Group_BasicApplicantHeatMapBypageSizeByfilter.rangeFromByfilter.rangeToByfilter.branchIdByfilter.rol
      x-api-path-slug: apigroupbasicapplicantheatmap-get
      parameters:
      - in: query
        name: filter.branchId
      - in: query
        name: filter.rangeFrom
      - in: query
        name: filter.rangeTo
      - in: query
        name: filter.roleTypes
      - in: query
        name: pageSize
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Return
      - Lat
      - Longsevery
      - Applicant
      - In
      - System
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