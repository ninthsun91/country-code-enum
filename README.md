# Country and Currency code in const Enum
last updated: 2024-03-30

This package contains const enums for,

- Country code (ISO 3166-1 alpha-2) from [Wikipedia](https://en.wikipedia.org/wiki/ISO_3166-1_alpha-2)
- Currency code (ISO 4217) from [Wikipedia](https://en.wikipedia.org/wiki/ISO_4217)

Also, only active codes are included.

## Usage
```ts
import { Country, Currency } from 'country-code-enum';

Country.US
Currency.USD
```