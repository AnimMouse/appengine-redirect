# Google App Engine PHP redirect
The simple PHP & HTTP redirect script designed to run on [Google App Engine](https://cloud.google.com/appengine).

## Configuration
```
header("Location: URL_HERE", true, HTTP_RESPONSE_CODE_HERE);
```
Replace https://example.com to the domain of your choice in index.php.

Use either 308 for permanent redirect, or 307 for temporary redirect.
```
window.location.href = URL_HERE;
<meta http-equiv="refresh" content="0;URL=URL_HERE" />
```
Replace both https://example.com to the domain of your choice in over_quata.html.

Deploy.

## What is over_quata.html?
over_quota.html is used when the instance is experiencing over quota.

When the instance is experiencing over quota, the PHP redirect will not work, so the HTML file will be used to redirect instead.