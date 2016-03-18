---
title: SAM Web Standards | Technology Considerations
layout: sam_web_standards
---
# Technology Considerations

The *SAM Web Standards* recommends and embraces the adoption of progressive enhancement, [^ProgressiveEnhancement1]<sup>,</sup> [^ProgressiveEnhancement2] whereby content (the data being consumed, tranferred, and created) is considered first through semantic and accessible HTML, the style and interactions then utilize CSS whenever possible, with JavaScript being added as necessary.[^Section508]<sup>,</sup>[^w3cProgressiveEnhancement]

There are generally four major areas of code developed for the delivery of information over the Internet:

1. A server-side language.
2. The Hypertext Markup Language (HTML) itself for the display of content.
3. Cascading Style Sheets (CSS), which lets the browser know how to render HTML elements visually (color, size, and so on).
4. A client-side language (usually JavaScript)



## Bandwidth and Processor Speeds

The *SAM Web Standards* recommends a [mobile first]({{ site.baseurl }}/sam_web_standards/visual_style/#mobile-first) approach to design and development. As part of this recommendation it is important to consider bandwidth constraints, caps of data plans, and process speeds. Therefore, it is recommended that the majority of processes be performed by the back-end while delivering the minimum data required to the front-end to update a user. Further, mobile and tablet devices typically have less processing power and harward resource availability, which should also be taken into consideration when creating client-side scripts.

## Secure by Default

There are two transfer protocols used to serve me Web content: Hypertext Transfer Protocol (HTTP) and HTTP Secure (HTTPS). By default all uniform resource locators (URLs) should use HTTPS; if possible, a non-HTTPS version should not be allowed.

URLs represent complete addresses for content and should be human-friendly. Two examples are below:

* https://domainname.com/service/mainpage/subpage
* not https://domainname.com/?id=2&main=8&sub=4

## No WWW

URLs should not require the use of “www”, as this represents a sub-domain and could lead to confusion if subdomains are implemented on the site. In other words, there is a question of whether the following are different sites or the same:

* https://www.my.domainname.com
* https://my.www.domainname.com
* https://my.domainname.com

## Human-Friendly and Readable

URLs should be case-*insensitive*; therefore, the following URL pairs should result in the display of the same content:

* https://My.DomainName.com and<br>https://my.domainname.com
* https://my.DomainName.com/MainPage/SubPage and<br>https://my.domainname.com/mainpage/subpage
* https://my.domainname.com/AFileOnTheServer.pdf and<br>https://my.domainname.com/afileontheserver.pdf

This allows communication collateral to be built in a more human-readable manner by using upper- and lower-case letters to separate words within URLs while simultaneously allowing direct copy and paste of the URL into a browser.

Further, when developing page addresses and URLs a user should be able to gain a basic understanding of what they will see, for example:

* https://domainname.com/mainpage/posts/descriptive-post-title
* as opposed to https://domainname.com/?page=1&post=5

[^Section508]: [Quick Reference Guide to Section 508 Requirements and Standards 1194.22 (l)](http://www.section508.gov/content/learn/standards/quick-reference-guide#1194.22l)
[^w3cProgressiveEnhancement]: [World Wide Web Consortium - Graceful degradation versus progressive enhancement](https://www.w3.org/wiki/Graceful_degradation_versus_progressive_enhancement)
[^AddressNames]: While there are some differences in the details of these terms, for the most part, they can be used interchangibly: URL, URI, Address, Path, Route, and others.
[^ProgressiveEnhancement1]: [Understanding Progressive Enhancement: A List Apart](http://alistapart.com/article/understandingprogressiveenhancement)
[^ProgressiveEnhancement2]: [Progressive Enhancement: Wikipedia](https://en.wikipedia.org/wiki/Progressive_enhancement)

*[SAM]: System for Award Management
*[IAE]: Integrated Award Environment
*[API]: Application Program Interface
*[APIs]: Application Program Interfaces
*[HTTP]: Hypertext Transfer Protocol
*[HTTPS]: Hypertext Transfer Protocol Secure
*[URL]: Uniform Resource Locator
*[URLs]: Uniform Resource Locators
*[AJAX]: Asynchronous JavaScript and eXtensible Markup Language
*[HTML]: Hypertext Markup Language