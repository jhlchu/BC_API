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
	"name": "Dvoak Cello",
	"price": 65.00,
	cost_price: ,
	retail_price: ,
	sale_price: ,
	brand_id
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
	condition: "New",

}
```