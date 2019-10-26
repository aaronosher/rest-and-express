Let's tell the app about this router

<pre><code data-trim data-noescape class="hljs" data-line-numbers="2">
    const express = require("express");
    const usersRouter = require("./resources/users.js")
    const app = express();
</code></pre>

<pre><code data-trim data-noescape class="hljs" data-line-numbers="5">
    app.get("/", (request, response) => {
        response.send("Hello world!");
    });

    app.use("/users", usersRouter);

    const listener = app.listen(process.env.PORT, () =>
</code></pre>