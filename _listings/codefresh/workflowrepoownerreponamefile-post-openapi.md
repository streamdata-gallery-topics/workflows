---
swagger: "2.0"
x-collection-name: Codefresh
x-complete: 0
info:
  title: Codefresh Post Workflow Repoowner Reponame File
  description: Post workflow repoowner reponame file.
  termsOfService: http://www.codefresh.io
  contact:
    name: Codefresh api team
    url: http://www.codefresh.io
  version: 1.0.0
host: g.codefresh.io
basePath: /api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /workflow/{repoOwner}/{repoName}/file:
    post:
      summary: Post Workflow Repoowner Reponame File
      description: Post workflow repoowner reponame file.
      operationId: postWorkflowRepoownerReponameFile
      x-api-path-slug: workflowrepoownerreponamefile-post
      parameters:
      - in: body
        name: options
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: repoName
        description: The name of the repo
      - in: path
        name: repoOwner
        description: The name of the repo owner
      responses:
        200:
          description: OK
      tags:
      - Workflow
      - Repoowner
      - Reponame
      - File
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