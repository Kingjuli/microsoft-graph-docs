---
description: "Automatically generated file. DO NOT MODIFY"
---

```bash

mgc device-app-management targeted-managed-app-configurations patch --targeted-managed-app-configuration-id {targetedManagedAppConfiguration-id} --body '{\
  "@odata.type": "#microsoft.graph.targetedManagedAppConfiguration",\
  "displayName": "Display Name value",\
  "description": "Description value",\
  "version": "Version value",\
  "customSettings": [\
    {\
      "@odata.type": "microsoft.graph.keyValuePair",\
      "name": "Name value",\
      "value": "Value value"\
    }\
  ],\
  "deployedAppCount": 0,\
  "isAssigned": true\
}\
'

```