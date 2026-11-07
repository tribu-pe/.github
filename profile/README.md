<p align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/tribu-pe/brand/main/logo/variants/tribu-horizontal-white.svg">
    <img src="https://raw.githubusercontent.com/tribu-pe/brand/main/logo/variants/tribu-horizontal-color-1200.png" alt="Tribu" width="320">
  </picture>
</p>

<p align="center">
  <strong>SUNAT electronic invoicing for TypeScript.</strong><br>
  Facturación electrónica SUNAT para TypeScript.
</p>

<p align="center">
  <a href="https://www.npmjs.com/package/tribu"><img src="https://img.shields.io/npm/v/tribu/experimental?label=npm&color=0F4C46" alt="npm version"></a>
  <a href="https://github.com/tribu-pe/tribu/blob/main/LICENSE"><img src="https://img.shields.io/github/license/tribu-pe/tribu?color=0F4C46" alt="MIT license"></a>
</p>

<p align="center">
  <a href="https://github.com/tribu-pe/tribu#readme">Get started</a> ·
  <a href="https://github.com/tribu-pe/tribu/tree/main/docs/guide">Guide</a> ·
  <a href="https://github.com/tribu-pe/tribu/blob/main/README.es.md">Leer en español</a>
</p>

Tribu is an open-source SDK for issuing Peruvian electronic payment documents to SUNAT. It calculates the amounts, validates the document against SUNAT's rules, builds and signs the XML, sends it, and hands back one plain record to save.

```ts
const { record } = await sunat.invoice({
  customer: { ruc: '20123456786', name: 'CLIENTE SAC' },
  items: [{ description: 'Teclado', quantity: 2, price: 118 }],
});
```

## Projects

| Project | What it does |
|---|---|
| [**tribu**](https://github.com/tribu-pe/tribu) | Issue invoices, receipts and notes to SUNAT |
| [**@tribu-pe/pdf**](https://github.com/tribu-pe/pdf) | Generate the printed representation of a document, with A4 and ticket templates |
| [**brand**](https://github.com/tribu-pe/brand) | Logo, palette, icons and usage guidelines |

## Status

Tribu is **experimental**. SUNAT's beta environment accepts every document type it issues, but it has not been verified in production yet.

## Contributing

Issues and pull requests are welcome. Start with the [contributing guide](https://github.com/tribu-pe/tribu/blob/main/CONTRIBUTING.md).
