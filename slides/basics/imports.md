## Import and Initialize

<pre><code data-trim data-noescape class="hljs" data-line-numbers="1,2">
const express = require("express");
const app = express();

app.get("/", (request, response) => {
  response.send("Hello world!");
});

const listener = app.listen(process.env.PORT, () =>
    console.log("Your app is listening on port " + listener.address().port));

</code></pre>

note:
 - Getting the express initializer from the express.js node module
 - Creating an instance of express on the `app` constant