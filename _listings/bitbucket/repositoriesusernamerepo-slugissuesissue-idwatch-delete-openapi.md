---
swagger: "2.0"
x-collection-name: Bitbucket
x-complete: 0
info:
  title: Bitbucket Delete Repositories Username Repo Slug Issues Issue  Watch
  description: Delete repositories username repo slug issues issue  watch
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