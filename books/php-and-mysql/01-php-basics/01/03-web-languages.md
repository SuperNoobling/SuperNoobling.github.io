---
layout: book-page
title: Web languages
book: Build dynamic websites with PHP & MySQL
type: section
---

When you create a web site, you'll need to deal with not one, but multiple languages. As a website administrator, mastering them is an absolute necessity.

Certain programs, called WYSIWYG (What You See Is What You Get), can help beginners create static web sites without knowing the programming languages that hide underneath… But to build a dynamic site, as we want to, we deﬁnitely need to get our hands dirty.

## HTML and CSS for static sites
Many languages have been create for building web sites. Two of these form the basis that all website administrators need to know.

### HTML
This is the basic language of web sites. It's easy to learn, and is based on tags. Here is an example of HTML code: 

{% highlight html %}
<p>Why hello there, I'm a fancy <em>paragraph</em>!</p>
{% endhighlight %}

### CSS
This is the styling language of web sites. HTML allows you to write the content of of your web pages and to structure them, and the CSS language takes care of the layout and design. You choose colours, sizes and more in CSS. Here is an example of CSS code: 

{% highlight css %}
.banner {
   text-align: center;
   font-weight: bold;
   font-size: 120%;
}
{% endhighlight %}

These languages are the basis of all web sites. When the server sends the web page to the client, it actually sends HTML and CSS code.

The problem is that when you only know HTML and CSS, you can only make static sites…not dynamic ones! For these, you have to use other languages as well as HTML and CSS.

So the main question is do you know HTML and CSS? If the answer is yes, then that's perfect, you can continue because you'll need it afterwards. If your response was no, don't panic. These languages aren't hard, they're accessible to everyone. You can learn them by following some tutorials on the internet (later on there will be a complete book for beginners about HTML and CSS on this web site). Learning these languages will only take a few weeks, less if you have enough free time.

## + PHP and MySQL for dynamic sites
Regardless of the web site you want to make, HTML and CSS are essential. But they're not enough for building dynamic sites. They need to be supplemented with other languages.

This is the goal of this book: you'll learn to use PHP and MySQL to build a dynamic web site.

### PHP
This is a language that only servers understant and makes your site dynamic. It's PHP that "generates" the web page as we saw in the previous illustrations.

This will be the ﬁrst language we learn about in this book. It can work alone, but it gets much more interesting when used with a tool like MySQL. Here is some PHP code:

{% highlight php %}
<?php 
echo "You are visitor n° " . $num_visitors; 
?>
{% endhighlight %}

### MySQL
This is what is called a DBMS (Database Management System). Put simply, its job is to save data in an organised manner to help you ﬁnd it easily later on. Thanks to MySQL you can save a list of members of your site, forum messages, etc. The language that lets you communicate with the database is called SQL. Here is some SQL code:

{% highlight sql %}
SELECT id, author, message, datemsg FROM guestbook ORDER BY datemsg DESC LIMIT 0, 10
{% endhighlight %}

PHP and MySQL are what's called open-source software. This garantees sustainability: everyone can contribute to their development, so you don't have to worry about web site developers losing interest in PHP an MySQL overnight, and that's very important!

Also, PHP and MySQL are available for free. This means that you won't need to pay a cent to build your web site!

PHP can work alone and is enough to make a dynamic site, but things get really interesting when you combine it with a database system such as MySQL. But to make things simple, let's forget MySQL for now and focus on PHP.


## PHP generates HTML
Clients can't understant PHP code: they only know HTML and CSS. Only the server can read PHP.

The role of PHP is precisely to generate HTML code (you can also generate CSS, but it's not as common), and this code is then sent to the client in the same way as a static site, as shown in the ﬁgure below.

<img class="figure-left" src="/assets/media/diagram-php-generation.gif" alt="Diagram of php generation" />

PHP is a programming language used on many servers for making decisions. PHP decides what HTML code will be generated and sent to the client each time

To understand the advantage of all this, let's look at an example. You can write in PHP: "If the visitor is a member of my site and is called Jonathan, display Welcome Jonathan on the web page. But if they're not a member of my site, display Welcome instead and suggest the visitor signs up."
This is a very basic example of a dynamic site: depending on whether you're a registered member or not, you won't see the same things and maybe won't have access to all the sections.
