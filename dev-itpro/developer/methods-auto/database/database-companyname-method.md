---
title: "Database.CompanyName() Method"
description: "Gets the current company name."
ms.author: solsen
ms.date: 08/26/2024
ms.topic: reference
author: SusanneWindfeldPedersen
ms.reviewer: solsen
---
[//]: # (START>DO_NOT_EDIT)
[//]: # (IMPORTANT:Do not edit any of the content between here and the END>DO_NOT_EDIT.)
[//]: # (Any modifications should be made in the .xml files in the ModernDev repo.)
# Database.CompanyName() Method
> **Version**: _Available or changed with runtime version 1.0._

Gets the current company name.


## Syntax
```AL
Name :=   Database.CompanyName()
```
> [!NOTE]
> This method can be invoked using property access syntax.
> [!NOTE]
> This method can be invoked without specifying the data type name.

## Return Value
*Name*  
&emsp;Type: [Text](../text/text-data-type.md)  
The name of the company, or an empty string if no company has been selected.


[//]: # (IMPORTANT: END>DO_NOT_EDIT)

## Example

```al
var
    CompName: Text[1024];
    Text000: Label 'The name is %1.';
begin
    CompName := CompanyName();  
    Message(Text000, CompName);  
end;
```  

## Related information

[Database Data Type](database-data-type.md)  
[Get Started with AL](../../devenv-get-started.md)  
[Developing Extensions](../../devenv-dev-overview.md)
