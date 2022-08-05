# Quick-Responsive-Web-Applications-HTML   
>How to quickly edit your index.html to turn it into a fully responsive web application that can be used without installing, the user just needs to add your webpage to the home screen and they have a instant application from your website.
    
### Step 1, Update Your Meta Tags. 
```
<!--  set viewport -->
  <meta http-equiv="X-UA-Compatible" content="IE=edge">
  <meta name="viewport" content="width=device-width, initial-scale=1, minimum-scale=1">

<!-- set info links for social media posts  -->
  <meta property="og:title" content="WickedApp"/>
  <meta property="og:url" content="http://wicked.app"/>
  <meta property="og:site_name" content="WickedApp"/>
  <meta property="og:image" content="http://wicked.app/post_image.jpg"/>
  <meta property="og:video" content="https://www.youtube.com/v/oHYWb-N5Aok"/>
  <meta property="og:type" content="document"/>
  <meta property="og:description" content="You can not define me with words."/>
  <link rel="shortcut icon" href="images/logo.png" type="image/x-icon">

<!-- set regular html info -->
  <meta name="description" content="You can not define me with words.">
  <title>WickedApp</title>

<!-- link App manifest file to tell the browser we are an application not a webpage. -->
  <link rel="manifest" href="/manifest.json">
 
<!-- Show we are capable of being a Web Application to the browser -->
  <meta name="apple-mobile-web-app-capable" content="yes">
  <meta name="mobile-web-app-capable" content="yes">

<!-- Set the Web App information -- >
   <meta name="apple-mobile-web-app-title" content="WickedApp">
   <meta name="mobile-web-app-title" content="WickedApp">
   <meta name="description" content="WickedApp can not be defined by words.">
```
   
### Step 2, Create your manifest file you defined above.    
> manifest.json
```
{
  "short_name": "Wicked",
  "name": "WickedApp",
  "icons": [
    {
      "src": "/assets/images/icon.png",
      "type": "image/png",
      "sizes": "192x192"
    },
    {
      "src": "/assets/images/icon.png",
      "type": "image/png",
      "sizes": "512x512"
    }
  ],
  "start_url": "/example/app/path/index.html",
  "background_color": "#3367D6",
  "display": "standalone",
  "scope": "/examples/app/path/",
  "theme_color": "#3367D6"
}
``` 
 
### Step 3, Enable HTTPS and SSL, web apps require SSL 
