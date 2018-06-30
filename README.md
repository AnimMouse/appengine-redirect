# Google App Engine PHP redirect
The simplest PHP redirect script designed to run on Google App Engine
## Configuration
```
header("Location: 'url here'", true, 'http response code here');
```
Replace https://example.com to the domain of your choice in index.php
```
window.location.href = 'url here';
<meta http-equiv="refresh" content="0;URL='url here'" />
```
Replace both https://example.com to the domain of your choice in over_quata.html
Deploy
## What is over_quata.html?
over_quata.html is used when the instance is experiencing over quata.
When the instance is experiencing over quata, the php redirect will not work, so instead we use the html file to redirect.
