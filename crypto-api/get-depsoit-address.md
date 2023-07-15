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

<table><thead><tr><th width="181">Parameter</th><th width="120">Required</th><th width="111">Type</th><th width="187">Example</th><th width="203">Description</th></tr></thead><tbody><tr><td><code>api</code></td><td><code>true</code></td><td><code>string</code></td><td><code>1257374757365723a3123ds3633123213123421412a</code></td><td>Get your API form your user dashboard.</td></tr><tr><td><code>callback_name</code></td><td><code>optional</code></td><td><code>string</code></td><td><code>myuser_asdas23123123123</code></td><td>The label you want to receive when you get the callback.</td></tr><tr><td><code>callback_url</code></td><td><code>true</code></td><td><code>string</code></td><td><code>https://mywebsapp.com/callback.php</code></td><td>We will be sending a POST notification to this URL when we receive a deposit.<br><br>For more info <a href="../api-deposits/deposit-notifications.md">Click here</a>.</td></tr><tr><td><code>time</code></td><td><code>optional</code></td><td><code>numeric</code></td><td><code>900</code></td><td>send the seconds for this deposit to expire in.<br>Default = <code>900</code> Sec<br>Minimum = <code>900</code> Sec (15 Minutes)<br>Maximum = <code>3600</code> Sec (60 Minutes)</td></tr></tbody></table>

