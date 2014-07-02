# Trim Objects

Sometimes you get data that needs to be trimmed, e.g. it has extra whitespace
at the beginning or end, like this:

{"   hello    ": "     world     "}

When what you really want is:

{"hello": "world"}

For trimming LDJSON data on the command line you can use **trim-object-stream**

To install it run **npm install --save trim-object-stream**

This challenge starts with a CSV file with 2000 lines of property parcel
ownership public data from the City of Oakland. The data is messy -- it has
lots of extra unnecessary whitespace.

This raw CSV data will be automatically piped into your gasket process.

**To pass this challenge** create a **package.json** file with a **"gasket"**
section that first converts the CSV data into LDJSON, and then prints out
the **"Owner name"** property of each JSON object with the keys and values trimmed.

Use the command **data-plumber verify package.json** to verify.

Use the command **data-plumber run package.json** to see the raw gasket output.

**Hint**: use the jku again for this challenge in addition to csv-parser
