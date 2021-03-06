---
title: "IDebugMethodField::GetGlobalContainer | Microsoft Docs"
ms.custom: ""
ms.date: "2018-06-30"
ms.prod: "visual-studio-dev14"
ms.reviewer: ""
ms.suite: ""
ms.technology: 
  - "vs-ide-sdk"
ms.tgt_pltfrm: ""
ms.topic: "article"
f1_keywords: 
  - "IDebugMethodField::GetGlobalContainer"
helpviewer_keywords: 
  - "IDebugMethodField::GetGlobalContainer method"
ms.assetid: 041ac5aa-0b80-4310-b9ae-b88f8e7e0e5f
caps.latest.revision: 10
ms.author: "gregvanl"
manager: "ghogen"
---
# IDebugMethodField::GetGlobalContainer
[!INCLUDE[vs2017banner](../../../includes/vs2017banner.md)]

The latest version of this topic can be found at [IDebugMethodField::GetGlobalContainer](https://docs.microsoft.com/visualstudio/extensibility/debugger/reference/idebugmethodfield-getglobalcontainer).  
  
Gets the global container of the method.  
  
## Syntax  
  
```cpp#  
HRESULT GetGlobalContainer(  
   IDebugClassField** ppClass  
);  
```  
  
```csharp  
int GetGlobalContainer(  
   out IDebugClassField ppClass  
);  
```  
  
#### Parameters  
 `ppClass`  
 [out] Returns an [IDebugClassField](../../../extensibility/debugger/reference/idebugclassfield.md) representing the module in which this method is defined.  
  
## Return Value  
 If successful, returns S_OK; otherwise, returns an error code.  
  
## Remarks  
 The returned [IDebugClassField](../../../extensibility/debugger/reference/idebugclassfield.md) object represents the entire module and is an artificial object, that is, the module itself does not have an actual class but it can be represented by an `IDebugClassField` object, allowing the various elements of the module to be enumerated and discovered.  
  
## See Also  
 [IDebugMethodField](../../../extensibility/debugger/reference/idebugmethodfield.md)   
 [IDebugClassField](../../../extensibility/debugger/reference/idebugclassfield.md)

