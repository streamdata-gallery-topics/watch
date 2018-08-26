---
swagger: "2.0"
x-collection-name: IBM Financial Crimes Insight for Insurance
x-complete: 0
info:
  title: IBM Financial Crimes Insight for Insurance API Retrieve the contents of a
    watchlist, based on its id
  description: This method is used to retrieve the contents of a watchlist from the
    database
  version: 1.0.0
host: fcihost.ibm.com:9443
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /ibm/fci/platform/fact/watchlist:
    get:
      summary: Retrieve a list of the registered watchlists
      description: This method is used to retrieve the list of registered watchlists
        from the database
      operationId: getWatchlists
      x-api-path-slug: ibmfciplatformfactwatchlist-get
      parameters:
      - in: header
        name: IBM-FCI-Role
        description: Userid / password for user with appropriate role
      - in: header
        name: IBM-FCI-Token
        description: Security token obtained for execution
      responses:
        200:
          description: OK
      tags:
      - Retrieve
      - List
      - Of
      - Registered
      - Watchlists
    post:
      summary: Persist the provided watchlist into the local database
      description: 'This method is used to persist the contents of a watchlist into
        the database.  Note: This method uses some data import functionality to create
        business object entries, then calls putWatchlist to create/update a watchlist
        for the provided identifier, and finally calls putWatchlistItem for every
        object created. This one also has the caveat of needing a disposition defined,
        but in this case all you need to pass in is the stereotype value.'
      operationId: uploadWatchlist
      x-api-path-slug: ibmfciplatformfactwatchlist-post
      parameters:
      - in: formData
        name: data
        description: CSV file containing an external watchlist
      - in: formData
        name: dataName
        description: CSV file name
      - in: query
        name: disposition
        description: watchlist_disposition stereotype
      - in: header
        name: IBM-FCI-Role
        description: Userid / password for user with appropriate role
      - in: header
        name: IBM-FCI-Token
        description: Security token obtained for execution
      - in: query
        name: identifier
      - in: query
        name: overwrite
      - in: formData
        name: properties
        description: 'A '
      - in: formData
        name: propertiesName
        description: Properties file name
      responses:
        200:
          description: OK
      tags:
      - Persist
      - Provided
      - Watchlist
      - Into
      - Local
      - Database
  /ibm/fci/platform/fact/watchlist/{id}:
    get:
      summary: Retrieve the contents of a watchlist, based on its id
      description: This method is used to retrieve the contents of a watchlist from
        the database
      operationId: getWatchlistById
      x-api-path-slug: ibmfciplatformfactwatchlistid-get
      parameters:
      - in: header
        name: IBM-FCI-Role
        description: Userid / password for user with appropriate role
      - in: header
        name: IBM-FCI-Token
        description: Security token obtained for execution
      - in: path
        name: id
      - in: query
        name: summary
        description: If set to true, this flag will cause inclusion any Watchlist_Item_Properties
          associated with the item
      responses:
        200:
          description: OK
      tags:
      - Retrieve
      - Contents
      - Of
      - Watchlist
      - ""
      - Based
      - "On"
      - Its
      - Id
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