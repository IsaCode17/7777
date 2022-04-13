---
title: URL.hash
slug: Web/API/URL/hash
tags:
  - API
  - Property
  - Reference
  - URL
  - URL API
browser-compat: api.URL.hash
---

{{ APIRef("URL API") }}

A propriedade **`hash`** da interface {{domxref("URL")}} é uma {{domxref("USVString")}} contendo o `'#'` seguido pelo identificador de fragmento da URL.

O fragmento não é [percent-decoded](/en-US/docs/Glossary/percent-encoding). Se a URL não tem o framento de identificação, esta propriedade contém uma string — `""`.

{{AvailableInWorkers}}

## Valor

Uma {{domxref("USVString")}}.

## Exemplos

```js
const url = new URL(
  "https://developer.mozilla.org/en-US/docs/Web/API/URL/href#Examples"
);
console.log(url.hash); // Logs: '#Examples'
```

## Especificações

{{Specifications}}

## Compatibildiade de browser

{{Compat}}

## Veja também

- A interface {{domxref("URL")}} a quem pertence.
