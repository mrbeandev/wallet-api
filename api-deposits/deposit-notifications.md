---
description: Deposit notification details
---

# 💬 Deposit Notification's

when we receive a Deposit to any of our address we send a Notification to the `callback_url` that you have sent us when creating [New Deposit Address](../admin-wallet/get-deposit-address.md).

> #### _There are 2 Types of notifications :_
>
> > _Success Notification_
>
> > _Expired Notification_

### _Note :_

* _**Success** notification is sent when a new deposit is received._
* _**Expired** notification is sent when the generated deposit address is expired._&#x20;
* _If a user makes deposit after the address has expired it will be lost for ever._
* _All notification's will be sent in_ <mark style="color:blue;background-color:green;"></mark> <mark style="color:blue;background-color:green;"></mark><mark style="color:blue;background-color:green;">**POST**</mark> <mark style="color:blue;background-color:green;"></mark><mark style="color:blue;background-color:green;"></mark>  _method only._

## Parameters :

### Deposit Notification :

| Parameter  | Type      | Example                                                            | Description                                                                       |
| ---------- | --------- | ------------------------------------------------------------------ | --------------------------------------------------------------------------------- |
| `status`   | `string`  | `received`                                                         | the status will always be `received` when a deposit is made.                      |
| `currency` | `string`  | `TRX`                                                              | Currency of the deposit                                                           |
| `txid`     | `string`  | `03691d5ac7395c57145526a6ab18fcabe0a726655822c4eff4cabd9ca362d2c6` | The Txid of the Deposit                                                           |
| `amount`   | `numeric` | `100`                                                              | The amount of deposit received                                                    |
| `name`     | `string`  | `myuser1`                                                          | Will be sent only if you mentioned `callback_name` when creating the new address. |

### Expired Notification :



| Parameter | Type     | Example                              | Description                                                                       |
| --------- | -------- | ------------------------------------ | --------------------------------------------------------------------------------- |
| `status`  | `string` | `expired`                            | the status will always be `expired` when a deposit address has expired.           |
| `address` | `string` | `TS28HzZK9QpVMYFDZkSib9TXHRB65Zni9D` | The deposit address.                                                              |
| `name`    | `string` | `myuser1`                            | Will be sent only if you mentioned `callback_name` when creating the new address. |

