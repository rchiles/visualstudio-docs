---
title: "IDebugDynamicFieldCOMPlus::GetTypeFromPrimitive | Microsoft Docs"
ms.custom: ""
ms.date: "2018-06-30"
ms.prod: "visual-studio-dev14"
ms.reviewer: ""
ms.suite: ""
ms.technology: 
  - "vs-ide-sdk"
ms.tgt_pltfrm: ""
ms.topic: "article"
helpviewer_keywords: 
  - "IDebugDynamicFieldCOMPlus::GetTypeFromPrimitive"
  - "GetTypeFromPrimitive"
ms.assetid: d7f51e2a-1b72-489c-b7b6-4af7b7e4d663
caps.latest.revision: 11
ms.author: "gregvanl"
manager: "ghogen"
---
# IDebugDynamicFieldCOMPlus::GetTypeFromPrimitive
[!INCLUDE[vs2017banner](../../../includes/vs2017banner.md)]

The latest version of this topic can be found at [IDebugDynamicFieldCOMPlus::GetTypeFromPrimitive](https://docs.microsoft.com/visualstudio/extensibility/debugger/reference/idebugdynamicfieldcomplus-gettypefromprimitive).  
  
Retrieves a type given its primitive type.  
  
## Syntax  
  
```cpp#  
HRESULT GetTypeFromPrimitive(  
   DWORD         dwCorElementType,  
   IDebugField** ppType  
);  
```  
  
```csharp  
int GetTypeFromPrimitive(  
   uint            dwCorElementType,  
   out IDebugField ppType  
);  
```  
  
#### Parameters  
 `dwCorElementType`  
 [in] Value from the [CorElementType Enumeration](/dotnet/framework/unmanaged-api/metadata/corelementtype-enumeration) that represents the primitive type.  
  
 `ppType`  
 [out] Returns the [IDebugField](../../../extensibility/debugger/reference/idebugfield.md) that represents the type.  
  
## Return Value  
 If successful, returns `S_OK`; otherwise, returns an error code.  
  
## See Also  
 [IDebugDynamicFieldCOMPlus](../../../extensibility/debugger/reference/idebugdynamicfieldcomplus.md)

