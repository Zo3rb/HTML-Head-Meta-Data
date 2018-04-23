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

Disables Pinch & Zoom on Mobile Devices
```
<meta name="viewport" content="width=device-width, initial-scale=1, maximum-scale=1, user-scalable=0">
```


The description of the document (ususally limit to 150 characters). The description meta tag provides a short description of the page. In some situations this description is used as a part of the snippet shown in the search results.
```
<meta name="description" content="A description of the page">
```

## Open Graph Protocol 
http://ogp.me

Most content is shared to Facebook as a URL, so it's important that you mark up your website with Open Graph tags to take control over how your content appears on Facebook.

Without these tags, the Facebook Crawler uses internal heuristics to make a best guess about the title, description, and preview image for your content. Designate this info explicitly with Open Graph tags to ensure the highest quality posts on Facebook.

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

With Twitter Cards, you can attach rich photos, videos and media experiences to Tweets, helping to drive traffic to your website. Simply add a few lines of markup to your webpage, and users who Tweet links to your content will have a “Card” added to the Tweet that’s visible to their followers.

```
<meta name="twitter:card" content="summary">
<meta name="twitter:site" content="@site_account">
<meta name="twitter:creator" content="@individual_account">
<meta name="twitter:url" content="http://example.com/page.html">
<meta name="twitter:title" content="Content Title">
<meta name="twitter:description" content="Content description less than 200 characters">
<meta name="twitter:image" content="http://example.com/image.jpg">
```

## Apple/iOS 

https://developer.apple.com/library/content/documentation/AppleApplications/Reference/SafariHTMLRef/Articles/MetaTags.html

Sets whether a web application runs in full-screen mode

```
<meta name="apple-mobile-web-app-capable" content="yes">
```

On iOS, similar to native applications, you can specify a launch screen image that is displayed while your web application launches. This is especially useful when your web application is offline. By default, a screenshot of the web application the last time it was launched is used. To set another startup image, add a link element to the webpage, as in:

```
<link rel="apple-touch-startup-image" href="/launch.png">
```

On iOS, you can specify a web application title for the launch icon. By default, the <title> tag is used. To set a different title, add a meta tag to the webpage, as in:

```
<meta name="apple-mobile-web-app-title" content="AppTitle">
```

Enable standalone (full-screen) mode
```
<meta name="apple-mobile-web-app-capable" content="yes">
```

Status bar appearance (has no effect unless standalone mode is enabled) 
```
<meta name="apple-mobile-web-app-status-bar-style" content="black">
```

If you want to disable the automatic detection and formatting of possible phone numbers in Safari on iOS, use:
```
<meta name="format-detection" content="telephone=no">
```


## Android

Android Chrome, FireFox and Opera theme color. Currently, the theme-color meta extension is supported by Chrome 39+ for Android Lollipop. The content attribute extension can take any valid CSS color.
```
<meta name="theme-color" content="#E64545">
```

Allow app shortcut on Home Screen
```
<meta name="mobile-web-app-capable" content="yes">
```


## Microsoft Internet Explorer
Internet Explorer 8/9/10 support document compatibility modes that affect the way webpages are interpreted and displayed. Because of this, even if your site's visitor is using, let's say, Internet Explorer 9, it's possible that IE will not use the latest rendering engine, and instead, decide to render your page using the Internet Explorer 5.5 rendering engine.
```
<meta http-equiv="x-ua-compatible" content="ie=edge">
```
This will force Internet Explorer 8/9/10 to render the webpage in the highest available mode in the various cases when it may not, and therefore, ensure that anyone browsing your site is treated to the best possible user experience that browser can offer.


## Miscellaneous

If you want to disable the translation prompt in Chrome or block Google Translate from translating your web page, use:
```
<meta name="google" value="notranslate">
```
