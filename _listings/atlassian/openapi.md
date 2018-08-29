swagger: "2.0"
x-collection-name: Atlassian
x-complete: 1
info:
  title: Stride API
  description: this-service-provides-public-api-for-the-stride-
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
  /api/2/issue/{issueIdOrKey}/watchers:
    post:
      summary: Add watcher
      description: Adds the user to the issue's watcher list.
      operationId: com.atlassian.jira.rest.v2.issue.IssueResource.addWatcher_post
      x-api-path-slug: api2issueissueidorkeywatchers-post
      parameters:
      - in: header
        name: force-account-id
      - in: path
        name: issueIdOrKey
        description: ID or key of the issue to be updated
      responses:
        200:
          description: OK
      tags:
      - Watcher
    delete:
      summary: Remove watcher
      description: Removes the user from the issue's watcher list.
      operationId: com.atlassian.jira.rest.v2.issue.IssueResource.removeWatcher_delete
      x-api-path-slug: api2issueissueidorkeywatchers-delete
      parameters:
      - in: query
        name: accountId
        description: Account ID of the user to be removed from the watcher list
      - in: header
        name: force-account-id
      - in: path
        name: issueIdOrKey
        description: ID or key of the issue to be updated
      - in: query
        name: username
        description: Name of the user to be removed from the watcher list
      responses:
        200:
          description: OK
      tags:
      - Remove
      - Watcher
    get:
      summary: Get issue watchers
      description: Returns the list of watchers for the issue with the given key.
      operationId: com.atlassian.jira.rest.v2.issue.IssueResource.getIssueWatchers_get
      x-api-path-slug: api2issueissueidorkeywatchers-get
      parameters:
      - in: path
        name: issueIdOrKey
        description: ID or key of the issue to retrieve watchers for
      responses:
        200:
          description: OK
      tags:
      - Issue
      - Watchers
  /api/2/notificationscheme:
    get:
      summary: Get notification schemes paginated
      description: |-
        Returns a [paginated](https://developer.atlassian.com/cloud/jira/platform/rest/#pagination) list of [notification schemes](https://confluence.atlassian.com/x/8YdKLg) in order by display name.

        ### About notification schemes

        A notification scheme is a list of events and recipients who will receive notifications for those events. The list is contained within the `notificationSchemeEvents` object and contains pairs of `events` and `notifications`:

        *   `event` Identifies the type of event. The events can be [Jira system events](https://confluence.atlassian.com/x/8YdKLg#Creatinganotificationscheme-eventsEvents) or [custom events](https://confluence.atlassian.com/x/AIlKLg).
        *   `notifications` Identifies the [recipients](https://confluence.atlassian.com/x/8YdKLg#Creatinganotificationscheme-recipientsRecipients) of notifications for each event. Recipients can be any of the following types:

        *   `CurrentAssignee`
        *   `Reporter`
        *   `CurrentUser`
        *   `ProjectLead`
        *   `ComponentLead`
        *   `User` (the `parameter` is the user key)
        *   `Group` (the `parameter` is the group name)
        *   `ProjectRole` (the `parameter` is the project role ID)
        *   `EmailAddress`
        *   `AllWatchers`
        *   `UserCustomField` (the `parameter` is the ID of the custom field)
        *   `GroupCustomField`(the `parameter` is the ID of the custom field)

        _Note that you should allow for events without recipients to appear in responses._

        **[Permissions](https://confluence.atlassian.com/x/FQiiLQ) required:** None, however the requesting user must have permission to administer at least one project associated with a notification scheme for it to be returned.
      operationId: com.atlassian.jira.rest.v2.notification.NotificationSchemeResource.getNotificationSchemes_get
      x-api-path-slug: api2notificationscheme-get
      parameters:
      - in: query
        name: expand
        description: Use [expand](https://developer
      - in: query
        name: maxResults
        description: The maximum number of items to return per page
      - in: query
        name: startAt
        description: The index of the first item to return in a page of results (page
          offset)
      responses:
        200:
          description: OK
      tags:
      - Notification
      - Schemes
      - Paginated