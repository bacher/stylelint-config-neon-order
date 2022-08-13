# stylelint-config-hudochenkov

My configs for [Stylelint]. Uses rules from [`stylelint-order`].

Available configs:

* `stylelint-config-hudochenkov` — default config which includes rules from Stylelint core only.
* `stylelint-config-hudochenkov/order` — config for order of content within declaration blocks and properties order. Uses [`stylelint-order`].
* `stylelint-config-hudochenkov/full` — combines all configs together and includes:
  * `stylelint-config-hudochenkov`
  * `stylelint-config-hudochenkov/order`

## Installation

Install config:

```
npm install --save-dev stylelint-config-hudochenkov
```

If you're using `stylelint-config-hudochenkov/order` or `stylelint-config-hudochenkov/full`, install additional plugin:

```
npm install --save-dev stylelint-order
```

**Note:** Additional plugins not listed as `peerDependencies`, because not every project need them. npm will shows warning after each `npm install` if not all `peerDependencies` are installed, even if they are not used.

## Usage

Add chosen config to the [`extends` section](https://eslint.org/docs/user-guide/configuring#extending-configuration-files) of your Stylelint configuration:

```
{
	"extends": ["stylelint-config-hudochenkov"]
}
```

```
{
	"extends": ["stylelint-config-hudochenkov/full"]
}
```

Recommended to run Stylelint with [`--max-warnings` flag](https://stylelint.io/user-guide/usage/options#maxwarnings), because most of the rules has [`warning` severity](https://stylelint.io/user-guide/configure#severity):

```
stylelint "**/*.css" --max-warnings 0
```

[Stylelint]: https://stylelint.io/
[`stylelint-order`]: https://github.com/hudochenkov/stylelint-order
