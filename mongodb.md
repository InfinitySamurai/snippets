# Mongo DB

## Searching

- Filtering if a sub object exists: `find({<fieldName>: {$exists: true}})`

- Filtering use a `like` operator: `find({<fieldName>: /<partial text here>/})`

- Filtering for equalities: `find({<fieldName>: {$ne: "<something>"}})`
  - `$ne` can be replaced by other equalities: https://docs.mongodb.com/manual/reference/operator/query-comparison/
  - Note that `$eq` is the same as `<fieldName>: "<something>"`, so no need to use equalities when checking for exact match, or when using the above regexy thing `/<partial text here>/`
  - Remember quotes around things cause mongo is kinda stringy
- Finding documents that have a field in a list
  - `find({name: { $in: ["Joe", "Frank", "Mary", "Jane"]}})`
