# Withdraw

:link: URL : `https://wallet.mrbean.dev/api/:currency/withdraw`  <mark style="color:blue;background-color:green;">POST</mark>&#x20;

Using this you can send payment / withdraw.

## _Note :_

* _Add the currency name in the link._&#x20;
  * _Example :_ `https://wallet.mrbean.dev/api/TRX/withdraw`
* _All withdrawals are instantly made._

## Parameters :

<table><thead><tr><th width="143">Parameter</th><th width="104">Required</th><th width="112">Type</th><th width="173">Example</th><th width="215">Description</th></tr></thead><tbody><tr><td><code>api</code></td><td><code>true</code></td><td><code>string</code></td><td><code>1257374757365723a3123ds3633123213123421412a</code></td><td>Get your API form your user dashboard.</td></tr><tr><td><code>address</code></td><td><code>true</code></td><td><code>string</code></td><td><code>TS28HzZK9QpVMYFDZkSib9TXHRB65Zni9D</code></td><td>send the address to be checked</td></tr><tr><td><code>amount</code></td><td><code>true</code></td><td><code>numeric</code></td><td><code>100</code></td><td>Send the amount you want to withdraw.<br>Minimum Withdraw : <code>10</code> TRX<br>Fee : <code>1%</code></td></tr></tbody></table>

