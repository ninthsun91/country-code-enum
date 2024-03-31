# Country and Currency code in const Enum
last updated: 2024-03-30

This package contains const enums for,

- Country code (ISO 3166-1 alpha-2) from [Wikipedia](https://en.wikipedia.org/wiki/ISO_3166-1_alpha-2)
  - 249 officially assigned codes
  - 13 exceptionally reserved codes
  - 7 transitional reservations
- Currency code (ISO 4217) from [Wikipedia](https://en.wikipedia.org/wiki/ISO_4217)
  - 157 active currency codes

## Usage
Both `Country` and `Currency` can be used as **enum** or **union string type**.
```ts
import { Country, Currency } from 'country-code-enum';

const country: Country = getCountry();
let currency: Currency;

switch (country) {
    // use as enum
    case Country.US:
        currency = Currency.USD;
        break;

    // use as union type - you still get auto-complete
    case 'EU':
        currency = 'EUR';

        // ERROR: Type '"Hello"' is not assignable to type 'Currency' .ts(2322)
        // currency = 'Hello';
        break;
}
```

## Contribution
Any effort to make this package invaluable is appreciated.

Leave issues or PRs if there is any updates in standard codes or if you have suggestions.