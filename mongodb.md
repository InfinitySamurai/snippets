# Mongo DB

## Searching

* Filtering if a sub object exists: `find({<fieldName>: {$exists: true}})`

* Filtering use a `like` operator: `find({<fieldName>: /<partial text here>/})`

* Filtering for equalities: `find({<fieldName>: {$eq: <something>}})`
    * `$eq` can be replaced by other equalities: https://docs.mongodb.com/manual/reference/operator/query-comparison/
