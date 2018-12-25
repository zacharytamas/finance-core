# finance-core

[![Greenkeeper badge](https://badges.greenkeeper.io/zacharytamas/finance-core.svg)](https://greenkeeper.io/)

A collection of financial Excel-style formulas implemented as Polymer components for easy composition.

## Current Elements

- `fin-fv`
- `fin-pmt`
- `fin-pv`
- `fin-rate`
- `fin-nper`

## Utilities

- `fin-formatter`: Formats a value (such as one returned from one of the calculations) as currency, percentage, etc.

---

### Example usage

```html
<fin-fv period="5" present-value="1000" contribution="5000" rate="0.3" value="{{fv}}"></fin-fv>
<fin-formatter type="currency" value="{{fv}}" formatted-value="{{fvFormatted}}"></fin-formatter>

<div>
  <h1>Future Value</h1>
  <span>[[fvFormatted]]</span>
</div>
```
