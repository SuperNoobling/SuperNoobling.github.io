---
layout: book-page
title: How does a web site work?
book: Build dynamic websites with PHP & MySQL
type: section
---

When you visit a web site, you type the address in your browser, whether that's Mozilla Firefox, Internet Explorer, Opera, Safari, or another. But have you ever wondered how the web page gets to you?

The internet is a network of computers. These computers can be categorised into two groups:

## The clients
<img class="figure-left" src="http://openclipart.org/image/100px/svg_to_png/181693/telephone.png" alt=""> 
These are the computers of users like you. Your computer belongs to the client category. Every client represents a web site visitor. In the illustrations below, the client computer will be represented by this image.

## The servers
<img class="figure-right" src="http://openclipart.org/image/100px/svg_to_png/181695/telephone3.png" alt=""> 
These are powerful computers that store and serve web sites to users, or clients. Most internet users have never seen a server in their lives, but servers are essential to making the web work. In the illustrations below, a server will be represented by this image.

Most of the time, the server doesn't have a screen: it stays on and works all by itself without human intervention, 24/7 (a real work slave).

So your computer is called the client, and the computer that stores the web site is called the server. How do they communicate? This is exactly what makes the difference between a static and a dynamic web site. Let's see what changes:

## A static site
When a site is static, the diagram is very simple. There are two steps, as shown in the ﬁgure below:

<img class="figure-center" src="/assets/media/diagram-static-site.gif" alt="Diagram of a static site" />

1. The client asks the server for a web page.
2. The server responds by sending the web page called for.

The communication is pretty basic, and on a static site nothing else happens. The server stores the web pages and sends them to clients that ask for them, without modifying them.

## A dynamic site
When a site is dynamic, there's an intermediate step: the page is generated (see the ﬁgure below).

1. The client asks the server for a web page
2. The server prepares the page specially for the client
3. The server sends the page it's just generated

<img class="figure-center" src="/assets/media/diagram-dynamic-site.gif" alt="Diagram of a dynamic site" />

The web page is generated each time a client asks for it. This is exactly what makes dynamic sites dynamic: a page's content can change in an instant. This is how some sites are able to display, for example, your username on every page. As the server generates a page each time someone asks for it, the page can be personalised according to user preferences (and display usernames etc.).
