---
swagger: "2.0"
x-collection-name: Atlassian
x-complete: 0
info:
  title: Jira Cloud API Get draft workflow
  description: Returns the draft workflow mappings or requested mapping to the caller.
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
  /api/2/workflow/transitions/{transitionId}/properties:
    get:
      summary: Get workflow transition properties
      description: |-
        Returns the properties on a workflow transition. Transition properties are used to change the behavior of a transition. For more information, see [Transition properties](https://confluence.atlassian.com/x/zIhKLg#Advancedworkflowconfiguration-transitionproperties) and [Workflow properties](https://confluence.atlassian.com/x/JYlKLg).

        **[Permissions](https://confluence.atlassian.com/x/FQiiLQ) required:** _Administer Jira_ global permission.
      operationId: com.atlassian.jira.rest.v2.admin.WorkflowTransitionResource.getWorkflowTransitionProperties_get
      x-api-path-slug: api2workflowtransitionstransitionidproperties-get
      parameters:
      - in: query
        name: includeReservedKeys
        description: Some properties with keys that have the _jira
      - in: query
        name: key
        description: The key of the property being returned, also known as the name
          of the property
      - in: path
        name: transitionId
        description: The ID of the transition
      - in: query
        name: workflowMode
        description: The workflow status
      - in: query
        name: workflowName
        description: The name of the workflow that the transition belongs to
      responses:
        200:
          description: OK
      tags:
      - Workflow
      - Transition
      - Properties
    post:
      summary: Create workflow transition property
      description: |-
        Adds a property to a workflow transition. Transition properties are used to change the behavior of a transition. For more information, see [Transition properties](https://confluence.atlassian.com/x/zIhKLg#Advancedworkflowconfiguration-transitionproperties) and [Workflow properties](https://confluence.atlassian.com/x/JYlKLg).

        **[Permissions](https://confluence.atlassian.com/x/FQiiLQ) required:** _Administer Jira_ global permission.
      operationId: com.atlassian.jira.rest.v2.admin.WorkflowTransitionResource.createWorkflowTransitionProperty_post
      x-api-path-slug: api2workflowtransitionstransitionidproperties-post
      parameters:
      - in: query
        name: key
        description: The key of the property being added, also known as the name of
          the property
      - in: path
        name: transitionId
        description: The ID of the transition
      - in: query
        name: workflowMode
        description: The workflow status
      - in: query
        name: workflowName
        description: The name of the workflow that the transition belongs to
      responses:
        200:
          description: OK
      tags:
      - Workflow
      - Transition
      - Property
    put:
      summary: Update workflow transition property
      description: |-
        Updates a workflow transition by changing the property value. Trying to update a property that does not exist results in a new property being added to the transition. Transition properties are used to change the behavior of a transition. For more information, see [Transition properties](https://confluence.atlassian.com/x/zIhKLg#Advancedworkflowconfiguration-transitionproperties) and [Workflow properties](https://confluence.atlassian.com/x/JYlKLg).

        **[Permissions](https://confluence.atlassian.com/x/FQiiLQ) required:** _Administer Jira_ global permission.
      operationId: com.atlassian.jira.rest.v2.admin.WorkflowTransitionResource.updateWorkflowTransitionProperty_put
      x-api-path-slug: api2workflowtransitionstransitionidproperties-put
      parameters:
      - in: query
        name: key
        description: The key of the property being updated, also known as the name
          of the property
      - in: path
        name: transitionId
        description: The ID of the transition
      - in: query
        name: workflowMode
        description: The workflow status
      - in: query
        name: workflowName
        description: The name of the workflow that the transition belongs to
      responses:
        200:
          description: OK
      tags:
      - Workflow
      - Transition
      - Property
    delete:
      summary: Delete workflow transition property
      description: |-
        Deletes a property from a workflow transition. Transition properties are used to change the behavior of a transition. For more information, see [Transition properties](https://confluence.atlassian.com/x/zIhKLg#Advancedworkflowconfiguration-transitionproperties) and [Workflow properties](https://confluence.atlassian.com/x/JYlKLg).

        **[Permissions](https://confluence.atlassian.com/x/FQiiLQ) required:** _Administer Jira_ global permission.
      operationId: com.atlassian.jira.rest.v2.admin.WorkflowTransitionResource.deleteWorkflowTransitionProperty_delete
      x-api-path-slug: api2workflowtransitionstransitionidproperties-delete
      parameters:
      - in: query
        name: key
        description: The name of the transition property to delete, also known as
          the name of the property
      - in: path
        name: transitionId
        description: The ID of the transition
      - in: query
        name: workflowMode
        description: The workflow status
      - in: query
        name: workflowName
        description: The name of the workflow that the transition belongs to
      responses:
        200:
          description: OK
      tags:
      - Workflow
      - Transition
      - Property
  /api/2/workflowscheme:
    post:
      summary: Create workflow scheme
      description: |-
        Create a new workflow scheme.

        The body contains a representation of the new scheme. Values not passed are assumed to be set to their defaults.
      operationId: com.atlassian.jira.rest.v2.admin.workflowscheme.WorkflowSchemeResource.createWorkflowScheme_post
      x-api-path-slug: api2workflowscheme-post
      responses:
        200:
          description: OK
      tags:
      - Workflow
      - Scheme
  /api/2/workflowscheme/{id}:
    get:
      summary: Get workflow scheme
      description: Returns the requested workflow scheme to the caller.
      operationId: com.atlassian.jira.rest.v2.admin.workflowscheme.WorkflowSchemeResource.getWorkflowScheme_get
      x-api-path-slug: api2workflowschemeid-get
      parameters:
      - in: path
        name: id
        description: the id of the scheme
      - in: query
        name: returnDraftIfExists
        description: when true indicates that a schemes draft, if it exists, should
          be queried instead of the scheme itself
      responses:
        200:
          description: OK
      tags:
      - Workflow
      - Scheme
    put:
      summary: Update workflow scheme
      description: |-
        Update the passed workflow scheme.

        The body of the request is a representation of the workflow scheme. Values not passed are assumed to indicate no change for that field.

        The passed representation can have its updateDraftIfNeeded flag set to true to indicate that the draft should be created and/or updated when the actual scheme cannot be edited (e.g. when the scheme is being used by a project). Values not appearing the body will not be touched.
      operationId: com.atlassian.jira.rest.v2.admin.workflowscheme.WorkflowSchemeResource.updateWorkflowScheme_put
      x-api-path-slug: api2workflowschemeid-put
      parameters:
      - in: path
        name: id
        description: the id of the scheme
      responses:
        200:
          description: OK
      tags:
      - Workflow
      - Scheme
    delete:
      summary: Delete workflow scheme
      description: Delete the passed workflow scheme.
      operationId: com.atlassian.jira.rest.v2.admin.workflowscheme.WorkflowSchemeResource.deleteWorkflowScheme_delete
      x-api-path-slug: api2workflowschemeid-delete
      parameters:
      - in: path
        name: id
        description: the id of the scheme
      responses:
        200:
          description: OK
      tags:
      - Workflow
      - Scheme
  /api/2/workflowscheme/{id}/createdraft:
    post:
      summary: Create workflow scheme draft from parent
      description: Create a draft for the passed scheme. The draft will be a copy
        of the state of the parent.
      operationId: com.atlassian.jira.rest.v2.admin.workflowscheme.WorkflowSchemeResource.createWorkflowSchemeDraftFrom
      x-api-path-slug: api2workflowschemeidcreatedraft-post
      parameters:
      - in: path
        name: id
        description: the id of the parent scheme
      responses:
        200:
          description: OK
      tags:
      - Workflow
      - Scheme
      - Draft
      - From
      - Parent
  /api/2/workflowscheme/{id}/default:
    get:
      summary: Get default workflow
      description: Return the default workflow from the passed workflow scheme.
      operationId: com.atlassian.jira.rest.v2.admin.workflowscheme.WorkflowSchemeResource.getDefaultWorkflow_get
      x-api-path-slug: api2workflowschemeiddefault-get
      parameters:
      - in: path
        name: id
        description: the id of the scheme
      - in: query
        name: returnDraftIfExists
        description: when true indicates that a schemes draft, if it exists, should
          be queried instead of the scheme itself
      responses:
        200:
          description: OK
      tags:
      - Default
      - Workflow
    put:
      summary: Update default workflow
      description: |-
        Set the default workflow for the passed workflow scheme.

        The passed representation can have its updateDraftIfNeeded flag set to true to indicate that the draft should be created/updated when the actual scheme cannot be edited.
      operationId: com.atlassian.jira.rest.v2.admin.workflowscheme.WorkflowSchemeResource.updateDefaultWorkflow_put
      x-api-path-slug: api2workflowschemeiddefault-put
      parameters:
      - in: path
        name: id
        description: the id of the scheme
      responses:
        200:
          description: OK
      tags:
      - Default
      - Workflow
    delete:
      summary: Delete default workflow
      description: Remove the default workflow from the passed workflow scheme.
      operationId: com.atlassian.jira.rest.v2.admin.workflowscheme.WorkflowSchemeResource.deleteDefaultWorkflow_delete
      x-api-path-slug: api2workflowschemeiddefault-delete
      parameters:
      - in: path
        name: id
        description: the id of the scheme
      - in: query
        name: updateDraftIfNeeded
        description: when true will create and return a draft when the workflow scheme
          cannot be edited (e
      responses:
        200:
          description: OK
      tags:
      - Default
      - Workflow
  /api/2/workflowscheme/{id}/draft:
    get:
      summary: Get workflow scheme draft
      description: Returns the requested draft workflow scheme to the caller.
      operationId: com.atlassian.jira.rest.v2.admin.workflowscheme.WorkflowSchemeResource.getWorkflowSchemeDraft_get
      x-api-path-slug: api2workflowschemeiddraft-get
      parameters:
      - in: path
        name: id
        description: the id of the parent scheme
      responses:
        200:
          description: OK
      tags:
      - Workflow
      - Scheme
      - Draft
    put:
      summary: Update workflow scheme draft
      description: |-
        Update a draft workflow scheme. The draft will created if necessary.

        The body is a representation of the workflow scheme. Values not passed are assumed to indicate no change for that field.
      operationId: com.atlassian.jira.rest.v2.admin.workflowscheme.WorkflowSchemeResource.updateWorkflowSchemeDraft_put
      x-api-path-slug: api2workflowschemeiddraft-put
      parameters:
      - in: path
        name: id
        description: the id of the parent scheme
      responses:
        200:
          description: OK
      tags:
      - Workflow
      - Scheme
      - Draft
    delete:
      summary: Delete workflow scheme draft
      description: Delete the passed draft workflow scheme.
      operationId: com.atlassian.jira.rest.v2.admin.workflowscheme.WorkflowSchemeResource.deleteWorkflowSchemeDraft_del
      x-api-path-slug: api2workflowschemeiddraft-delete
      parameters:
      - in: path
        name: id
        description: the id of the parent scheme
      responses:
        200:
          description: OK
      tags:
      - Workflow
      - Scheme
      - Draft
  /api/2/workflowscheme/{id}/draft/default:
    get:
      summary: Get draft default workflow
      description: Return the default workflow from the passed draft workflow scheme
        to the caller.
      operationId: com.atlassian.jira.rest.v2.admin.workflowscheme.WorkflowSchemeResource.getDraftDefaultWorkflow_get
      x-api-path-slug: api2workflowschemeiddraftdefault-get
      parameters:
      - in: path
        name: id
        description: the id of the parent scheme
      responses:
        200:
          description: OK
      tags:
      - Draft
      - Default
      - Workflow
    put:
      summary: Update draft default workflow
      description: Set the default workflow for the passed draft workflow scheme.
      operationId: com.atlassian.jira.rest.v2.admin.workflowscheme.WorkflowSchemeResource.updateDraftDefaultWorkflow_pu
      x-api-path-slug: api2workflowschemeiddraftdefault-put
      parameters:
      - in: path
        name: id
        description: the id of the parent scheme
      responses:
        200:
          description: OK
      tags:
      - Draft
      - Default
      - Workflow
    delete:
      summary: Delete draft default workflow
      description: Remove the default workflow from the passed draft workflow scheme.
      operationId: com.atlassian.jira.rest.v2.admin.workflowscheme.WorkflowSchemeResource.deleteDraftDefaultWorkflow_de
      x-api-path-slug: api2workflowschemeiddraftdefault-delete
      parameters:
      - in: path
        name: id
        description: the id of the parent scheme
      responses:
        200:
          description: OK
      tags:
      - Draft
      - Default
      - Workflow
  /api/2/workflowscheme/{id}/draft/issuetype/{issueType}:
    get:
      summary: Get workflow scheme draft issue type
      description: Returns the issue type mapping for the passed draft workflow scheme.
      operationId: com.atlassian.jira.rest.v2.admin.workflowscheme.WorkflowSchemeResource.getWorkflowSchemeDraftIssueTy
      x-api-path-slug: api2workflowschemeiddraftissuetypeissuetype-get
      parameters:
      - in: path
        name: id
        description: the id of the parent scheme
      - in: path
        name: issueType
        description: the issue type to query
      responses:
        200:
          description: OK
      tags:
      - Workflow
      - Scheme
      - Draft
      - Issue
      - Type
    put:
      summary: Set workflow scheme draft issue type
      description: |-
        Set the issue type mapping for the passed draft scheme.

        The passed representation can have its updateDraftIfNeeded flag set to true to indicate that the draft should be created/updated when the actual scheme cannot be edited.
      operationId: com.atlassian.jira.rest.v2.admin.workflowscheme.WorkflowSchemeResource.setWorkflowSchemeDraftIssueTy
      x-api-path-slug: api2workflowschemeiddraftissuetypeissuetype-put
      parameters:
      - in: path
        name: id
        description: the id of the parent scheme
      - in: path
        name: issueType
        description: the issue type being set
      responses:
        200:
          description: OK
      tags:
      - Set
      - Workflow
      - Scheme
      - Draft
      - Issue
      - Type
    delete:
      summary: Delete workflow scheme draft issue type
      description: Remove the specified issue type mapping from the draft scheme.
      operationId: com.atlassian.jira.rest.v2.admin.workflowscheme.WorkflowSchemeResource.deleteWorkflowSchemeDraftIssu
      x-api-path-slug: api2workflowschemeiddraftissuetypeissuetype-delete
      parameters:
      - in: path
        name: id
        description: the parent of the draft scheme
      - in: path
        name: issueType
        description: the issue type to remove
      responses:
        200:
          description: OK
      tags:
      - Workflow
      - Scheme
      - Draft
      - Issue
      - Type
  /api/2/workflowscheme/{id}/draft/workflow:
    get:
      summary: Get draft workflow
      description: Returns the draft workflow mappings or requested mapping to the
        caller.
      operationId: com.atlassian.jira.rest.v2.admin.workflowscheme.WorkflowSchemeResource.getDraftWorkflow_get
      x-api-path-slug: api2workflowschemeiddraftworkflow-get
      parameters:
      - in: path
        name: id
        description: the id of the parent scheme
      - in: query
        name: workflowName
        description: the workflow mapping to return
      responses:
        200:
          description: OK
      tags:
      - Draft
      - Workflow
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