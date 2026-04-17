Summary Scorecard   
Total Tests:  20  
Passed:  15   
Failed:  5   
Pass Rate:  75%   

### Suite 1: Registration and Security

| TC ID | Test Scenario | Priority | Actual Result | Status |
| :--- | :--- | :--- | :--- | :--- |
| **REG_01** | Valid Registration | High | Account created | ✅  |
| **REG_02** | Duplicate Email | High | Correct error shown | ✅  |
| **REG_03** | Empty Fields | Medium | Generic error shown | ✅  |
| **REG_04** | Password Masking | High | Input is hidden | ✅  |
| **REG_05** | Whitespace Password | Critical | Accepted 6 spaces | ❌  |
| **REG_06** | Privacy Policy | Medium | Correctly blocked | ✅  |
| **REG_07** | Phone Data Type | Medium | Accepted "ABCDEF" | ❌  |

### Suite 2: Product Search & Discovery
| TC ID | Test Scenario | Priority | Actual Result | Status |
| :--- | :--- | :--- | :--- | :--- |
| **SRCH_01** | Existing Product Search | High | Product "iPhone" found | ✅  |
| **SRCH_02** | Non-existent Product | Low | "No products match" msg | ✅  |
| **SRCH_03** | Empty Search Query | Low | Shown "no match" msg | ✅  |
| **SRCH_04** | Category Navigation | Medium | Correct products load | ✅  |
| **SRCH_05** | Currency Toggle | High | UI updates to €/£ | ✅  |

### Suite 3: Shopping Cart Logic
| TC ID | Test Scenario | Priority | Actual Result | Status |
| :--- | :--- | :--- | :--- | :--- |
| **CART_01** | Add to Cart (Home) | High | Total updated instantly | ✅  |
| **CART_02** | Quantity Increase | High | Math is correct (Price x N) | ✅  |
| **CART_03** | Remove Item | High | Item removed; Total $0.00 | ✅  |
| **CART_04** | Negative Quantity | Critical | Subtracted from total | ❌  |
| **CART_05** | Zero Quantity | Medium | Showed "Success" msg | ❌  |

### Suite 4: Checkout Flow
| TC ID | Test Scenario | Priority | Actual Result | Status |
| :--- | :--- | :--- | :--- | :--- |
| **CHKT_01** | Guest Checkout Flow | High | Step-by-step works | ✅  |
| **CHKT_02** | Terms & Cond. Bypass | High | Correctly blocked | ✅  |
| **CHKT_03** | Inventory Validation | Critical | Blocked only at end | ❌  |
