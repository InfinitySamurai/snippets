# Mongo DB

## Searching

Filtering if a sub object exists: `find({<fieldName>: {$exists: true}})`

Filtering use a `like` operator: `find({<fieldName>: /<partial text here>/})`