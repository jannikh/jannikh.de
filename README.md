# jannikh.de
This is the open-source repository for [jannikh.de](https://jannikh.de), hosted directly by [github pages](https://pages.github.com/).

The websites in this repository serve to redirect all traffic from the domain jannikh.de towards [jannikh.com](https://jannikh.com), including a 404 redirect that keeps the rest of the URL path intact.

---

## Files in this repository
### CNAME file
***[CNAME](CNAME)*** contains the domain names that host this website, detected by github pages to seamlessly host the site.

### Landing page for jannikh.de
***[index.html](index.html)*** redirects all traffic that lands on this page towards the homepage of [jannikh.com](https://jannikh.com).

This takes place in three redundant ways:
1. a meta-redirect statement in the header, executed immediately thus taking precedence
1. a javascript window-location change
1. a manual link in the body in case the other options fail

### 404 page
***[404.html](404.html)*** automatically redirects any traffic that lands on any other page of this domain towards [jannikh.com](https://jannikh.com), attempting to keep the rest of the URL intact, thus avoiding going back to the homepage if the user typed an otherwise intact URL.

This redirect happens in three redundant ways:
1. a javascript window-location change that only replaces the domain
1. a meta-redirect statement in the header in case javascript is disabled, delayed by one second in order to allow the javascript redirect to take precedence
1. a manual link in the body in case the other options fail

However, if the redirected URL does not exist on jannikh.com either, the user will end up on the [404 page of jannikh.com](https://jannikh.com/404)

---

## Redirecting to a German version of jannikh.com
Redirecting towards specific German translations of the website and all its subpages is a future goal, which will be tackled after the main development of [jannikh.com](https://jannikh.com) in English is finished.

See also: [repository of jannikh.com](https://github.com/jannikh/jannikh.com/)
