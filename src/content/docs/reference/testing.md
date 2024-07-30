---
title: Software Testing
---

# About Unit Testing

please put some notes about what you have learned


# API Testing with Albo

```csharp
 
using Alba;
 
namespace HelpDesk.Tests.Software;
public class GettingSoftware
{
    // Test that we can make an HTTP GET requests to /api/software
 
    [Fact]
    public async Task CanGetSoftware()
    {
        var host = await AlbaHost.For<Program>();
 
        await host.Scenario(api =>
        {
            api.Get.Url("/api/software");
            api.StatusCodeShouldBeOk();
        });
 
 
    }
}
```
 
Write what you understand about this code. What is Alba? Where did that come from? What is `Program`?