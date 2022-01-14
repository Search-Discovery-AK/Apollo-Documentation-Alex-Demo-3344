# Product Location Listing Item Clicked

### 

## Javascript Code
```js
window.appEventData = window.appEventData || [];;;
appEventData.push({
  "event": "Product Location Listing Item Clicked",
    "listingItemClicked": {
        "listing": [
            {
                "itemPosition": <itemPosition>,
                "location": {
                    "latitude": <latitude>,
                    "longitude": <longitude>
                },
                "price": {
                    "pointRangeLow": <pointRangeLow>
                },
                "productInfo": {
                    "productID": "<productID>"
                }
            }
        ],
        "listingContext": "<listingContext>",
        "listingDriver": "<listingDriver>"
    }
});
```

## Variable Definitions

|Field|Type|Description|Example|Pattern|Min Length|Max Length|Minimum|Maximum|Multiple Of|
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
|itemPosition|integer|Integer position of a property within a sorted result. The first returned is position 1. For map results, this value can be the rank by distance from POI.|1, 2, 3, 4, 5||||0|||
|latitude|number|The latitude of the map center for a location search.|48.858093||||-90|90||
|listingContext|string|Describes the context of a listing display \(sort changed, filter added, filter removed\)|Filter Added, Filter Removed, Sort Change, Pagination|||||||
|listingDriver|string|Describes the action that caused the listing to be displayed|Onsite Search, Curated Assortment, Navigation|||||||
|longitude|number|The longitude of the map center for a location search.|2.294694||||-180|180||
|pointRangeLow|integer|Lower end of the point range shown.|1000, 1510, 1800|||||||
|productID|string|Unique Identifier of a product or offering.  Must match the format of back-end systems if used as a key for import of product meta data. Most often, one level above SKU for products with SKU variants. |155, 65588, 987764448|||||||




