---
title: EcdsaParams
slug: Web/API/EcdsaParams
tags:
  - API
  - Dictionary
  - EcdsaParams
  - Reference
  - Web Crypto API
spec-urls: https://www.w3.org/TR/WebCryptoAPI/#dfn-EcdsaParams
---
{{ APIRef("Web Crypto API") }}

The **`EcdsaParams`** dictionary of the [Web Crypto API](/en-US/docs/Web/API/Web_Crypto_API) represents the object that should be passed as the `algorithm` parameter into {{domxref("SubtleCrypto.sign()")}} or {{domxref("SubtleCrypto.verify()")}} when using the [ECDSA](/en-US/docs/Web/API/SubtleCrypto/sign#ecdsa) algorithm.

## Properties

- `name`
  - : A string. This should be set to `ECDSA`.
- `hash`

  - : A string. An identifier for the [digest algorithm](/en-US/docs/Web/API/SubtleCrypto/digest) to use. This should be one of the following:

    - `SHA-256`: selects the [SHA-256](/en-US/docs/Web/API/SubtleCrypto/digest#sha-256) algorithm.
    - `SHA-384`: selects the [SHA-384](/en-US/docs/Web/API/SubtleCrypto/digest#sha-384) algorithm.
    - `SHA-512`: selects the [SHA-512](/en-US/docs/Web/API/SubtleCrypto/digest#sha-512) algorithm.

    > **Warning:** `SHA-1` is also supported here but the [SHA-1](/en-US/docs/Web/API/SubtleCrypto/digest#sha-1) algorithm is considered vulnerable and should no longer be used.

## Examples

See the examples for {{domxref("SubtleCrypto.sign()")}} or {{domxref("SubtleCrypto.verify()")}}.

## Specifications

{{Specifications}}

## Browser compatibility

Browsers that support the "ECDSA" algorithm for the {{domxref("SubtleCrypto.sign()")}} and {{domxref("SubtleCrypto.verify()")}} methods will support this type.

{{Compat("api.SubtleCrypto.sign")}}

## See also

- {{domxref("SubtleCrypto.sign()")}} and {{domxref("SubtleCrypto.verify()")}}.
