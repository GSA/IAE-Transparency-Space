---
title: SAM Web Standards | Information Architecture
layout: sam_web_standards
---

# Information Architecture

There are two primary ways for a front-end user to find information. The first is through links from one page to another. The second is by searching for content and following links within those results. 

When a front-end user is looking for high-level or general information, the front-end user should be able to navigate the site quickly via static menus. The front-end user may not know exactly where to go or what (s)he is looking for; the architecture can help guide the front-end user by starting broad (categories) and becoming more detailed (a specific notice, wage determination, program, and so on).

When a front-end user knows the information (s)he is looking for, search becomes the better option; therefore, front-end users should be allowed to search using text with additional filtering capabilities within a given category.

## Navigation

Information Architecture, in terms of navigation, refers to the layout and depth of pages within a website. The *SAM Web Standards* recognizes three types of navigation, resulting in five levels of navigation for page-related content.

1. **Main Navigation:** Contained within the [header](http://gsa.github.io/openIAE/sam_web_standards/components/#header) and [footer](http://gsa.github.io/openIAE/sam_web_standards/components/#footer) components, available on the majority (all) of the pages. From a front-end user perspective, this results in a change from transition.SAM.gov to something like transition.SAM.gov/wages or transition.SAM.gov/about/legal.
2. **Category Navigation:** Appended to the header area and provides navigation within a primary are of the site (transition.SAM.gov/systeminformaiton); thereby, allowing each primary page to have sub-pages (“Due to Be Revised” within Wages, for example).
3. **Side Navigation (up to three levels):** Navigation appearing in a vertical sidebar along the left side of pages using the [Side Navigation](https://playbook.cio.gov/designstandards/sidenav/) component from the *US Web Standards*. This type of navigation should be avoided, if possible or practical. Further, if possible, only one level of navigation will make it easier for a front-end user to navigate.

## Content

Information Architecture, in terms of content, refers to how content is displayed. This could be the ordering of information within a block of content (chapters within a book, paragraphs within a chapter, sentences within a paragraph, and so on) or how sections of content are arranged within a page.

For the purposes of the *SAM Web Standards* we recognize two primary types of content from a front-end user perspective: content and metadata. Content refers to titles of pages, body copy, attachments, and so on. Metadata refers to details related to *that* content; posting date, related category, and so on.

Grouping content and metadata separately allows you to quickly discern the *content* of a page from the information *about* the content of a page. Further, content and metadata should be ordered, as much as possible, in a way that gives you what you are most likely concerned about first, with the details later. For reference, see the Inverted Pyramid[^InvertedPyramid] from journalism.

## Content-focused and printable

For content pages (as opposed to those designed as portals or navigation), the text-based content should not be overpowered by the surrounding navigation or branding (chrome). Normal operating distance from the screen should be considered (mobile versus tablet, versus lap- or desk-top). 

To allow users the ability to adjust font sizes using their browser, front-end developers and designers should use relative font sizing. Increased leading (the space between lines) makes it easier for readers to discern one line of text from the next.

On any given page, you should be able to print (or print to file) the content of that page and receive a well-formed (readable) document, without chrome elements. Print stylesheets can be used to facilitate this outcome by hiding the navigation elements, sidebars, footers (except copyright information if applicable), and so on. Further, the size of the printed page is usually unknown; therefore, it is important to remove (or override) any fixed width information and replace it with a percentage (usually 100%).

Note: Printing a page should only include content considered public unless you add proper document handling, marking and labeling in accordance with Federal regulations.

[^InvertedPyramid]: [Wikipedia - Inverted Pyramid](https://en.wikipedia.org/wiki/Inverted_pyramid)

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