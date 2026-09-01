# Global IBAN, BIC/SWIFT & Bank Routing Validator API — Rust Client

[![Crates.io](https://img.shields.io/crates/v/iban-validator-client.svg)](https://crates.io/crates/iban-validator-client)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![RapidAPI Listing](https://img.shields.io/badge/RapidAPI-Dedicated%20Listing-blueviolet)](https://rapidapi.com/noor-mkdad-apis-noor-mkdad-apis-default/api/global-iban-bic-swift-bank-routing-validator-api)

Official high-speed Rust client for **Global IBAN, BIC/SWIFT & Bank Routing Validator API**.

> High-speed ISO 13616 MOD-97 IBAN checksum verification, ISO 9362 BIC/SWIFT validation, and national bank routing extraction across 87 countries.

> 🔑 **Get your Dedicated API Key:** [Subscribe to Global IBAN, BIC/SWIFT & Bank Routing Validator API on RapidAPI](https://rapidapi.com/noor-mkdad-apis-noor-mkdad-apis-default/api/global-iban-bic-swift-bank-routing-validator-api)

---

## 🚀 Installation

```bash
cargo add iban-validator-client
```

---

## ⚡ Quickstart

```rust
use iban_validator_client::{IbanValidatorClient, RapidApiConfig};
use serde_json::json;

fn main() -> Result<(), Box<dyn std::error::Error>> {
    let client = IbanValidatorClient::new(Some(RapidApiConfig {
        api_key: "YOUR_RAPIDAPI_KEY".to_string(), // Get key from https://rapidapi.com/noor-mkdad-apis-noor-mkdad-apis-default/api/global-iban-bic-swift-bank-routing-validator-api
        ..Default::default()
    }));

    let result = client.validate(&json!({
        // Enter validation payload
    }))?;

    println!("Result: {:?}", result);
    Ok(())
}
```

---

## 🔗 Links
- 📖 [RapidAPI Documentation & Key](https://rapidapi.com/noor-mkdad-apis-noor-mkdad-apis-default/api/global-iban-bic-swift-bank-routing-validator-api)

## 📄 License
MIT © RapidAPI Microservices Portfolio
