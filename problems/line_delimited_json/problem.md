# Line Delimited JSON

Line Delimited JSON (abbreviated as LDJSON or sometimes NDJSON for "Line" or
"Newline") is simply a plain text format where you have one piece of JSON-
encoded data per line, e.g.:

{"foo": "bar"}
{"foo": "bar"}
{"foo": "bar"}

(Notice no commas nor surrounding array.)

The **jsonfilter** command line module is really handy for processing LDJSON data.

Read about how it works at: **npmjs.org/jsonfilter**.

To install it, run **npm install --save jsonfilter**. This will add jsonfilter
to your package.json's dependencies field. **Note**: you don't have to use **-g**.
gasket is smart enough to find commands inside the node_modules directory.

**To pass this challenge:**

Create a **package.json** file with a **"gasket"** section that prints out the
**value** of the **name** field of each JSON object using the **jsonfilter**
module. It should print one name per line.

Raw data will be automatically piped into your gasket process.

Use the command **data-plumber run package.json** to see the raw gasket output.

Use the command **data-plumber verify package.json** to verify.
