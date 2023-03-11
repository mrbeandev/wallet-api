# Withdraw

:link: URL : `https://wallet.mrbean.dev/api/:currency/validate`  <mark style="color:blue;background-color:green;">POST</mark>&#x20;

Using this you can send payment / withdraw.

## _Note :_

* _Add the currency name in the link._&#x20;
  * _Example :_ `https://wallet.mrbean.dev/api/TRX/newaddress`
* _All withdrawals are instantly made._

## Parameters :

| Parameter | Required | Type      | Example                                       | Description                                                                                                       |
| --------- | -------- | --------- | --------------------------------------------- | ----------------------------------------------------------------------------------------------------------------- |
| `api`     | `true`   | `string`  | `1257374757365723a3123ds3633123213123421412a` | Get your API form your user dashboard.                                                                            |
| `address` | `true`   | `string`  | `TS28HzZK9QpVMYFDZkSib9TXHRB65Zni9D`          | send the address to be checked                                                                                    |
| `amount`  | `true`   | `numeric` | `100`                                         | <p>Send the amount you want to withdraw.<br>Minimum Withdraw : <code>2</code> TRX<br>Fee : <code>1</code> TRX</p> |

