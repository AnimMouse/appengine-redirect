# Google App Engine PHP redirect
The simple PHP HTTP redirect script designed to run on Google App Engine.

## Configuration
```
header("Location: URL_HERE", true, HTTP_RESPONSE_CODE_HERE);
```
Replace https://example.com to the domain of your choice in index.php.

Use either 301 for pernament redirect, or 303 for temporary redirect. (I don't recommend 302 for temporary redirect)
```
window.location.href = URL_HERE;
<meta http-equiv="refresh" content="0;URL=URL_HERE" />
```
Replace both https://example.com to the domain of your choice in over_quata.html.

Deploy.

## What is over_quata.html?
over_quata.html is used when the instance is experiencing over quata.

When the instance is experiencing over quata, the php redirect will not work, so the html file will be used to redirect.
