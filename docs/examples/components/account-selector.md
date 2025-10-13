# Account Selector Template

## Closed State
```
Account
┌────────────────────────────────────────┐
│ Operating Account (...4521) ▼         │
└────────────────────────────────────────┘
```

## Open State (Dropdown)
```
Account
┌────────────────────────────────────────┐
│ Operating Account (...4521) ▲         │
├────────────────────────────────────────┤
│ ● Operating Account - Checking         │
│   Account: ****4521                    │
│   Balance: $2,458,392.00               │
├────────────────────────────────────────┤
│   Payroll Account - Checking           │
│   Account: ****7832                    │
│   Balance: $142,560.00                 │
├────────────────────────────────────────┤
│   Reserve Account - Savings            │
│   Account: ****9104                    │
│   Balance: $500,000.00                 │
├────────────────────────────────────────┤
│   Line of Credit                       │
│   Account: ****2398                    │
│   Available: $750,000.00               │
└────────────────────────────────────────┘
```

## Compact View (No Details)
```
Account: ┌──────────────────────────┐
         │ Operating (...4521) ▼   │
         └──────────────────────────┘
```

## With Search
```
Account
┌────────────────────────────────────────┐
│ 🔍 Search accounts...                  │
├────────────────────────────────────────┤
│ ● Operating Account - Checking         │
│   ****4521  •  $2,458,392.00           │
│                                        │
│   Payroll Account - Checking           │
│   ****7832  •  $142,560.00             │
│                                        │
│   Reserve Account - Savings            │
│   ****9104  •  $500,000.00             │
└────────────────────────────────────────┘
```

## Detailed View
```
┌──────────────────────────────────────────────────┐
│ Selected Account                                 │
├──────────────────────────────────────────────────┤
│ Operating Account - Primary Checking             │
│                                                  │
│ Account Number: ****4521                         │
│ Account Type: Business Checking                  │
│ Current Balance: $2,458,392.00                   │
│ Available Balance: $2,458,392.00                 │
│                                                  │
│ [Change Account ▼]                               │
└──────────────────────────────────────────────────┘
```

## Multi-Select Mode
```
Accounts (2 selected)
┌────────────────────────────────────────┐
│ ☑ Operating Account (...4521)          │
│ ☑ Payroll Account (...7832)            │
│ ☐ Reserve Account (...9104)            │
│ ☐ Line of Credit (...2398)             │
└────────────────────────────────────────┘
```

## Usage

The account selector allows users to:
- **View available accounts**: Shows all accounts with details
- **Select an account**: Change the active account for viewing
- **Search accounts**: Filter by name or number (if searchable)
- **View balances**: See current balance for each account
- **Account details**: Number (masked), type, balance

Account object structure:
```json
{
  "id": "acc-001",
  "name": "Operating Account",
  "number": "****4521",
  "type": "Checking",
  "balance": 2458392.00,
  "currency": "USD"
}
```

The selector automatically:
- Masks account numbers for security
- Formats currency values
- Highlights the selected account
- Supports keyboard navigation
