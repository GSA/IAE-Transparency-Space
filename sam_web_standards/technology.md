---
title: SAM Web Standards | Technology Considerations
layout: sam_web_standards
---
# Technology Considerations

The *SAM Web Standards* recommends and embraces the adoption of progressive enhancement, [^ProgressiveEnhancement1]<sup>,</sup> [^ProgressiveEnhancement2] whereby content (the data being consumed, transferred, and created) is considered first through semantic and accessible HTML, the style and interactions then utilize CSS whenever possible, with JavaScript being added as necessary.[^Section508]<sup>,</sup>[^w3cProgressiveEnhancement]

There are generally four major areas of code developed for the delivery of information over the Internet:

1. A server-side language.
2. The Hypertext Markup Language (HTML) itself for the display of content.
3. Cascading Style Sheets (CSS), which lets the browser know how to render HTML elements visually (color, size, and so on).
4. A client-side language (usually JavaScript)

When a user requests a URI, the server-side language (or framework) performs the duties of querying databases and preparing HTML content for the client.

HTML is the relatively static content interpreted by the browser for the display of content. Further, it plays the primary role in accessibility and assistive technologies; therefore, it should be well-formed (semantic) and as minimal as possible.

Cascading Style Sheets (CSS) are responsible for defining the aesthetic characteristics of the rendered page. Further, they play a secondary role in accessibility and assistive technologies. Finally, most modern browsers allow CSS to be used instead of JavaScript for things such as animations and device handling.

Client-side languages, which are executed on the user’s device. Client-side scripts can degrade battery life on mobile devices, exceed the limits of processor capabilities resulting in longer load times, or be disabled by the user altogether, which creates a poor experience. Therefore, client-side script capabilities should be created only once the core functionality and experience are complete.

## Bandwidth and Processor Speeds

The *SAM Web Standards* recommends a [mobile first]({{ site.baseurl }}/sam_web_standards/visual_style/#mobile-first) approach to design and development. As part of this recommendation it is important to consider bandwidth constraints, caps of data plans, and processor speeds. Therefore, it is recommended that the majority of processes be performed server-side while delivering the minimum data required to the client-side to update a user. Further, mobile and tablet devices typically have less processing power and hardware resources available, which should also be taken into consideration when creating client-side scripts.

## Secure by Default

There are two transfer protocols used to serve Web content: Hypertext Transfer Protocol (HTTP) and HTTP Secure (HTTPS). By default all uniform resource locators (URLs) should use HTTPS; an HTTP URL should redirect to the HTTPS equivalent.


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

This allows communication and marketing collateral to be built in a more human-readable manner by using upper- and lower-case letters to separate words within URLs while supporting copy and paste of the URL into a browser.

Further, when developing page addresses and URLs a user should be able to gain a basic understanding of what they will see, for example:

* https://domainname.com/mainpage/posts/descriptive-post-title
* not https://domainname.com/?page=1&post=5

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
*[URI]: Uniform Resource Indicator
*[URLs]: Uniform Resource Locators
*[AJAX]: Asynchronous JavaScript and eXtensible Markup Language
*[HTML]: Hypertext Markup Language