<pre><code data-trim data-noescape class="hljs" data-line-numbers>
cors = require('cors')

var corsOptions = {
  origin: 'mysite.com',
};

app.use(cors(corsOptions))
</code></pre>

<pre><code data-trim data-noescape data-line-numbers>
Access-Control-Allow-Origin: mysite.com
</code></pre>