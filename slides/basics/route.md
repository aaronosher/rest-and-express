## Basic Route

<pre><code data-trim data-noescape class="hljs" data-line-numbers="4-6">
const express = require("express");
const app = express();

app.get("/", (request, response) => {
  response.send("Hello world!");
});

const listener = app.listen(process.env.PORT, () =>
    console.log("Your app is listening on port " + listener.address().port));

</code></pre>

note:
 - Telling express to execute the callback on the `/` route
 - Callback has a request and response object
 - Sending a plain text response use response.send