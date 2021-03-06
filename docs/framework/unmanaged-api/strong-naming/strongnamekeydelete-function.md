---
title: "StrongNameKeyDelete Function"
ms.date: "03/30/2017"
api_name:
  - "StrongNameKeyDelete"
api_location:
  - "mscoree.dll"
api_type:
  - "DLLExport"
f1_keywords:
  - "StrongNameKeyDelete"
helpviewer_keywords:
  - "StrongNameKeyDelete function [.NET Framework strong naming]"
ms.assetid: 313e71e4-1790-4d2f-b68b-5040ebd1c149
topic_type:
  - "apiref"
author: "rpetrusha"
ms.author: "ronpet"
---

# StrongNameKeyDelete Function

Deletes the specified key container.

This function has been deprecated. Use the [ICLRStrongName::StrongNameKeyDelete](../../../../docs/framework/unmanaged-api/hosting/iclrstrongname-strongnamekeydelete-method.md) method instead.

## Syntax

```cpp
BOOLEAN StrongNameKeyDelete (
    [in]  LPCWSTR   wszKeyContainer
);
```

#### Parameters

`wszKeyContainer`
[in] The name of the key container to delete.

## Return Value

`true` on successful completion; otherwise, `false`.

## Remarks

Use the [StrongNameKeyInstall](../../../../docs/framework/unmanaged-api/strong-naming/strongnamekeyinstall-function.md) function to import a public/private key pair into a container.

If the `StrongNameKeyDelete` function does not complete successfully, call the [StrongNameErrorInfo](../../../../docs/framework/unmanaged-api/strong-naming/strongnameerrorinfo-function.md) function to retrieve the last generated error.

## Requirements

**Platforms:** See [System Requirements](../../../../docs/framework/get-started/system-requirements.md).

**Header:** StrongName.h

**Library:** Included as a resource in MsCorEE.dll

**.NET Framework Versions:** [!INCLUDE[net_current_v10plus](../../../../includes/net-current-v10plus-md.md)]

## See also

- [StrongNameKeyDelete Method](../../../../docs/framework/unmanaged-api/hosting/iclrstrongname-strongnamekeydelete-method.md)
- [StrongNameKeyInstall Method](../../../../docs/framework/unmanaged-api/hosting/iclrstrongname-strongnamekeyinstall-method.md)
- [ICLRStrongName Interface](../../../../docs/framework/unmanaged-api/hosting/iclrstrongname-interface.md)
