---
swagger: "2.0"
x-collection-name: Bitbucket
x-complete: 0
info:
  title: Bitbucket Update Snippets Username Encoded  Watch
  description: Used to start watching a specific snippet. Returns 204 (No Content).
  termsOfService: https://www.atlassian.com/legal/customer-agreement
  contact:
    name: Bitbucket Support
    url: https://support.atlassian.com/bitbucket
    email: support@bitbucket.org
  version: 1.0.0
host: api.bitbucket.org
basePath: /2.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /repositories/{username}/{repo_slug}/issues/{issue_id}/watch:
    delete:
      summary: Delete Repositories Username Repo Slug Issues Issue  Watch
      description: Delete repositories username repo slug issues issue  watch
      operationId: deleteRepositoriesUsernameRepoSlugIssuesIssueWatch
      x-api-path-slug: repositoriesusernamerepo-slugissuesissue-idwatch-delete
      parameters:
      - in: path
        name: issue_id
        description: The issues id
      responses:
        200:
          description: OK
      tags:
      - Repositories
      - Username
      - Repo
      - Slug
      - Issues
      - Issue
      - ""
      - Watch
    get:
      summary: Get Repositories Username Repo Slug Issues Issue  Watch
      description: |-
        Indicated whether or not the authenticated user is watching this
        issue.
      operationId: getRepositoriesUsernameRepoSlugIssuesIssueWatch
      x-api-path-slug: repositoriesusernamerepo-slugissuesissue-idwatch-get
      parameters:
      - in: path
        name: issue_id
        description: The issues id
      responses:
        200:
          description: OK
      tags:
      - Repositories
      - Username
      - Repo
      - Slug
      - Issues
      - Issue
      - ""
      - Watch
    parameters:
      summary: Parameters Repositories Username Repo Slug Issues Issue  Watch
      description: Parameters repositories username repo slug issues issue  watch
      operationId: parametersRepositoriesUsernameRepoSlugIssuesIssueWatch
      x-api-path-slug: repositoriesusernamerepo-slugissuesissue-idwatch-parameters
      responses:
        200:
          description: OK
      tags:
      - Repositories
      - Username
      - Repo
      - Slug
      - Issues
      - Issue
      - ""
      - Watch
    put:
      summary: Update Repositories Username Repo Slug Issues Issue  Watch
      description: |-
        Start watching this issue.

        To start watching this issue, do an empty PUT. The 204 status code
        indicates that the operation was successful.
      operationId: putRepositoriesUsernameRepoSlugIssuesIssueWatch
      x-api-path-slug: repositoriesusernamerepo-slugissuesissue-idwatch-put
      parameters:
      - in: path
        name: issue_id
        description: The issues id
      responses:
        200:
          description: OK
      tags:
      - Repositories
      - Username
      - Repo
      - Slug
      - Issues
      - Issue
      - ""
      - Watch
  /snippets/{username}/{encoded_id}/watch:
    delete:
      summary: Delete Snippets Username Encoded  Watch
      description: |-
        Used to stop watching a specific snippet. Returns 204 (No Content)
        to indicate success.
      operationId: deleteSnippetsUsernameEncodedWatch
      x-api-path-slug: snippetsusernameencoded-idwatch-delete
      parameters:
      - in: path
        name: encoded_id
        description: The snippet id
      responses:
        200:
          description: OK
      tags:
      - Snippets
      - Username
      - Encoded
      - ""
      - Watch
    get:
      summary: Get Snippets Username Encoded  Watch
      description: |-
        Used to check if the current user is watching a specific snippet.

        Returns 204 (No Content) if the user is watching the snippet and 404 if
        not.

        Hitting this endpoint anonymously always returns a 404.
      operationId: getSnippetsUsernameEncodedWatch
      x-api-path-slug: snippetsusernameencoded-idwatch-get
      parameters:
      - in: path
        name: encoded_id
        description: The snippet id
      responses:
        200:
          description: OK
      tags:
      - Snippets
      - Username
      - Encoded
      - ""
      - Watch
    parameters:
      summary: Parameters Snippets Username Encoded  Watch
      description: Parameters snippets username encoded  watch
      operationId: parametersSnippetsUsernameEncodedWatch
      x-api-path-slug: snippetsusernameencoded-idwatch-parameters
      responses:
        200:
          description: OK
      tags:
      - Snippets
      - Username
      - Encoded
      - ""
      - Watch
    put:
      summary: Update Snippets Username Encoded  Watch
      description: Used to start watching a specific snippet. Returns 204 (No Content).
      operationId: putSnippetsUsernameEncodedWatch
      x-api-path-slug: snippetsusernameencoded-idwatch-put
      parameters:
      - in: path
        name: encoded_id
        description: The snippet id
      responses:
        200:
          description: OK
      tags:
      - Snippets
      - Username
      - Encoded
      - ""
      - Watch
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