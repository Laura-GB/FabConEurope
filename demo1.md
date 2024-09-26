# Demo 1 - Create file in OneLake from legacy system with no apis

## Power Automate Desktop

Show web page - text filter North that data into Fabric

Mini record then here is one I made earlier to put a file in SharePoint.

## File in SharePoint to OneLake

* Trigger for new file in SharePoint

* Steps to get the file content

* Lakehouse - Files - click on three dots and select properties.
* Copy url path

* In compose add the filename to the path

```
https://onelake.dfs.fabric.microsoft.com/2e4ed64c-ff7f-4ab7-b990-1057a12bc8d6/dd6161ec-f076-4e6b-81de-4a9c75433e31/Files
```
## Create blank file

Add preauthorised http call 

* Action = PUT 
* URL = Compose & ?resource=file

![Creating a blank file using a http step](<Images/demo 1 blank file.png>)

## Append file content

Add preauthorised http call 

* Action = PATCH 
* URL = Compose & ?action=append&position=0&flush=true
* Body = File content from previous step

![Append file content](<Images/demo 1 append file content and finalise.png>)

## Back to Front
[Link back to Readme.md](README.md)
