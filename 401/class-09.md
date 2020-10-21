# Read 09

## Review

- How does route prefixing work with an external routing module?
In the line where you use the route `app.use()` you input the prefix you want, this way everything inside the route file has this prefix applied to them.

- When routing, what’s the difference between app.get('/data/:id') and app.get('/data/:name')?
This is how you set a parameter in the request `req.param`

- Explain how Express handles routing conflicts?
By priority, whatever comes first is more valid.

- What are the ways that a browser can send “data” or request variables to an HTTP server
fetch API, forms, ajax


## Preparation summary

### Router param

router.param(name, callback)
Adds callback triggers to route parameters, where name is the name of the parameter and callback is the callback function. Although name is technically optional, using this method without it is deprecated starting with Express v4.11.0 (see below).

The parameters of the callback function are:

req, the request object.
res, the response object.
next, indicating the next middleware function.
The value of the name parameter.
The name of the parameter.
Unlike app.param(), router.param() does not accept an array of route parameters.

### Middleware

Middleware (also called pre and post hooks) are functions which are passed control during execution of asynchronous functions. Middleware is specified on the schema level and is useful for writing plugins.

Types of Middleware
Mongoose has 4 types of middleware: document middleware, model middleware, aggregate middleware, and query middleware. Document middleware is supported for the following document functions. In document middleware functions, this refers to the document.

validate
save
remove
updateOne
deleteOne
init (note: init hooks are synchronous)
Query middleware is supported for the following Model and Query functions. In query middleware functions, this refers to the query.

count
deleteMany
deleteOne
find
findOne
findOneAndDelete
findOneAndRemove
findOneAndUpdate
remove
update
updateOne
updateMany

### Subdocuments

Subdocuments
Subdocuments are documents embedded in other documents. In Mongoose, this means you can nest schemas in other schemas. Mongoose has two distinct notions of subdocuments: arrays of subdocuments and single nested subdocuments.

const childSchema = new Schema({ name: 'string' });

const parentSchema = new Schema({
  // Array of subdocuments
  children: [childSchema],
  // Single nested subdocuments. Caveat: single nested subdocs only work
  // in mongoose >= 4.2.0
  child: childSchema
});
Aside from code reuse, one important reason to use subdocuments is to create a path where there would otherwise not be one to allow for validation over a group of fields (e.g. dateRange.fromDate <= dateRange.toDate).

### Populate Virtuals

So far you've only populated based on the _id field. However, that's sometimes not the right choice. In particular, arrays that grow without bound are a MongoDB anti-pattern. Using mongoose virtuals, you can define more sophisticated relationships between documents.
```
const PersonSchema = new Schema({
  name: String,
  band: String
});

const BandSchema = new Schema({
  name: String
});
BandSchema.virtual('members', {
  ref: 'Person', // The model to use
  localField: 'name', // Find people where `localField`
  foreignField: 'band', // is equal to `foreignField`
  // If `justOne` is true, 'members' will be a single doc as opposed to
  // an array. `justOne` is false by default.
  justOne: false,
  options: { sort: { name: -1 }, limit: 5 } // Query options, see http://bit.ly/mongoose-query-options
});

const Person = mongoose.model('Person', PersonSchema);
const Band = mongoose.model('Band', BandSchema);

/**
 * Suppose you have 2 bands: "Guns N' Roses" and "Motley Crue"
 * And 4 people: "Axl Rose" and "Slash" with "Guns N' Roses", and
 * "Vince Neil" and "Nikki Sixx" with "Motley Crue"
 */
Band.find({}).populate('members').exec(function(error, bands) {
  /* `bands.members` is now an array of instances of `Person` */
});
```