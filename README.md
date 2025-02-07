# customer-db-no-keys
Primary Keys (PK) - column or set of columns (in the case of a composite PK) in a database table that uniquely identifies every record within that table; a PK, such as the typical ID column, enforces uniqueness within table and ensures each record is identifiable.
PK Rules? 
1. Unique values only, no duplicate values, and identify with only one record in our table
2. PK needs to be never changing
3. PK can never be null (left blank)
4. Every table must have 1 and only 1 PK. 

Foreign Keys (FK) - column or columns (in the case of a composite FK) in a database table that is used to link tables with referential relationships (i.e. orders.user_id references users.user_id). FK also ensure accuracy by rejecting insertions when they don't match what's in the referenced table.
FK Rules? 
1. FK does not have to be unique, it can be repeated inside a table.
2. column in table we are referencing must have only unique values
3. good practice to make sure all FK reference PK in other tables
4. Possible to have multiple FKs in a table, or conversely 0 FKs.

Cardinality - help define MIN and MAX relationship between tables in a numerical context. Common cardinality relationships:
one-to-one - each value of a table is linked to a singular value in another table (i.e. a specific user may have personal info that only relates to that user)
one-to-many - singular value in a table connects with multiple values in another table (i.e. single customer can place many orders, but a specific order can only be placed by a single customer)
many-to-many - several values in one table link to multiple values in another table 


