# finance-core
A collection of financial formulas implemented as Polymer components for easy composition. 

## Calculations

- `fin-future-value`
- `fin-present-value`
- `fin-payment`

## Utilities

- `fin-formatter`: Formats a value (such as one returned from one of the calculations) as currency, percentage, etc.

---

### Example usage

```html
<fin-future-value period="5" present-value="1000" contribution="5000" rate="0.3" value="{{fv}}"></fin-future-value>
<fin-formatter type="currency" value="{{fv}}" formatted-value="{{fvFormatted}}"></fin-formatter>
    
<div>
  <h1>Future Value</h1>
  <span>[[fvFormatted]]</span>
</div>
```
