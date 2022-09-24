# Get Balance

:link: URL : `https://wallet.mrbean.dev/api/user/`  <mark style="color:blue;background-color:green;">POST</mark>&#x20;

Using this you can get your wallet balance.

| Parameter  | Required   | Type     | Example                                       | Description                                    |
| ---------- | ---------- | -------- | --------------------------------------------- | ---------------------------------------------- |
| `api`      | `true`     | `string` | `1257374757365723a3123ds3633123213123421412a` | Get your API form your user dashboard.         |
| `method`   | `true`     | `string` | `get_balance`                                 | ---                                            |
| `currency` | `Optional` | `string` | `TRX`                                         | send the currency you want to get balance for. |
