### Add cors

<pre><code data-trim data-noescape class="hljs" data-line-numbers>
cors = require('cors')

var corsOptions = {
  origin: '*',
};

app.use(cors(corsOptions))
</code></pre>