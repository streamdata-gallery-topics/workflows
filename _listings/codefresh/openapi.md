swagger: "2.0"
x-collection-name: Codefresh
x-complete: 1
info:
  title: Codefresh API
  description: codefresh-api-swagger2-0-specification
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
  /workflow:
    get:
      summary: Get Workflow
      description: Get workflow.
      operationId: getWorkflow
      x-api-path-slug: workflow-get
      parameters:
      - in: query
        name: query
        description: Fields to search by
      responses:
        200:
          description: OK
      tags:
      - Workflow