---
UID: NF:textstor.ITextStoreACP.GetText
title: ITextStoreACP::GetText (textstor.h)
description: The ITextStoreACP::GetText method returns information about text at a specified character position. This method returns the visible and hidden text and indicates if embedded data is attached to the text.
old-location: tsf\itextstoreacp_gettext.htm
tech.root: TSF
ms.assetid: c3788e8f-ddb8-4ad6-971c-e9c1f6a21f88
ms.date: 12/05/2018
ms.keywords: GetText, GetText method [Text Services Framework], GetText method [Text Services Framework],ITextStoreACP interface, ITextStoreACP interface [Text Services Framework],GetText method, ITextStoreACP.GetText, ITextStoreACP::GetText, _tsf_itextstoreacp_gettext_ref, textstor/ITextStoreACP::GetText, tsf.itextstoreacp_gettext
ms.topic: method
f1_keywords:
- textstor/ITextStoreACP.GetText
dev_langs:
- c++
req.header: textstor.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows 2000 Professional [desktop apps only]
req.target-min-winversvr: Windows 2000 Server [desktop apps only]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: Textstor.idl
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: 
req.dll: Msctf.dll
req.irql: 
topic_type:
- APIRef
- kbSyntax
api_type:
- COM
api_location:
- msctf.dll
api_name:
- ITextStoreACP.GetText
targetos: Windows
req.typenames: 
req.redist: TSF 1.0 on Windows 2000 Professional
ms.custom: 19H1
---

# ITextStoreACP::GetText


## -description


The <b>ITextStoreACP::GetText</b> method returns information about text at a specified character position. This method returns the visible and hidden text and indicates if embedded data is attached to the text.


## -parameters




### -param acpStart [in]

Specifies the starting character position.


### -param acpEnd [in]

Specifies the ending character position. If this parameter is 1, then return all text in the text store.


### -param pchPlain [out]

Specifies the buffer to receive the plain text data. If this parameter is <b>NULL</b>, then the <i>cchPlainReq</i> parameter must be 0.


### -param cchPlainReq [in]

Specifies the number of plain text characters passed to the method.


### -param pcchPlainRet [out]

Receives the number of characters copied into the plain text buffer. This parameter cannot be <b>NULL</b>. Use a parameter if values are not required.


### -param prgRunInfo [out]

Receives an array of <a href="https://docs.microsoft.com/windows/desktop/api/textstor/ns-textstor-ts_runinfo">TS_RUNINFO</a> structures. May be <b>NULL</b> only if <i>cRunInfoReq</i> = 0.


### -param cRunInfoReq [in]

Specifies the size, in characters, of the text run buffer.


### -param pcRunInfoRet [out]

Receives the number of <b>TS_RUNINFO</b> structures written to the text run buffer. This parameter cannot be <b>NULL</b>.


### -param pacpNext [out]

Receives the character position of the next unread character. Cannot be <b>NULL</b>.


## -returns



This method can return one of these values.

<table>
<tr>
<th>Value</th>
<th>Description</th>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>S_OK</b></dt>
</dl>
</td>
<td width="60%">
The method was successful.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>TF_E_INVALIDPOS</b></dt>
</dl>
</td>
<td width="60%">
The <i>acpStart</i> or <i>acpEnd</i> parameters are outside of the document text.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>TF_E_NOLOCK</b></dt>
</dl>
</td>
<td width="60%">
The caller does not have a read-only lock on the document.

</td>
</tr>
</table>
 




## -remarks



Callers that use this method must have a read-only lock on the document by calling the <b>ITextStoreACP::RequestLock</b> method. Without a read-only lock, the method fails and returns <a href="https://docs.microsoft.com/windows/desktop/TSF/manager-return-values">TF_E_NOLOCK</a>.

Applications can also truncate the method return values for internal reasons. Callers should carefully examine the return characters and text run counts to get the required return values. If the return values are incomplete, repeatedly call the method until the return values are complete.

The caller can request plain text only by setting the <i>cRunInfoReq</i> parameter to 0 and the <i>prgRunInfo</i> parameter to <b>NULL</b>. The caller can request only text run data by setting the <i>cchPlainReq</i> parameter to 0 and the <i>pchPlain</i> parameter to <b>NULL</b>. However, the caller must still supply valid non-<b>null</b> values for <i>pcchPlainRet</i>, even if this parameter is not used.

If <i>acpEnd</i> is -1, then it should be handled as if set at the end of the stream. Otherwise, it will be greater than or equal to zero.

On exit, <i>pacpNext</i> should be set to the character position of the next character in the stream not referenced by the return values. A caller would use this to quickly scan text with multiple ITextStoreACP::GetText calls.




## -see-also




<a href="https://docs.microsoft.com/windows/desktop/api/textstor/nn-textstor-itextstoreacp">ITextStoreACP</a>



<a href="https://docs.microsoft.com/windows/desktop/api/textstor/nf-textstor-itextstoreacp-requestlock">ITextStoreACP::RequestLock
      </a>



<a href="https://docs.microsoft.com/windows/desktop/TSF/manager-return-values">Manager Return Values</a>



<a href="https://docs.microsoft.com/windows/desktop/api/textstor/ns-textstor-ts_runinfo">TS_RUNINFO
      </a>
 

 

