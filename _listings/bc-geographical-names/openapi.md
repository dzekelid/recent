swagger: "2.0"
x-collection-name: BC Geographical Names
x-complete: 1
info:
  title: Geo Mark Web Service
  description: the-geomark-web-service-allows-you-to-create-and-share-geographic-areas-of-interest-over-the-web-in-a-variety-of-formats-and-coordinate-systems--this-service-is-especially-helpful-when-you-need-to-share-an-area-of-interest-with-people-who-require-that-the-data-be-in-a-different-format-or-they-use-different-mapping-software-
  termsOfService: http://www2.gov.bc.ca/gov/content/governments/about-the-bc-government/databc/open-data/api-terms-of-use-for-ogl-information
  contact:
    name: Data BC
    url: http://data.gov.bc.ca/
    email: DataBCBA@gov.bc.ca
  version: 4.1.2
host: apps.gov.bc.ca
basePath: /pub/geomark
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /names/decisions/recent:
    get:
      summary: Search for names affected by recent naming decision
      description: Search for information about geographical names affected by naming
        'decisions' made by the BC Geographical Names Office (naming authority) within
        the last X days.
      operationId: search-for-information-about-geographical-names-affected-by-naming-decisions-made-by-the-bc-geograph
      x-api-path-slug: namesdecisionsrecent-get
      parameters:
      - in: query
        name: days
        description: The number of days used to define the time window of naming decisions
          to search
      - in: query
        name: embed
        description: A flag to indicate whether to embed the corresponding feature
          into each matching name
      - in: query
        name: featureCategory
        description: A filter to limit the search to names associated with features
          of a certain category  The value of this parameter should be a featureCategoryCode
          value returned by the /featureCategories resource, or an asterisk (*) to
          request that all feature categories be included
      - in: query
        name: featureClass
        description: A filter to limit the search to names associated with features
          of a certain class  The value of this parameter should be a featureClassCode
          value returned by the /featureClasses resource, or an asterisk (*) to request
          that all feature classes be included
      - in: query
        name: featureType
        description: A filter to limit the search to names associated with features
          of a certain type  The value of this parameter should be a featureTypeCode
          value returned by the /featureTypes resource, or an asterisk (*) to request
          that all feature types be included
      - in: query
        name: itemsPerPage
        description: The number of search results to return (1-200)
      - in: query
        name: outputFormat
        description: The format of the output
      - in: query
        name: outputSRS
        description: The EPSG code of the spatial reference system (SRS) to use for
          output geometries
      - in: query
        name: outputStyle
        description: A flag indicating whether to include with each matching name
          a succinct list of attributes (summary), or a comprehensive list of attributes
          (detail)
      - in: query
        name: sortBy
        description: The distance to move the accessPoint away from the curb and towards
          the inside of the parcel (in metres)
      - in: query
        name: startIndex
        description: The index of the first record to be returned (>= 1)
      responses:
        200:
          description: OK
      tags:
      - Names
      - Decisions
      - Recent