# PayPal

A library for processing PayPal payments. Uses the new PayPal REST API.

The primary interface is the `PaymentStore`, which provides simple access to your collection of `Payment` objects, as stored by PayPal. The `PaymentStore` allows the caller to create a payment, examine its status, and execute the payment to accept the collected funds.
