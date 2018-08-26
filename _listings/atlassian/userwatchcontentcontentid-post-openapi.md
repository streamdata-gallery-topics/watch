---
swagger: "2.0"
x-collection-name: Atlassian
x-complete: 0
info:
  title: Confluence Cloud API Add content watcher
  description: "Adds a user as a watcher to a piece of content. Choose the user by
    doing \none of the following:\n\n- Specify a user via a query parameter: Use the
    `username`, `key`, or `accountId` \nto identify the user. The user making the
    request must be a Confluence administrator.\n- Do not specify a user: The currently
    logged-in user will be used.\n\nNote, you must add the `X-Atlassian-Token: no-check`
    header when making a \nrequest, as this operation has XSRF protection.\n\n**[Permissions](https://confluence.atlassian.com/x/_AozKw)
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
    post:
      summary: Add content watcher
      description: "Adds a user as a watcher to a piece of content. Choose the user
        by doing \none of the following:\n\n- Specify a user via a query parameter:
        Use the `username`, `key`, or `accountId` \nto identify the user. The user
        making the request must be a Confluence administrator.\n- Do not specify a
        user: The currently logged-in user will be used.\n\nNote, you must add the
        `X-Atlassian-Token: no-check` header when making a \nrequest, as this operation
        has XSRF protection.\n\n**[Permissions](https://confluence.atlassian.com/x/_AozKw)
        required**: \n'Confluence Administrator' global permission if specifying a
        user, otherwise \npermission to access the Confluence site ('Can use' global
        permission)."
      operationId: com.atlassian.confluence.plugins.restapi.resources.UserWatchResource.addContentWatcher_post
      x-api-path-slug: userwatchcontentcontentid-post
      parameters:
      - in: query
        name: accountId
        description: The `accountId` of the user that will be added as a watcher
      - in: path
        name: contentId
        description: The ID of the content to add the watcher to
      - in: query
        name: key
        description: The `key` of the user that will be added as a watcher
      - in: query
        name: username
        description: The `username` of the user that will be added as a watcher
      responses:
        200:
          description: OK
      tags:
      - Content
      - Watcher
    delete:
      summary: Remove content watcher
      description: "Removes a user as a watcher from a piece of content. Choose the
        user by \ndoing one of the following:\n\n- Specify a user via a query parameter:
        Use the `username`, `key`, or `accountId` \nto identify the user. The user
        making the request must be a Confluence administrator.\n- Do not specify a
        user: The currently logged-in user will be used.\n\n**[Permissions](https://confluence.atlassian.com/x/_AozKw)
        required**: \n'Confluence Administrator' global permission if specifying a
        user, otherwise \npermission to access the Confluence site ('Can use' global
        permission)."
      operationId: com.atlassian.confluence.plugins.restapi.resources.UserWatchResource.removeContentWatcher_delete
      x-api-path-slug: userwatchcontentcontentid-delete
      parameters:
      - in: query
        name: accountId
        description: The `accountId` of the user that will be removed as a watcher
      - in: path
        name: contentId
        description: The ID of the content to remove the watcher from
      - in: query
        name: key
        description: The `key` of the user that will be removed as a watcher
      - in: query
        name: username
        description: The `username` of the user that will be removed as a watcher
      responses:
        200:
          description: OK
      tags:
      - Remove
      - Content
      - Watcher
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
    post:
      summary: Add label watcher
      description: "Adds a user as a watcher to a label. Choose the user by doing
        one of the \nfollowing:\n\n- Specify a user via a query parameter: Use the
        `username`, `key`, or `accountId` \nto identify the user. The user making
        the request must be a Confluence administrator.\n- Do not specify a user:
        The currently logged-in user will be used.\n\nNote, you must add the `X-Atlassian-Token:
        no-check` header when making a \nrequest, as this operation has XSRF protection.\n\n**[Permissions](https://confluence.atlassian.com/x/_AozKw)
        required**: \n'Confluence Administrator' global permission if specifying a
        user, otherwise \npermission to access the Confluence site ('Can use' global
        permission)."
      operationId: com.atlassian.confluence.plugins.restapi.resources.UserWatchResource.addLabelWatcher_post
      x-api-path-slug: userwatchlabellabelname-post
      parameters:
      - in: query
        name: accountId
        description: The `accountId` of the user that will be added as a watcher
      - in: query
        name: key
        description: The `key` of the user that will be added as a watcher
      - in: path
        name: labelName
        description: The name of the label to add the watcher to
      - in: query
        name: username
        description: The `username` of the user that will be added as a watcher
      responses:
        200:
          description: OK
      tags:
      - Label
      - Watcher
    delete:
      summary: Remove label watcher
      description: "Removes a user as a watcher from a label. Choose the user by doing
        one of \nthe following:\n\n- Specify a user via a query parameter: Use the
        `username`, `key`, or `accountId` \nto identify the user. The user making
        the request must be a Confluence administrator.\n- Do not specify a user:
        The currently logged-in user will be used.\n\n**[Permissions](https://confluence.atlassian.com/x/_AozKw)
        required**: \n'Confluence Administrator' global permission if specifying a
        user, otherwise \npermission to access the Confluence site ('Can use' global
        permission)."
      operationId: com.atlassian.confluence.plugins.restapi.resources.UserWatchResource.removeLabelWatcher_delete
      x-api-path-slug: userwatchlabellabelname-delete
      parameters:
      - in: query
        name: accountId
        description: The `accountId` of the user that will be removed as a watcher
      - in: query
        name: key
        description: The `key` of the user that will be removed as a watcher
      - in: path
        name: labelName
        description: The name of the label to remove the watcher from
      - in: query
        name: username
        description: The `username` of the user that will be removed as a watcher
      responses:
        200:
          description: OK
      tags:
      - Remove
      - Label
      - Watcher
  /user/watch/space/{spaceKey}:
    get:
      summary: Get space watch status
      description: "Returns whether a user is watching a space. Choose the user by
        \ndoing one of the following:\n\n- Specify a user via a query parameter: Use
        the `username`, `key`, or `accountId` \nto identify the user. The user making
        the request must be a Confluence administrator.\n- Do not specify a user:
        The currently logged-in user will be used.\n\n**[Permissions](https://confluence.atlassian.com/x/_AozKw)
        required**: \n'Confluence Administrator' global permission if specifying a
        user, otherwise \npermission to access the Confluence site ('Can use' global
        permission)."
      operationId: com.atlassian.confluence.plugins.restapi.resources.UserWatchResource.isWatchingSpace_get
      x-api-path-slug: userwatchspacespacekey-get
      parameters:
      - in: query
        name: accountId
        description: The `accountId` of the user to be queried for whether they are
          watching the space
      - in: query
        name: key
        description: The `key` of the user to be queried for whether they are watching
          the space
      - in: path
        name: spaceKey
        description: The key of the space to be queried for whether the specified
          user is watching it
      - in: query
        name: username
        description: The `username` of the user to be queried for whether they are
          watching the space
      responses:
        200:
          description: OK
      tags:
      - Space
      - Watch
      - Status
    delete:
      summary: Remove space watch
      description: "Removes a user as a watcher from a space. Choose the user by doing
        one of \nthe following:\n\n- Specify a user via a query parameter: Use the
        `username`, `key`, or `accountId` \nto identify the user. The user making
        the request must be a Confluence administrator.\n- Do not specify a user:
        The currently logged-in user will be used.\n\n**[Permissions](https://confluence.atlassian.com/x/_AozKw)
        required**: \n'Confluence Administrator' global permission if specifying a
        user, otherwise \npermission to access the Confluence site ('Can use' global
        permission)."
      operationId: com.atlassian.confluence.plugins.restapi.resources.UserWatchResource.removeSpaceWatch_delete
      x-api-path-slug: userwatchspacespacekey-delete
      parameters:
      - in: query
        name: accountId
        description: The `accountId` of the user that will be removed as a watcher
      - in: query
        name: key
        description: The `key` of the user that will be removed as a watcher
      - in: path
        name: spaceKey
        description: The key of the space to remove the watcher from
      - in: query
        name: username
        description: The `username` of the user that will be removed as a watcher
      responses:
        200:
          description: OK
      tags:
      - Remove
      - Space
      - Watch
    post:
      summary: Add space watcher
      description: "Adds a user as a watcher to a space. Choose the user by doing
        one of the \nfollowing:\n\n- Specify a user via a query parameter: Use the
        `username`, `key`, or `accountId` \nto identify the user. The user making
        the request must be a Confluence administrator.\n- Do not specify a user:
        The currently logged-in user will be used.\n\nNote, you must add the `X-Atlassian-Token:
        no-check` header when making a \nrequest, as this operation has XSRF protection.\n\n**[Permissions](https://confluence.atlassian.com/x/_AozKw)
        required**: \n'Confluence Administrator' global permission if specifying a
        user, otherwise \npermission to access the Confluence site ('Can use' global
        permission)."
      operationId: com.atlassian.confluence.plugins.restapi.resources.UserWatchResource.addSpaceWatcher_post
      x-api-path-slug: userwatchspacespacekey-post
      parameters:
      - in: query
        name: accountId
        description: The `accountId` of the user that will be added as a watcher
      - in: query
        name: key
        description: The `key` of the user that will be added as a watcher
      - in: path
        name: spaceKey
        description: The key of the space to add the watcher to
      - in: query
        name: username
        description: The `username` of the user that will be added as a watcher
      responses:
        200:
          description: OK
      tags:
      - Space
      - Watcher
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