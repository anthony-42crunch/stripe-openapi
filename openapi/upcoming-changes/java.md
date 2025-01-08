* Add support for `close` method on resource `Treasury.FinancialAccount`
* Add support for `ownership_exemption_reason` on `Account.company`, `AccountCreateParams.company`, `AccountUpdateParams.company`, and `TokenCreateParams.account.company`
* Add support for `directorship_declaration` on `Account.company`
* Add support for `advice_code` on `Charge.outcome`, `Invoice.last_finalization_error`, `PaymentIntent.last_payment_error`, `SetupAttempt.setup_error`, `SetupIntent.last_setup_error`, and `StripeError`
* Remove support for value `always_invoice` from enums `billingportal.ConfigurationCreateParams.features.subscription_cancel.proration_behavior` and `billingportal.ConfigurationUpdateParams.features.subscription_cancel.proration_behavior`
* Add support for `country` on `Charge.payment_method_details.paypal`, `ConfirmationToken.payment_method_preview.paypal`, and `PaymentMethod.paypal`
* Add support for `nickname` on `Treasury.FinancialAccount`, `treasury.FinancialAccountCreateParams`, and `treasury.FinancialAccountUpdateParams`
* Add support for `forwarding_settings` on `treasury.FinancialAccountUpdateParams`
* Add support for `is_default` on `Treasury.FinancialAccount`
* Add support for `destination_payment_method_data` on `treasury.OutboundTransferCreateParams`
* Add support for `financial_account` on `Treasury.OutboundTransfer.destination_payment_method_details`
* Change type of `Treasury.OutboundTransfer.destination_payment_method_details.type` from `literal('us_bank_account')` to `enum('financial_account'|'us_bank_account')`
* Add support for new value `outbound_transfer` on enum `treasury.ReceivedCreditListParams.linked_flows.source_flow_type`
* Add support for `outbound_transfer` on `Treasury.ReceivedCredit.linked_flows.source_flow_details`