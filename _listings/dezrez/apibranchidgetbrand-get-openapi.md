---
swagger: "2.0"
x-collection-name: Dezrez
x-complete: 0
info:
  title: Dezrez Get a specific brand by brandId or default brand within a branch if
    brandId is not supplied.
  version: 1.0.0
  description: Get a specific brand by brandid or default brand within a branch if
    brandid is not supplied..
host: api.dezrez.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/stationary/html/{brandId}:
    get:
      summary: "Does a simple merge of the selected envelopeTemplatePack using the
        data supplied\r\nwill only use certain merge functions, and the correspondence
        can only contain one envelope and the envelope can only contain one document."
      description: "Does a simple merge of the selected envelopetemplatepack using
        the data supplied\r\nwill only use certain merge functions, and the correspondence
        can only contain one envelope and the envelope can only contain one document.."
      operationId: Stationary_HtmlStationaryBybrandId
      x-api-path-slug: apistationaryhtmlbrandid-get
      parameters:
      - in: path
        name: brandId
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Does
      - Simple
      - Merge
      - Of
      - Selected
      - EnvelopeTemplatePack
      - Using
      - Data
      - "Supplied\r\nWill"
      - Only
      - Use
      - Certain
      - Merge
      - Functions
      - ""
      - Correspondence
      - Can
      - Only
      - Contain
      - Envelope
      - Envelope
      - Can
      - Only
      - Contain
      - Document
  /api/stationary/sms/{brandId}:
    get:
      summary: "Does a simple merge of the selected envelopeTemplatePack using the
        data supplied\r\nwill only use certain merge functions, and the correspondence
        can only contain one envelope and the envelope can only contain one document."
      description: "Does a simple merge of the selected envelopetemplatepack using
        the data supplied\r\nwill only use certain merge functions, and the correspondence
        can only contain one envelope and the envelope can only contain one document.."
      operationId: Stationary_SmsStationaryBybrandId
      x-api-path-slug: apistationarysmsbrandid-get
      parameters:
      - in: path
        name: brandId
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Does
      - Simple
      - Merge
      - Of
      - Selected
      - EnvelopeTemplatePack
      - Using
      - Data
      - "Supplied\r\nWill"
      - Only
      - Use
      - Certain
      - Merge
      - Functions
      - ""
      - Correspondence
      - Can
      - Only
      - Contain
      - Envelope
      - Envelope
      - Can
      - Only
      - Contain
      - Document
  /api/agency/{id}/getbrand:
    get:
      summary: Get a specific brand by brandId or default agency brand if brandId
        is not supplied.
      description: Get a specific brand by brandid or default agency brand if brandid
        is not supplied..
      operationId: Agency_GetAgencyBrandByidBybrandId
      x-api-path-slug: apiagencyidgetbrand-get
      parameters:
      - in: query
        name: brandId
        description: The id of brand to get
      - in: path
        name: id
        description: The id of an agency
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Specific
      - Brand
      - By
      - BrandId
      - Default
      - Agency
      - Brand
      - If
      - BrandId
      - Is
      - Not
      - Supplied
  /api/branch/{id}/getbrand:
    get:
      summary: Get a specific brand by brandId or default brand within a branch if
        brandId is not supplied.
      description: Get a specific brand by brandid or default brand within a branch
        if brandid is not supplied..
      operationId: Branch_GetBranchBrandByidBybrandId
      x-api-path-slug: apibranchidgetbrand-get
      parameters:
      - in: query
        name: brandId
        description: The id of brand to get
      - in: path
        name: id
        description: The id of a branch
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Specific
      - Brand
      - By
      - BrandId
      - Default
      - Brand
      - Within
      - Branch
      - If
      - BrandId
      - Is
      - Not
      - Supplied
  /api/people/findbyemail:
    get:
      summary: Returns a list of people that have the supplied email address.
      description: Returns a list of people that have the supplied email address..
      operationId: People_GetPeopleWithEmailAddressByemailAddress
      x-api-path-slug: apipeoplefindbyemail-get
      parameters:
      - in: query
        name: emailAddress
        description: The email address
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Returns
      - List
      - Of
      - People
      - That
      - Have
      - Supplied
      - Email
      - Address
  /api/property/{id}/addgrouptoproperty:
    put:
      summary: Creates/Adds a group to the CurrentOwners of the supplied PropertyId
      description: Creates/adds a group to the currentowners of the supplied propertyid.
      operationId: Property_AddGroupToPropertyByidBydatacontract
      x-api-path-slug: apipropertyidaddgrouptoproperty-put
      parameters:
      - in: body
        name: datacontract
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: The property id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Creates
      - S
      - Group
      - To
      - CurrentOwners
      - Of
      - Supplied
      - PropertyId
  /api/receipt/recordpayment:
    post:
      summary: Makes payment to supplied account.
      description: Makes payment to supplied account..
      operationId: Receipt_RecordPaymentByrecordPaymentDataContract
      x-api-path-slug: apireceiptrecordpayment-post
      parameters:
      - in: body
        name: recordPaymentDataContract
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Makes
      - Payment
      - To
      - Supplied
      - Account
  /api/role/{id}/addgrouptopropertyrole:
    put:
      summary: Creates/Adds a group to the supplied roleId
      description: Creates/adds a group to the supplied roleid.
      operationId: Role_AddGroupToPropertyRoleByidBydatacontract
      x-api-path-slug: apiroleidaddgrouptopropertyrole-put
      parameters:
      - in: body
        name: datacontract
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: The role id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Creates
      - S
      - Group
      - To
      - Supplied
      - RoleId
  /api/role/sales/{id}/getepc:
    get:
      summary: Gets EPC from the supplied propertyRoleId
      description: Gets epc from the supplied propertyroleid.
      operationId: SalesRole_GetEPCByid
      x-api-path-slug: apirolesalesidgetepc-get
      parameters:
      - in: path
        name: id
        description: The role id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - S
      - EPC
      - From
      - Supplied
      - PropertyRoleId
  /api/role/sales/{id}/saveepc:
    post:
      summary: Creates/Overrides the EPC for the supplied propertyRoleId
      description: Creates/overrides the epc for the supplied propertyroleid.
      operationId: SalesRole_SaveEPCByidBydatacontract
      x-api-path-slug: apirolesalesidsaveepc-post
      parameters:
      - in: body
        name: datacontract
        description: The EPC information
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: The role id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Creates
      - Overrides
      - EPCthe
      - Supplied
      - PropertyRoleId
  /api/tenantreferncing/case/{tenancyRoleId}:
    get:
      summary: Gets a tenancy referencing case based on the role id supplied
      description: Gets a tenancy referencing case based on the role id supplied.
      operationId: TenantReferencing_GetCaseBytenancyRoleId
      x-api-path-slug: apitenantreferncingcasetenancyroleid-get
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: path
        name: tenancyRoleId
        description: The id of the tenancy role the case linked to
      responses:
        200:
          description: OK
      tags:
      - S
      - Tenancy
      - Referencing
      - Case
      - Based
      - "On"
      - Role
      - Id
      - Supplied
    post:
      summary: Creates a tenancy referencing case using the role id supplied
      description: Creates a tenancy referencing case using the role id supplied.
      operationId: TenantReferencing_CreateCaseBytenancyRoleId
      x-api-path-slug: apitenantreferncingcasetenancyroleid-post
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: path
        name: tenancyRoleId
        description: The tenancy id the created case will be linked to
      responses:
        200:
          description: OK
      tags:
      - Creates
      - Tenancy
      - Referencing
      - Case
      - Using
      - Role
      - Id
      - Supplied
  /api/tenantreferncing/addapplication/{caseId}/{tenancyRoleId}/{personId}/{productId}:
    post:
      summary: Creates a tenancy referencing application for a case using the details
        supplied
      description: Creates a tenancy referencing application for a case using the
        details supplied.
      operationId: TenantReferencing_CreateApplicationBycaseIdBytenancyRoleIdBypersonIdByproductId
      x-api-path-slug: apitenantreferncingaddapplicationcaseidtenancyroleidpersonidproductid-post
      parameters:
      - in: path
        name: caseId
        description: The id of the case to add the Application to
      - in: path
        name: personId
        description: The id of the individual the application is for
      - in: path
        name: productId
        description: The id of the product the client has chosen
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: path
        name: tenancyRoleId
        description: The role id of the tenancy the case is linked to
      responses:
        200:
          description: OK
      tags:
      - Creates
      - Tenancy
      - Referencing
      - Applicationa
      - Case
      - Using
      - Details
      - Supplied
  /api/tenantreferncing/addguarantor/{caseId}/{tenancyRoleId}/{personId}:
    post:
      summary: Adds a Guarantor to a tenancy referencing application for a case using
        the details supplied
      description: Adds a guarantor to a tenancy referencing application for a case
        using the details supplied.
      operationId: TenantReferencing_CreateApplicationBycaseIdBytenancyRoleIdBypersonId
      x-api-path-slug: apitenantreferncingaddguarantorcaseidtenancyroleidpersonid-post
      parameters:
      - in: path
        name: caseId
        description: The id of the case to add the Guarantor to
      - in: path
        name: personId
        description: The id of the individual the application is for
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: path
        name: tenancyRoleId
        description: The role id of the tenancy the case is linked to
      responses:
        200:
          description: OK
      tags:
      - S
      - Guarantor
      - To
      - Tenancy
      - Referencing
      - Applicationa
      - Case
      - Using
      - Details
      - Supplied
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