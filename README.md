# BC_API
## Minimum Parameters:
1. **Name**: The name of your product as a string.
2. **Price**: How much the items costs in number format.
3. **Type**:
   1. **Physical**: Anything that is shipped to the customer, such as a t-shirt.
   2. **Digital**: Products that the customer downloads, such as a PDF of an ebook.
4. **Weight**: How much the product weighs as a number. The measurement unit is determined by the store settings.
5. **Category**: The {category_id} for the category this product belongs to. An item can be assigned to more than one category. You can /GET the category id by using:

```
{
	"name": "Dvorak Cello",
	"inventory_level": 0,
	"inventory_warning_level": 2,
	"inventory_tracking": "product",

	"is_visible": false,


	"price": 65.00,
	"cost_price": 32.00,
	"retail_price": 65.00,
	
	"type": "physical",
	"fixed_cost_shipping_price":,


	"weight": 5.
	"depth": 2,
	"width": 12,
	"height": 12,
	
	"description: "<p>blah blah blah</p>",
	"categories": [
		{{category_id}}
	],
	"condition": {group_sid==93 ? 'Used' : 'New'},
	"search_keywords": "Dvoark,Cello,{brand},{genre},{split on whitespace}",
	"is_condition_shown": true,
	"custom_fields": [
		{
			"name": "Genre",
			"value": {string}
		},
		{
			"name": "Source",
			"value": {string}
		},
		{
			"name": "Label",
			"value": {string},
		},
		{
			"name": "Artist",
			"value": {string}
		},
		{
			"name": "MediaAmount",
			"value": {int}
		},

	],
	"date_created": {Date.now().toLocaleString()},
	"date_modified": {Date.now().toLocaleString()},
	"images": array[object],

	"brand_id": {int},
}
```
Category:
- Source: e.g. clearaudio
- 


performer
label: MGM
storage location



```{layout_file}```?

```categories: {{category_id}}```?

```
"hidden"
	upc: {string}
	is_featured: {boolean}
	availibilty: {string}
		Availability of the product.
		Availability options are:
			available - the product can be purchased on the storefront;
			disabled - the product is listed in the storefront, but cannot be purchased;
			preorder - the product is listed for pre-orders.
		sort_order: {int}
			Priority to give this product when included in product lists on category pages and in search results. Lower integers will place the product closer to the top of the results.
	variant: array[object],
	sales_price: ,
```