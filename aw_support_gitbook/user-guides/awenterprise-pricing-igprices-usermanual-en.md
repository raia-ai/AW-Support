---
description: "EN-UM-AWEnterprise_8"
---


---
## Prices

### – CU:
The price is reduced by the amount entered.
**Technical info:** alphanumeric field, toggle field, numeric field

### Offset 1-20, rounding
Specification how the prices should be rounded after the change. In the first field, enter the type of rounding; in the second, the value in question to which rounding should be done.

*   **Up:** The price is rounded up to the specified decimal place.
*   **Down:** The price is rounded down to the specified decimal place.
*   **Com:** The price is rounded up or down to the specified decimal place.

**Example**

| Rounding | Value | from | to |
| :--- | :--- | :--- | :--- |
| to 50 | 4.38 € | 4.50 € | rounded up |
| | 4.78 € | 5.00 € | |
| from 50 | 4.38 € | 4.00 € | rounded down |
| | 4.78 € | 4.50 € | |
| Com 10 | 4.38 € | 4.40 € | rounded up |
| | 4.78 € | 4.80 € | |
| | 4.34 € | 4.30 € | rounded down |
| | 4.73 € | 4.70 € | |
| Com 100 | 4.38 € | 4.00 € | rounded down |
| | 4.78 € | 5.00 € | rounded up |

**Technical info:** alphanumeric field, toggle field, numeric field

### PU Price
Currently not used.

## Export matrices

**Master data > Prices > Export price lists**

