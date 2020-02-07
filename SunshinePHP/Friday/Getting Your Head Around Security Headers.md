# Getting Your Head Around (Security) Headers

Elisa Towbis

[@ElisaInFla](https://twitter.com/ElisaInFla)

[Joind link](https://joind.in/talk/05246)

## What is it and why do we care?

Request and Response Headers
* Things that travel along with requests to and from the server

Headers are set:
* Edge (Cloudflare, etc)
* Server (Apache, NGINX, etc)
* Code (PHP)
* HTML

Premise of layered defense.

### HSTS - HTTP Strict Transport Security

* Avoids Man in the Middle attacks during redirect
* Tells the browser to only connect to this site using HTTPS, even if HTTP was entered
* [Chromes preload list](https://hstspreload.org/)
* Easy to implement

### Subresource directory

* Integrity flag on img/script tags lets you include a hash of the file being pulled in
* Implemented at the HTML level which might be tricky

### X-Frame-Options

* Prevents clickjacking
* When your site can be included in a frame and when it can't
* Apache setting: Content-Security-Policy, X-Frame-Options

### X-Content-Type-Options

* Tells browsers not to load unless the server indicates the correct MIME type
* X-Content-Type-Options: "nosniff"

### Content Security Policy

CSP - Block Cross Site Security (XSS) Attack

* Exploit: Attacker injects script into your site

#### Countermeasures

* Whitelist Trusted Content
* Load only from a safe domain


Takeaways: Test on multiple browsers because they don't all implement these rules themselves

### Cookies

* Travel with each request as part of the header


Takeaways: Secure your stuff, yo.