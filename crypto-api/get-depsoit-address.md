---
description: Using this , you can receive Deposits from users.
---

# Get Depsoit Address

:link: URL : `https://wallet.mrbean.dev/api/:currency/newaddress`  <mark style="color:blue;background-color:green;">POST</mark>&#x20;

## _Note :_

* _Add the currency name in the link._&#x20;
  * _Example :_ `https://wallet.mrbean.dev/api/TRX/newaddress`
* _This is a temporary address only; you have to mention the time for the expiry, or the default time is `900` Sec (`15` Minutes). If you will not mention the parameter, `time` the address will expire in 15 minutes automatically, and any deposit made to the address will be lost forever._

## Parameters :

| Parameter       | Required   | Type      | Example                                       | Description                                                                                                                                                                             |
| --------------- | ---------- | --------- | --------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `api`           | `true`     | `string`  | `1257374757365723a3123ds3633123213123421412a` | Get your API form your user dashboard.                                                                                                                                                  |
| `callback_name` | `optional` | `string`  | `TS28HzZK9QpVMYFDZkSib9TXHRB65Zni9D`          | send the address you want to check balance for                                                                                                                                          |
| `callback_url`  | `true`     | `string`  | `https://mywebsapp.com/callback.php`          | <p>We will be sending a POST notification to this URL when we receive a deposit.<br><br>For more info <a href="../api-deposits/deposit-notifications.md">Click here</a>.</p>            |
| `time`          | `optional` | `numeric` | `900`                                         | <p>send the seconds for this deposit to expire in.<br>Default = <code>900</code> Sec<br>Minimum = <code>900</code> Sec (15 Minutes)<br>Maximum = <code>3600</code> Sec (60 Minutes)</p> |

