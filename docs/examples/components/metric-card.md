# Metric Card Template

## Default State
```
╭──────────────────────────────╮
│ {{icon}} {{label}}           │
│                              │
│ {{value}}                    │
│ {{trend}} ↑                  │
│                              │
│ {{subtitle}}                 │
│ ──────────────────────────── │
│ {{footer}}                   │
╰──────────────────────────────╯
```

## Positive Trend (Up)
```
╭──────────────────────────────╮
│ 💰 Cash Position             │
│                              │
│ $2,458,392.00                │
│ +12.3% ↑                     │
│                              │
│ Available balance            │
│ ──────────────────────────── │
│ Updated 2 min ago            │
╰──────────────────────────────╯
```

## Negative Trend (Down)
```
╭──────────────────────────────╮
│ 📉 Accounts Payable          │
│                              │
│ $847,291.00                  │
│ -5.2% ↓                      │
│                              │
│ Due within 30 days           │
│ ──────────────────────────── │
│ Updated 5 min ago            │
╰──────────────────────────────╯
```

## Neutral/No Trend
```
╭──────────────────────────────╮
│ 📊 Net Working Capital       │
│                              │
│ $1,611,101.00                │
│ No change →                  │
│                              │
│ 30-day average               │
│ ──────────────────────────── │
│ Updated just now             │
╰──────────────────────────────╯
```

## Compact (No Footer/Subtitle)
```
╭──────────────────────────────╮
│ 💵 Available Credit          │
│                              │
│ $500,000.00                  │
│ 75% utilized                 │
╰──────────────────────────────╯
```

## Usage

The metric card displays key financial metrics with:
- **Label**: The metric name/title
- **Icon**: Visual indicator (optional)
- **Value**: The main metric value (typically currency)
- **Trend**: Percentage or directional change indicator
- **Subtitle**: Additional context (optional)
- **Footer**: Timestamp or metadata (optional)

The card automatically styles based on `trendDirection`:
- `up`: Success/positive styling (green)
- `down`: Error/negative styling (red)
- `neutral`: Neutral styling (gray)
