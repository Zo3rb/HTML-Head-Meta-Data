# HTML-Head-Meta-Data
Important tags to add to standard HTML

## Meta Tags

Specify the character encoding for the HTML document
The charset attribute is new in HTML5, and replaces the need for something like: http-equiv="Content-Type" content="text/html; charset=UTF-8"
```
<meta charset="utf-8">
```


A meta viewport element gives the browser instructions on how to control the page's dimensions and scaling.

The width=device-width part sets the width of the page to follow the screen-width of the device (which will vary depending on the device).

The initial-scale=1.0 part sets the initial zoom level when the page is first loaded by the browser.
```
<meta name="viewport" content="width=device-width, initial-scale=1.0">
```


Force IE 8/9/10 to use its latest rendering engine (compatability)
```
<meta http-equiv="x-ua-compatible" content="ie=edge">
```


Short description of the document (ususally limit to 150 characters)
```
<meta name="description" content="A description of the page">
```


Theme Color for Chrome, Firefox OS and Opera (Android)
```
<meta name="theme-color" content="#4285f4">
```


Allow adding website to home screen as shortcut
```
<meta name="mobile-web-app-capable" content="yes">
```


## Open Graph Protocol 
http://ogp.me

The Open Graph protocol enables any web page to become a rich object in a social graph. For instance, this is used on Facebook to allow any web page to have the same functionality as any other object on Facebook.
```
<meta property="fb:app_id" content="123456789">
<meta property="og:url" content="http://example.com/page.html">
<meta property="og:type" content="website">
<meta property="og:title" content="Content Title">
<meta property="og:image" content="http://example.com/image.jpg">
<meta property="og:description" content="Description Here">
<meta property="og:site_name" content="Site Name">
<meta property="og:locale" content="en_US">
<meta property="article:author" content="">
```

## Optimizing with Twitter Cards 
https://developer.twitter.com/en/docs/tweets/optimize-with-cards/guides/getting-started

```
<meta name="twitter:card" content="summary">
<meta name="twitter:site" content="@site_account">
<meta name="twitter:creator" content="@individual_account">
<meta name="twitter:url" content="http://example.com/page.html">
<meta name="twitter:title" content="Content Title">
<meta name="twitter:description" content="Content description less than 200 characters">
<meta name="twitter:image" content="http://example.com/image.jpg">
```
