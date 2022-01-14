# Product Location Listing Displayed

### 

## Javascript Code
```js
window.appEventData = window.appEventData || [];;;
appEventData.push({
  "event": "Product Location Listing Displayed",
    "listingDisplayed": {
        "displayCount": <displayCount>,
        "listing": [
            {
                "price": {
                    "pointRangeLow": <pointRangeLow>,
                    "priceRangeHigh": "<priceRangeHigh>"
                },
                "productInfo": {
                    "brand": "<brand>",
                    "productID": "<productID>"
                }
            }
        ]
    }
});
```

## Variable Definitions

|Field|Type|Description|Example|Pattern|Min Length|Max Length|Minimum|Maximum|Multiple Of|
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
|brand|string|Describes the brand of a product or offering.|Ford, Chevrolet, Dodge, Levis, Columbia, Patagonia|||||||
|displayCount|integer|The total number of items displayed out of all returned items. \(Integer\)|10, 20, 30, 40||||0|||
|pointRangeLow|integer|Lower end of the point range shown.|1000, 1510, 1800|||||||
|priceRangeHigh|string|String representation of the upper end of the price range shown.||^[0-9]*(\.[0-9]{1,2})?$||||||
|productID|string|Unique Identifier of a product or offering.  Must match the format of back-end systems if used as a key for import of product meta data. Most often, one level above SKU for products with SKU variants. |155, 65588, 987764448|||||||




