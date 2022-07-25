# Order Placed

### 

## Javascript Code
```js
window.dataLayer = window.dataLayer || [];
dataLayer.push({ ecommerce: null });  // Clear the previous ecommerce object.
dataLayer.push({
  "event": "purchase",
  "detailed_event": "Order Placed",
    "ecommerce": {
        "affiliation": "<affiliation>",
        "cart_id": "<cart_id>",
        "country": "<country>",
        "currency": "<currency>",
        "fulfillment_method": "<fulfillment_method>",
        "items": [
            {
                "affiliation": "<affiliation>",
                "currency": "<currency>",
                "item_category": "<item_category>",
                "item_category2": "<item_category2>",
                "item_category3": "<item_category3>",
                "item_category4": "<item_category4>",
                "item_category5": "<item_category5>",
                "item_id": "<item_id>",
                "item_name": "<item_name>",
                "item_variant": "<item_variant>",
                "price": <price>,
                "quantity": <quantity>
            }
        ],
        "payment_id": "<payment_id>",
        "payment_method": "<payment_method>",
        "postal_code": "<postal_code>",
        "revenue_band": "<revenue_band>",
        "state_province": "<state_province>",
        "transaction_id": "<transaction_id>",
        "value": <value>
    }
});
```

## Variable Definitions

|Path|Type|Description|Example|Pattern|Min Length|Max Length|Minimum|Maximum|Multiple Of|
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
|ecommerce.affiliation|string|A order affiliation to designate a supplying company or brick and mortar store location.|Google Store|||||||
|ecommerce.cart_id|string|Captures the name or ID of the region within which CTA links are used.|12345, 435678, 34567, XCV456, XCV876|||||||
|ecommerce.country|string|Captures the country associated with payments used for a transaction \(i.e. order, booking, dontation, etc.\).|US, CA, FR, UK|^[A-Z]{2}$||||||
|ecommerce.currency|string|The currency, in 3-letter ISO 4217 format.||||||||
|ecommerce.fulfillment_method|string|Captures the shipping fullfilment method associated with a product.|Shipped, Emailed, Pick Up In Store, Will Call|||||||
|ecommerce.items[n].affiliation|string|A product affiliation to designate a supplying company or brick and mortar store location.|Google Store|||||||
|ecommerce.items[n].currency|string|The currency, in 3-letter ISO 4217 format.|USD|||||||
|ecommerce.items[n].item_category|string|Item Category \(context-specific\). item\_category2 through item\_category5 can also be used if the item has many categories.|pants|||||||
|ecommerce.items[n].item_category2|string|The second category of an item.||||||||
|ecommerce.items[n].item_category3|string|The third category of an item.||||||||
|ecommerce.items[n].item_category4|string|The fourth category of an item.||||||||
|ecommerce.items[n].item_category5|string|The fifth category of an item.||||||||
|ecommerce.items[n].item_id|string|Item ID \(context-specific\).The product primary ID \(SKU or UPC\)|SKU\_12345|||||||
|ecommerce.items[n].item_name|string|Item Name \(context-specific\).|jeggings|||||||
|ecommerce.items[n].item_variant|string|The variant of the item.|Black|||||||
|ecommerce.items[n].price|number|The monetary price of the item, in units of the specified currency parameter.|9.99|||||||
|ecommerce.items[n].quantity|integer|Item quantity.|1|||||||
|ecommerce.payment_id|string|Captures a unique payment ID for a transaction.||ZPH-87698-098||||||
|ecommerce.payment_method|string|Captures the payment methods used for a transaction \(i.e. credit card, Visa, MasterCard, Amex, Paypal, purchase order, etc\).|Credit Card, PayPal, Mastercard, Visa, Amex, Discover|||||||
|ecommerce.postal_code|string|Captures the postal code associated with a transaction \(i.e. order, booking, dontation, etc.\).|53533, 30381, M1R 0E9, M3C 0C1|||||||
|ecommerce.revenue_band|string|Captures the revenue dollar amount of the order for use in bucketing orders into specific revenue bands \(i.e. $0-$50, $51-$100\).|125.05, 432.21, 90.22, 12.05|^[0-9]*(\.[0-9]{1,2})?$||||||
|ecommerce.state_province|string|Captures the state or province associated with payments used for a transaction \(i.e. order, booking, dontation, etc.\).|WI, GA, NB, ON|||||||
|ecommerce.transaction_id|string|The unique identifier of a transaction.|T\_12345, 19283j2nm9jdjs|^[a-zA-Z0-9]{6,20}$|6|20||||
|ecommerce.value|number|The monetary value of the event.|7.77, 239.55, 659|||||||




