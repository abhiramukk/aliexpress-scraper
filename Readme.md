# Aliexpress Dataset

| Field name          | Field Type            | Description                                                                                                        |
| ------------------- | --------------------- | ------------------------------------------------------------------------------------------------------------------ |
| website_name        | Fixed value           | Name of the website, as provided                                                                                   |
| competence_date     | Formula               | Date of data collection format YYYY-MM-DD                                                                          |
| brand               | From website          | Brand, as appears on product list page (PLP)                                                                       |
| product_code        | From website          | Product ID as appears in PLP.                                                                                      |
| country_code        | Fixed value           | ISO 3 letter country code                                                                                          |
| variant description | From website          | Variant description                                                                                                |
| currency_code       | Fixed value           | ISO 3 letter currency code. This must be consistent with currency code expected for the country                    |
| full_price          | From website          | Decimal, precision 2. Price before visible discount. If multiple prices are available, the highest price available |
| price               | From website          | Decimal, precision 2. Discounted price                                                                             |
| category1_code      | From website          | navigation tree level 1                                                                                            |
| category2_code      | From website          | navigation tree level 2                                                                                            |
| category3_code      | From website          | navigation tree level 3                                                                                            |
| title               | From website          | Product title                                                                                                      |
| long description    | From website          | Concatenation of all description fields in product detail page                                                     |
| imageurl            | From website          | URL of image                                                                                                       |
| itemurl             | From website          | URL of product detail page (PDP)                                                                                   |
| contract_id         | Seller specific value | ID of contract (assigned upon application)                                                                         |
| seller_id           | Seller specific value | ID of seller, assigned upon acceptance as seller                                                                   |
| delivery_id         | Formula               | Timestamp in Unix Epoch format. NNNNNNNNNN.NNNNNNN EXTRACT(EPOCH FROM current_timestamp). Ex. 1693286240.4167356   |
