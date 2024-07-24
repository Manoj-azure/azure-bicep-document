# azure-bicep-document
Azure Bicep is a domain-specific language (also known as DSL) designed by Microsoft for defining and deploying Azure resources in a declarative manner. It's the next generation of Azure Resource Manager (ARM) templates, offering a cleaner syntax, improved type safety, and better support for modularization. While ARM templates use JSON syntax, Bicep uses a more concise syntax that aims to make it easier for developers to author and maintain Azure deployments.

Although Azure’s Resource Manager still operates based on the JSON format, and your Azure Bicep templates will be converted to Json format when you submit them, it is clear that Azure Bicep templates are more readable and easier to maintain for developers than Json-based Azure Resource Manager (ARM) templates.

![image](https://github.com/user-attachments/assets/9f7eac5d-c37d-49e5-833c-4331d93ab2f3)

<details>
  <summary>
    <span><b>Basics</b></span>
    <p><i>Declarations of new and existing resources, variables, parameters and outputs, etcetera.</i></p>
  </summary>

### Create a resource

```bicep
resource resourceName 'ResourceType@version' = {
  name: 'exampleResourceName'
  properties: {
    // resource properties here
  }
}
```
