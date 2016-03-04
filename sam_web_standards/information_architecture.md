---
title: SAM Web Standards | Information Architecture
layout: sam_web_standards
---

# Information Architecture

There are two primary ways for a front-end user to find information. The first is through links from one page to another. The second is by searching for content and following links within those results. 

When a front-end user is looking for high-level or general information, the front-end user should be able to navigate the site quickly via static menus. The front-end user may not know exactly where to go or what (s)he is looking for; the architecture can help guide the front-end user by starting broad (categories) and becoming more detailed (a specific notice, wage determination, program, and so on).

When a front-end user knows the information (s)he is looking for, search becomes the better; therefore, front-end users should be allowed to search using text with additional filtering capabilities within a given category.

## Navigation

Information Architecture, in terms of navigation, refers to the layout and depth of pages within a website. The *SAM Web Standards* recognizes four levels of navigation for page-related content.

1. **Main Navigation:** Contained within the header and footer components and is used to navigate between system-wide pages (the Legal page, for example) and between categories within the system (Wages, for example). From a front-end user perspective, this results in a change from transition.SAM.gov to something like transition.SAM.gov/wages.
2. **Category Navigation:** Appended to the header area and provides navigation within a category; thereby, allowing each category to have primary pages (“Due to Be Revised” within Wages, for example). Resulting in something like transition.SAM.gov/wages/to-be-revised.
3. **Sidebar Navigation (up to three levels):** Navigation appearing in a vertical sidebar along the left side of pages using the element from the *US Web Standards*. This type of navigation should be avoided, if possible or practical. Further, if possible, only one level of navigation will make it easier to navigate.

## Content

Information Architecture, in terms of content, refers to how content is displayed. This could be the ordering of information within a block of content (chapters within a book, paragraphs within a chapter, sentences within a paragraph, and so on) or how blocks of content are arranged within a page (books in a library).

For the purposes of the *SAM Web Standards* we recognize two primary types of content from a front-end user perspective: content and metadata. Content refers to titles of pages, body copy, attachments, and so on. Metadata refers to details related to *that* content; posting date, related category, and so on.

Grouping content and metadata separately allows me to quickly discern the *content* of a page from the information *about* the content of a page depending on which I, as a front-end user, am interested in. Further, content and metadata should also be ordered, as much as possible, in a way that gives me what I am mostly likely concerned about first, with the details later. For reference, see the Inverted Pyramid from the profession of journalism.

## Content-focused and printable

For content pages (as opposed to those designed as portals or navigation purposes), the text-based content should not be overpowered by the surrounding navigation or branding (chrome). Normal operating distance from the screen should also be considered. To allow users the ability to adjust font sizes using their browser, front-end developers and designers should use relative font sizing (ems) and not stipulate font sizes less than one em. Increased leading (the space between lines) makes it easier for readers to discern one line of text from the next.

On any given page, I should be to print (or print to file) the content of that page and receive a well-formed (readable) document, without chrome elements. Print stylesheets can be used to facilitate this outcome by hiding the navigation elements, sidebars, footers (except copyright information if applicable), and so on. Further, the size of the printed page is usually unknown; therefore, it is important to remove (or override) any fixed width information and replace it with a percentage (usually 100%).

Note: Printing a page should only include content considered public unless you add proper document handling, marking and labeling in accordance with Federal regulations.

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