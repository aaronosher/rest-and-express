## Listen

<pre><code data-trim data-noescape class="hljs" data-line-numbers="8,9">
const express = require("express");
const app = express();

app.get("/", (request, response) => {
  response.send("Hello world!");
});

const listener = app.listen(process.env.PORT, () =>
    console.log("Your app is listening on port " + listener.address().port));

</code></pre>

note:
 - `app.listen` to tell the express instance what port to liten to
 - We're getting the port form a PORT environment variable set by Glitch