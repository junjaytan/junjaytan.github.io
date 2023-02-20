---
layout: post
published: false
---

Things I learned porting my wordpress site to jekyll.

* so much less bloat.
* transferring posts is a pain.
  * I ended up manually porting each page. Also, wordpress has some nice image resizing features, which jekyll doesn't.
* Adding analytics is easy.
* Using gem installation was difficult for replicating a custom index page with the blog as a subpage.
* You lose some nice features of wordpress themes, like searching through posts and category widgets.
* Importing the wordpress export directly into disqus fails because the jekyll pages end with `.html`. So I had to replace the non-html extension links with .html
  * e.g.,: `http://junjaytan.com/blog/python-data-cleaning-people-contact-data` to `http://junjaytan.com/blog/python-data-cleaning-people-contact-data.html`