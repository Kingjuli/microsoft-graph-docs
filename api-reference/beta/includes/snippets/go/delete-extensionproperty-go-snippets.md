---
description: "Automatically generated file. DO NOT MODIFY"
---

```go


import (
	  "context"
	  msgraphsdk "github.com/microsoftgraph/msgraph-beta-sdk-go"
	  //other-imports
)

graphClient := msgraphsdk.NewGraphServiceClientWithCredentials(cred, scopes)



graphClient.Applications().ByApplicationId("application-id").ExtensionProperties().ByExtensionPropertieId("extensionProperty-id").Delete(context.Background(), nil)


```