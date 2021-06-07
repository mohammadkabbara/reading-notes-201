# INTRODUCING HTML5 STORAGE

So what is HTML5 Storage? Simply put, it’s a way for web pages to store named key/value pairs locally, within the client web browser. Like cookies, this data persists even after you navigate away from the web site, close your browser tab, exit your browser, or what have you. Unlike cookies, this data is never transmitted to the remote web server (unless you go out of your way to send it manually). Unlike all previous attempts at providing persistent local storage, it is implemented natively in web browsers, so it is available even when third-party browser plugins are not.


# LOCAL STORAGE

HTML5 storage provides a way for web sites to store information on your computer and retrieve it later. The concept is similar to cookies, but it’s designed for larger quantities of information. Cookies are limited in size, and your browser sends them back to the web server every time it requests a new page (which takes extra time and precious bandwidth). HTML5 storage stays on your computer, and web sites can access it with JavaScript after the page is loaded.

# WEB WORKERS

Web Workers provide a standard way for browsers to run JavaScript in the background. With web workers, you can spawn multiple “threads” that all run at the same time, more or less. (Think of how your computer can run multiple applications at the same time, and you’re most of the way there.) These “background threads” can do complex mathematical calculations, make network requests, or access local storage while the main web page responds to the user scrolling, clicking, or typing.

# OFFLINE WEB APPLICATIONS

Reading static web pages offline is easy: connect to the Internet, load a web page, disconnect from the Internet, drive to a secluded cabin, and read the web page at your leisure. (To save time, you may wish to skip the step about the cabin.) But what about web applications like Gmail or Google Docs? Thanks to HTML5, anyone (not just Google!) can build a web application that works offline.

---

*Offline web applications start out as online web applications. The first time you visit an offline-enabled web site, the web server tells your browser which files it needs in order to work offline. These files can be anything — HTML, JavaScript, images, even videos. Once your browser downloads all the necessary files, you can revisit the web site even if you’re not connected to the Internet. Your browser will notice that you’re offline and use the files it has already downloaded. When you get back online, any changes you’ve made can be uploaded to the remote web server.*

# GEOLOCATION

Geolocation is the art of figuring out where you are in the world and (optionally) sharing that information with people you trust. There is more than one way to figure out where you are — your IP address, your wireless network connection, which cell tower your phone is talking to, or dedicated GPS hardware that calculates latitude and longitude from information sent by satellites in the sky.


# MICRODATA

Microdata is a standardized way to provide additional semantics in your web pages. For example, you can use microdata to declare that a photograph is available under a specific Creative Commons license.

*The HTML5 microdata standard includes both HTML markup (primarily for search engines) and a set of DOM functions (primarily for browsers). There’s no harm in including microdata markup in your web pages.*

# USING HTML5 STORAGE

HTML5 Storage is based on named key/value pairs. You store data based on a named key, then you can retrieve that data with the same key. The named key is a string. The data can be any type supported by JavaScript, including strings, Booleans, integers, or floats. However, the data is actually stored as a string.

