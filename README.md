# stylelint-config-ordering

Ordering config for [Stylelint]. Uses rules from [`stylelint-order`].

Based on https://github.com/hudochenkov/stylelint-config-hudochenkov/blob/master/order.js

## Installation

Install config:

```
npm install --save-dev stylelint-config-neon-order
```

## Usage

Add chosen config to the [`extends` section](https://eslint.org/docs/user-guide/configuring#extending-configuration-files) of your Stylelint configuration:

```json
{
	"extends": ["stylelint-config-neon-order"]
}
```

[Stylelint]: https://stylelint.io/
[`stylelint-order`]: https://github.com/hudochenkov/stylelint-order
