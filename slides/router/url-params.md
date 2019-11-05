### URL Parameters

<pre><code data-trim data-noescape class="hljs" data-line-numbers="1">
router.put('/:name', (request, response) => {
  response.json({
    success: true,
    message: `Updated ${request.params.name} sucesfully.`,
  });
});
</code></pre>