# Demo 2 - Trigger Pipeline

## Trigger - manual for now

Manual trigger - could be triggered by an app etc

## Pipeline details

Initialise Variables with values from pipeline

Workspace ID

Pipeline ID

Then combine into a string using a compose

```
https://api.fabric.microsoft.com/v1/workspaces/@{variables('WorkspaceID')}/items/@{variables('PipelineID')}/jobs/instances?jobType=Pipeline
```

## HTTP Call

* Method - POST
* URL - Compose output


## Back to Front
[Link back to Readme.md](README.md)