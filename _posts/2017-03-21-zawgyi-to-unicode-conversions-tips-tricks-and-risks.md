---
layout: post
title: Zawgyi To Unicode Conversions Tips, Tricks and Risks
date: 2017-03-21 11:45
author: unicodeadmin
comments: true
categories: [Converter]
---
We are very familiar with Zawgyi too long. But now is the time to move, use 100% Unicode fonts. It is not very easy for every one, to convert all our - documents, files, web pages, blog posts and database - writing in Zawgyi to 100% Unicode character fonts (Myanmar3, Padauk, Parabaik etc). In this article, I will share my experience and conversion processes. This article is divided into two parts. One for normal users, whose without knowledge of - database and server management. The other one is for expert users, whose have database and server management experience.
<h2>A. Simple Conversion Method</h2>
In this method, we are going to convert post by post basic. The process is ...
<ol>
 	<li>Download <strong>KaNaungConverter_Window_Build200508.zip</strong> from the Kanaung project page and Unzip <a href="http://code.google.com/p/kanaung/downloads/list" target="_blank" rel="noopener noreferrer">http://code.google.com/p/kanaung/downloads/list</a></li>
 	<li>Run the <strong>KaNaung.exe</strong> and start the conversion for individual posts.</li>
 	<li>Re-Publish the posts.</li>
</ol>
In summary, this method is very easy. The only problem is - we need to use too much time. But it is very safe way. We don't need any expert knowledge in the conversion process. This method is suitable for most users.
<h2>B. Database Conversion Method</h2>
In this method, we are going to convert from the database level. The process is ...
<ol>
 	<li>Dump the table (e.g - <strong>posts</strong> table from a WordPress database, <strong>node_review</strong> table from a Drupal database) or the whole database in <strong>SQL, TXT</strong> or <strong>XML</strong> format.</li>
 	<li>Use one of the converter from the converter list below, to convert your file from Zawgyi to Unicode encoding.</li>
 	<li>Import back to the original table.</li>
</ol>
Look very easy, right? But there are some risks, problems and limitations in this method.
<h2>Problems &amp; Limitations with PHP Settings</h2>
The PHP settings of most shared hosting are difficult to change for every website owner. This is the major problem. By default the <strong>"max_input_time"</strong> and <strong>"max_execution_time"</strong> are about <strong>"60" seconds</strong> in <strong>php.ini</strong> file of most shared hostings. <em>If our database files are very large</em> and <em>the internet connection is too slow</em>, our import process is difficult to success.

<strong>Best Practise</strong>

In summary, this method is <strong>more faster</strong> than the first one. However we need
<ul>
 	<li><em>Database Knowledge</em></li>
 	<li><em>Faster Internet Connection</em></li>
 	<li><em>Changing the php.ini settings (if required)</em></li>
</ul>
. And also it is a <strong>High Risk Process</strong>.

<strong>As a best practise, you should try (or practise) more than three times in your local development environment (localhost/phpmyadmin) before you change anything on your live web server.</strong>
<h2>Unicode Converters</h2>
<ol>
 	<li>Kanaung Converter - <a href="http://code.google.com/p/kanaung/downloads/list" target="_blank" rel="noopener noreferrer">Download KaNaungConverter_Window_Build200508.zip</a></li>
 	<li>Myanmar NLP Unicode Converter - <a href="http://www.myanmarnlp.org.mm/index.php?option=com_content&amp;view=article&amp;id=2&amp;Itemid=5" target="_blank" rel="noopener noreferrer">Download Myanmar NLP Unicode Cnverter</a></li>
 	<li>ThanLwinSoft Converter<a href="http://thanlwinsoft.org/ThanLwinSoft/DocCharConvert/" target="_blank" rel="noopener noreferrer">Download ThanLwinSoft DocCharConvert-1.3.0.exe</a></li>
</ol>
Do you know other converters? Please give a comment for the download link. We will update the list later. Thank you for your support to the community.
<h2>We can Help &amp; Support</h2>
Still got problem? <strong>We are ready to help &amp; Support in your Unicode Conversion Process</strong>. Feel free to <a href="http://www.myanmarlanguage.org/contact">Contact us</a> or leave a comment. Want to know more useful tips (like this) easily and automatically? <a href="http://feeds.feedburner.com/mmlang" target="_blank" rel="noopener noreferrer">Subscribe</a> our <a href="http://feeds.feedburner.com/mmlang" target="_blank" rel="noopener noreferrer">RSS Feed</a>. Moreover, you also can <a href="http://feedburner.google.com/fb/a/mailverify?uri=mmlang&amp;loc=en_US" target="_blank" rel="noopener noreferrer">read from your email</a> too.

<strong>This is a cross post from mmshare.org. I just change the links and website names only.</strong>

Credit:<a href="http://www.myanmarlanguage.org/"><strong>myanmarlanguage.org</strong></a>
