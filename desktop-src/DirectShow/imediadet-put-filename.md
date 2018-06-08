---
Description: The put\_Filename method specifies the name of the source file for the media detector to use.
ms.assetid: 37bcc7ed-d2c1-4182-b85a-03bad92c5ba7
title: IMediaDet::put\_Filename method
ms.technology: desktop
ms.prod: windows
ms.author: windowssdkdev
ms.topic: article
ms.date: 05/31/2018
---

# IMediaDet::put\_Filename method

> [!Note]  
> \[Deprecated. This API may be removed from future releases of Windows.\]

 

The `put_Filename` method specifies the name of the source file for the media detector to use.

Do not call this method twice on the same MediaDet object. To use this interface with more than one source file, create separate instances of the MediaDet object.

## Syntax


```C++
HRESULT put_Filename(
  [in] BSTR newVal
);
```



## Parameters

<dl> <dt>

*newVal* \[in\]
</dt> <dd>

File name of the source.

</dd> </dl>

## Return value

If this method succeeds, it returns **S\_OK**. Otherwise, it returns an **HRESULT** error code.

## Remarks

> [!Note]  
> The header file Qedit.h is not compatible with Direct3D headers later than version 7.

 

> [!Note]  
> To obtain Qedit.h, download the [Microsoft Windows SDK Update for Windows Vista and .NET Framework 3.0](http://go.microsoft.com/fwlink/p/?linkid=129787). Qedit.h is not available in the Microsoft Windows SDK for Windows 7 and .NET Framework 3.5 Service Pack 1.

 

## Requirements



|                    |                                                                                         |
|--------------------|-----------------------------------------------------------------------------------------|
| Header<br/>  | <dl> <dt>Qedit.h</dt> </dl>      |
| Library<br/> | <dl> <dt>Strmiids.lib</dt> </dl> |



## See also

<dl> <dt>

[**IMediaDet Interface**](imediadet.md)
</dt> <dt>

[Error and Success Codes](error-and-success-codes.md)
</dt> </dl>

 

 



