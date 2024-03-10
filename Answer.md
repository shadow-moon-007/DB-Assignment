Ans 1> the relationship between the "Product" and "Product_Category" entities is one-to-many. This means that a single product can belong to one category, but a category can have many products.

Ans 2> To ensure that each product in the "Product" table has a valid category assigned to it:
1. Not Null Constraint: You can add a NOT NULL constraint on the category_id column in the "Product" table.
    This will prevent products from being inserted without a valid category assigned.
2. Foreign Key Constraint: You can also add a FOREIGN KEY constraint on the category_id column in the "Product" table.
    This constraint will reference the primary key of the "Product_Category" table. This will ensure that the category_id specified in the "Product" table exists in the "Product_Category" table.
