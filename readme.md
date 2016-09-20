#Shop Module
###Lemonstand Version 1
This updated module can be installed using the updatecenter module: https://github.com/damanic/ls1-module-updatecenter

####Variant Invoice Templates
Allows for any number of 'invoice' variants to be selected for print (eg. quotes, refund, proforma-invoice, invoice). Example config in `/invoice_templates/ls_variant`

####Updates
- 1.30.0 Invoice templates updated to support variant commercial document templates (eg. quote, proforma-invoice) and some render override events (eg. pass html to a PDF renderer).
- 1.30.1 Minor improvement in the API. Added new API event: shop:onCustomerBeforeCreate
- 1.30.2 Minor improvement in the API. Added new API event: shop:onBeforeCheckoutStepPay
- 1.30.3 Minor improvement in internal classes. Shop_OrderHelper deprecated some methods in Shop_Orders controller
- 1.30.4 Minor improvement. Shop_Settings controller triggers form record events (core:onBeforeFormRecordUpdate|core:onAfterFormRecordUpdate).
- 1.30.5 Minor improvement. Added shop:onCustomerSaved event to Customer Model. This is fired on both model create and update.
- 1.30.6 Minor improvement. Added filter to hide disabled shipping options in list view.
- 1.30.7 New Event: Added shop:onOrderSetAppliedCartRules
- 1.30.8 Minor improvement. Hidden order currency fields, updated reports to convert totals to shop/base currency if order in different currency.
- 1.30.9 Fix: Shop_PaymentType::update_currency_data()
- 1.30.10 New Event: shop:onGetOptionMatrixProduct
- 1.30.11 Added new API event: shop:onApplyOrderEmailVars
- 1.30.12 Fixed issue with order document/invoice templates
- 1.30.13 Added discount action 'Discount the shipping cost by fixed amount'