# Check Balance

:link: URL : `https://wallet.mrbean.dev/api/:currency/getbalance`  <mark style="color:blue;background-color:green;">POST</mark>&#x20;

Using this page you can get your wallet balance.

## Note

* Add currency name in the link.&#x20;
  * Example : `https://wallet.mrbean.dev/api/TRX/getbalance`

## Parameters :

| Parameter  | Required | Type     | Example                                       | Description                                    |
| ---------- | -------- | -------- | --------------------------------------------- | ---------------------------------------------- |
| `api`      | `true`   | `string` | `1257374757365723a3123ds3633123213123421412a` | Get your API form your user dashboard.         |
| `currency` | `true`   | `string` | `TRX`                                         | send the currency you want to get balance for. |
| `address`  | `true`   | `string` | `TS28HzZK9QpVMYFDZkSib9TXHRB65Zni9D`          | send the address you want to check balance for |
