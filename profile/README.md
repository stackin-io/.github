<div align="center">
  <img src="https://raw.githubusercontent.com/stackin-io/stackin-python-sdk/master/docs/assets/stackin.png" width="140" />

  # stackin.io

  **Issue fiscal documents from a single API call.**  
  NFe · NFSe · Multi-tenant · Multi-jurisdiction

  [![License](https://img.shields.io/badge/license-MIT-informational?style=flat-square)](https://stackin.io)
  [![Python SDK](https://img.shields.io/pypi/v/stackin-python-sdk?label=python%20sdk&style=flat-square)](https://pypi.org/project/stackin-python-sdk)
  [![Go SDK](https://img.shields.io/badge/go%20sdk-available-00ADD8?style=flat-square)](https://github.com/stackin-io/stackin-go-sdk)
</div>

---

## What is stackin?

Stackin abstracts Brazil's fiscal infrastructure (SEFAZ, NFe model 55, NFSe national) behind a simple REST API.  
No certificates, no XML, no XSD, no SOAP — just business fields.

```python
from stackin import Invoice, DocumentType
from stackin.br import Product

client = Invoice(api_key="COMPANY_API_KEY")

client.issue(
    document_type=DocumentType.NFSE,
    client_name="John Doe",
    tax_id="00000000000",
    items=[Product(description="Software development", amount=5000.00)],
)
```

---

## SDKs

| Language | Package | Status |
|----------|---------|--------|
| Python | [`stackin-python-sdk`](https://github.com/stackin-io/stackin-python-sdk) | `pip install stackin-python-sdk` |
| Go | [`stackin-go-sdk`](https://github.com/stackin-io/stackin-go-sdk) | available |

---

## Links

- [Dashboard](https://app.stackin.io)
- [Docs](https://stackin.io)
- [API Reference](https://github.com/stackin-io/stackin-api/blob/master/docs/API.md)
- [support@stackin.io](mailto:support@stackin.io)
