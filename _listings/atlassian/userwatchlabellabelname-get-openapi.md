---
swagger: "2.0"
x-collection-name: Atlassian
x-complete: 0
info:
  title: Confluence Cloud API Get label watch status
  description: "Returns whether a user is watching a label. Choose the user by doing
    one \nof the following:\n\n- Specify a user via a query parameter: Use the `username`,
    `key`, or `accountId` \nto identify the user. The user making the request must
    be a Confluence administrator.\n- Do not specify a user: The currently logged-in
    user will be used.\n\n**[Permissions](https://confluence.atlassian.com/x/_AozKw)
    required**: \n'Confluence Administrator' global permission if specifying a user,
    otherwise \npermission to access the Confluence site ('Can use' global permission)."
  termsOfService: http://atlassian.com/terms/
  version: 1.0.0
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /user/watch/content/{contentId}:
    get:
      summary: Get content watch status
      description: "Returns whether a user is watching a piece of content. Choose
        the user by \ndoing one of the following:\n\n- Specify a user via a query
        parameter: Use the `username`, `key`, or `accountId` \nto identify the user.
        The user making the request must be a Confluence administrator.\n- Do not
        specify a user: The currently logged-in user will be used.\n\n**[Permissions](https://confluence.atlassian.com/x/_AozKw)
        required**: \n'Confluence Administrator' global permission if specifying a
        user, otherwise \npermission to access the Confluence site ('Can use' global
        permission)."
      operationId: com.atlassian.confluence.plugins.restapi.resources.UserWatchResource.getContentWatchStatus_get
      x-api-path-slug: userwatchcontentcontentid-get
      parameters:
      - in: query
        name: accountId
        description: The `accountId` of the user to be queried for whether they are
          watching the content
      - in: path
        name: contentId
        description: The ID of the content to be queried for whether the specified
          user is watching it
      - in: query
        name: key
        description: The `key` of the user to be queried for whether they are watching
          the content
      - in: query
        name: username
        description: The `username` of the user to be queried for whether they are
          watching the content
      responses:
        200:
          description: OK
      tags:
      - Content
      - Watch
      - Status
  /user/watch/label/{labelName}:
    get:
      summary: Get label watch status
      description: "Returns whether a user is watching a label. Choose the user by
        doing one \nof the following:\n\n- Specify a user via a query parameter: Use
        the `username`, `key`, or `accountId` \nto identify the user. The user making
        the request must be a Confluence administrator.\n- Do not specify a user:
        The currently logged-in user will be used.\n\n**[Permissions](https://confluence.atlassian.com/x/_AozKw)
        required**: \n'Confluence Administrator' global permission if specifying a
        user, otherwise \npermission to access the Confluence site ('Can use' global
        permission)."
      operationId: com.atlassian.confluence.plugins.restapi.resources.UserWatchResource.isWatchingLabel_get
      x-api-path-slug: userwatchlabellabelname-get
      parameters:
      - in: query
        name: accountId
        description: The `accountId` of the user to be queried for whether they are
          watching the label
      - in: query
        name: key
        description: The `key` of the user to be queried for whether they are watching
          the label
      - in: path
        name: labelName
        description: The name of the label to be queried for whether the specified
          user is watching it
      - in: query
        name: username
        description: The `username` of the user to be queried for whether they are
          watching the label
      responses:
        200:
          description: OK
      tags:
      - Label
      - Watch
      - Status
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