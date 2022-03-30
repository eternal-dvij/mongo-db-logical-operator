# mongo-db-logical-operator
Advanced CRUD Operations | Logic Operators

# **Query:** 
db.companies.find({"$or":[{"$and":[{"founded_year":{"$eq":2004}},{"$or":[{"category_code":{"$eq":"social"}},{"category_code":{"$eq":"web"}}]}]},{"$and":[{"founded_month":{"$eq":10}},{"$or":[{"category_code":{"$eq":"social"}},{"category_code":{"$eq":"web"}}]}]}]}
).count()


To complete this exercise connect to your Atlas cluster using the in-browser IDE space.

How many companies in the (database).(document-name) dataset were 

either founded in 2004
[and] either have the social category_code [or] web category_code,

[or] were founded in the month of October
[and] also either have the social category_code [or] web category_code?

Answer: 149
