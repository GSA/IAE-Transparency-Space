# SAM Web Standards v1.2

* [Getting Started](http://gsaiae.confluence.micropaas.io:8090/pages/viewpage.action?title=SAM+Web+Standards&spaceKey=UX#SAMWebStandards-gettingstarted)
  * Users and Technology Layers
  * Front-End User
    * Secure by default, human-friendly, and no WWW
    * Content-focused and printable
    * Navigation, search, and information architecture
  * Front-End Developer
    * Connection and processor speeds
    * Pages, content, and other elements
    * Web technologies
* Use US Web Design Standards For...
* Visual Style
  * Colors
  * Logo & Usage
  * Imagery
  * Animation
* Form Templates
  * Application Filter
* Header
  * Application Navigation
* Footer
* Pagination
* Page Templates
  * Defaults

# Getting Started

The *SAM Web Standards* are developed primarily for Front-End Developers; however, the information provided can be used to inform all user levels identified. The *SAM Web Standards* defines principles and practices that help developers, designers, and users of the SAM platform and services. These guidelines inherit from multiple private and Federal resources including, but not limited to:

* **Design and development:**
  * *US Web Design Standards* (<https://playbook.cio.gov/designstandards/getting-started/>),
  * The U.S. Digital Services Playbook (<https://playbook.cio.gov>),
  * Usability Starter Kit (<http://www.digitalgov.gov/resources/digitalgov-user-experience-program/digitalgov-user-experience-program-usability-starter-kit/>),
  * *GSA Government-wide Section 508 Accessibility Program* (<http://www.section508.gov>), and
  * The Research-Based Web Design & Usability Guidelines, Enlarged/Expanded edition (<http://guidelines.usability.gov>).* **Writing and language:**
  * *The Chicago Manual of Style* (<http://www.chicagomanualofstyle.org/home.html>),
  * *The U.S. Government Printing Office Style Manual* (<http://www.gpo.gov/fdsys/pkg/GPO-STYLEMANUAL-2008/content-detail.html>),
  * *The Federal Plain Language Guide* (<http://www.plainlanguage.gov/howto/guidelines/FederalPLGuidelines/FederalPLGuidelines.pdf>), and
  * *The 18f Content Guide* (<https://18f.gsa.gov/2015/07/06/18f-content-guide/>).
  
NOTE: If your question is not answered directly within the *SAM Web Standards*, refer to the aforementioned resources. If your question is not answered in the aforementioned resources, either use your professional judgment or contact the IAE User Experience Team.

## Users and Technology Layers

| System | Layer | transition.SAM.gov |
| ------ | ----- | ------------------ |
| System Front-End User | ![Presentation](http://gsaiae.confluence.micropaas.io:8090/download/thumbnails/6722902/HIG-Graphics.png?version=1&modificationDate=1436361553625&api=v2) Presentation| transition.SAM.gov Front-End-User |

The *SAM Web Standards* identifies the following user types (not to be confused with personae established for transition.SAM.gov):

* Front-end user: An individual using the Website
* Front-end developer: A developer who is responsible for creating code to display the front-end to front-end users
* Middleware developer: A developer who is responsible for creating code that acts as a bridge between the front-end presentation and back-end data layers
* Back-end developer: A developer who is responsible for creating data architectures and relationships to be accessed via APIs.

Each user type may be modified for further definition and clarification of scope:

* transition.SAM.gov:  A user or developer who interacts with pages or code classified as part of transition.SAM.gov common services.
* System: A user or developer who interacts with pages or code used strictly by a system to be subsumed by transition.SAM.gov.

The *SAM Web Standards* recognizes the following states for front-end users and developers:

* Unauthenticated: A user who has NOT signed in to the site via the sign in process.
* Authenticated: A user who has signed in to the via the registration and sign in process.

The *SAM Web Standards* identifies the following technology layers to describe the human-computer interaction of transition.SAM.gov:

* Presentation: Represents the final rendered page in a browser
* Markup: Refers to all markup and code downloaded to (or run on) the user’s computer (client-side) to render (or update) the page in a browser
* Middleware: Refers to code acting as a bridge between the markup and data layers; further, this layer may refer to server-side code used in calculating, preparing, or returning information
* Data: Refers to all individual files, database tables and database records stored for retrieval by the interface layer.

Each user type can be modified to distinguish between system personnel. Further, each type can be directly associated with a technology layer. Finally, it is important to note that the fidelity and validity of each layer are dependent on the preceding layer.  EXAMPLE: if the data layer does not house the proper information in the proper format, the middleware layer loses fidelity and validity, and so on.

## Front-End User

This section is written from the perspective of a front-end user, i.e., someone wanting to view and interact with the content of the site.

### Secure by default, human-friendly, and no www

There are two transfer protocols used to serve me Web content: Hypertext Transfer Protocol (HTTP) and HTTP Secure (HTTPS). By default all uniform resource locators (URLs) should use HTTPS; if possible, a non-HTTPS version should not be allowed.1

URLs represent complete addresses for content and should be human-friendly.  Two examples are below:

* https://domainname.com/service/mainpage/subpage
* https://domainname.com/?id=2&main=8&sub=4

URLs should not require the use of “www”, as this represents a sub-domain and could lead to confusion if subdomains are implemented on the site. In other words, there is a question of whether the following are different sites or the same:

* https://www.my.domainname.com
* https://my.www.domainname.com
* https://my.domainname.com

URLs should be case-insensitive; therefore, the following URL pairs should result in the display of the same content:

* https://My.DomainName.com and https://my.domainname.com
* https://my.DomainName.com/MainPage/SubPage and https://my.domainname.com/mainpage/subpage
* https://my.domainname.com/AFileOnTheServer.pdf and https://my.domainname.com/afileontheserver.pdf

This allows communication collateral to be built in a more human-readable manner by using upper- and lower-case letters to separate words within URLs while simultaneously allowing direct copy and paste of the URL into a browser.

### Content-focused and printable

For content pages (as opposed to those designed as portals or navigation purposes), the text-based content should not be overpowered by the surrounding navigation or branding (chrome). Normal operating distance from the screen should also be considered. To allow users the ability to adjust font sizes using their browser, front-end developers and designers should use relative font sizing (ems) and not stipulate font sizes less than one em. Increased leading (the space between lines) makes it easier for readers to discern one line of text from the next.

On any given page, I should be to print (or print to file) the content of that page and receive a well-formed (readable) document, without chrome elements. Print stylesheets can be used to facilitate this outcome by hiding the navigation elements, sidebars, footers (except copyright information if applicable), and so on. Further, the size of the printed page is usually unknown; therefore, it is important to remove (or override) any fixed width information and replace it with a percentage (usually 100%).

Note: Printing a page should only include content considered public unless you add proper document handling, marking and labeling in accordance with Federal regulations.

### Navigation, search, and information architecture

There are two major ways for me to find the content I am looking for. The first is through following links from one page to the next. The second is by searching for content and following links in those results. 

When I am looking for high-level or general information, I should be able to navigate the site quickly through the use of static menus. If I am using the navigation, I may not know exactly where I am going, and the architecture of the site can help guide me to where I want to be—getting increasingly detailed the further I go.

When I am looking for a specific piece of information, I want more control. When I search, I want the ability either to filter the results by service or to bring up an advanced search for a specific service.

## Front-End Developer

### Connection and Processor Speeds

As the Internet becomes more ubiquitous across multiple platforms and devices, it is important to allow for various display sizes, download speeds (bandwidth) and processing capabilities. As such, it is important to create layouts that adjust and change content as the display width of the screen changes; height is not considered, as scrolling vertically can be of any length. Further, whenever possible, processing should be performed on the server before the content is downloaded by the user’s device (server-side) as opposed to performing complex calculations on the device (client-side) using technologies such as JavaScript.

### Pages, Content, and Other Elements

A Web page is made up of three primary components: URL, page title and content. Without a URL, I can not get to a specific page. Page titles, while optional, help me orient myself within the overall environment. Content can be described as related text, images or other data conveying a topic of interest; therefore, site navigation, footer text, and so on (chrome) are not generally considered content. 

Having said that, chrome elements are considered part of the page. transition.SAM.gov supports unauthenticated (public), authenticated (requires login; private) and mixed pages, content and elements:

* Public pages, content and other elements are visible by front-end users at all times
* Private pages, content and other elements are not delivered by the system to front-end users unless logged in. Put another way, links to pages or the content of a page requiring authentication should not be contained within the hypertext markup language (HTML) of the served page
* By extension, a page containing both types of content and elements displays the public content to all front-end users and both the public and private content to logged in front-end users.

### Web Technologies

The server-side language performs the duties of querying the database(s) and preparing HTML content for the user’s device (client). Because the hardware capabilities are managed by transition.SAM.gov, it is recommended that the server-side language be used as much as possible for processing as much information as possible.

HTML is the relatively static content interpreted by the browser for the display of content. Further, it plays the primary role in accessibility and assistive technologies; therefore, it should be well-formed and as minimal as possible (see Accessibility).

Cascading Style Sheets (CSS) are responsible for defining the aesthetic characteristics of the rendered page. Further, they play a secondary role in accessibility and assistive technologies. Finally, most modern browsers allow CSS to be used instead of JavaScript for things such as animations and device handling.  It is recommended that CSS be leveraged whenever possible.

JavaScript is a client-side language, which means the code is executed and processed by the user’s device. JavaScript can degrade battery life on mobile devices, exceed the limits of processor capabilities resulting in longer load times, or be disabled by the user altogether, which creates a poor experience. JavaScript use should, therefore, be limited to those functions that could not be achieved by other means. Examples include Asynchronous JavaScript and eXtensible Markup Language (AJAX) executions and/or HTML insertions; however, the use of JavaScript should not be required for the navigation of the site.

## Use US Web Design Standards for...

For the following the SAM Web Standards do not modify the US Web Standards:

* typography (<https://playbook.cio.gov/designstandards/visual-style/#typography>),
  * NOTE: use the ____________ typeface pairing
* grid (https://playbook.cio.gov/designstandards/grids/),
buttons (<https://playbook.cio.gov/designstandards/buttons/>),
* labels (<https://playbook.cio.gov/designstandards/labels/>),
* tables (<https://playbook.cio.gov/designstandards/tables/>),
* alerts (<https://playbook.cio.gov/designstandards/alerts/>),
* accordions (<https://playbook.cio.gov/designstandards/accordions/>),
* form controls (<https://playbook.cio.gov/designstandards/form-controls/>),
* colors (<https://playbook.cio.gov/designstandards/visual-style/#colors>),
* search bar (<https://playbook.cio.gov/designstandards/search-bar/>), and 
* side navigation (<https://playbook.cio.gov/designstandards/sidenav/>).

# Visual Style

## Logo & Usage (need approval for public posting)

\\[logo pages from branding style guide]

## Imagery

You have the ability to surf the Internet on multiple devices, with multiple resolutions (low, medium, high, extra high, and so on), and the ability to make the browser almost any size you want. It is disappointing when a site dictates how you should use it or when the graphics are fuzzy because they are not accounting for the resolution capabilities of my display.

* Use Scalable Vector Graphics (SVG) when possible, especially flat artwork
* Use Portable Network Graphics (PNG) for flat artwork, images with transparency, or photographs
* Create and save images at 100 pixels per inch and two times the rendered dimensions; this does not apply to SVG
* Avoid imagery not directly related to the content being presented
* Avoid clip art style images.

\\[text and examples of image types and usage]

## Animation

The Internet, as a platform, has come a very long way in a very short time, relatively speaking. The modern Web holds few boundaries when it comes to what can be accomplished; however, just because something can be done, does not mean it should be done.

Gratuitous animations that do not contribute to user feedback and goals become annoying, causing a speed bump. Animated graphics (or static imagery) that does not aid the communication of the content are distracting and make it difficult to navigate the site. The Web, generally speaking, is a silent world.  Sound (even as part of a video) should be optional.

For each page you should ask yourself, "What is the primary purpose of this page? What is the secondary purpose? What are the tertiary purposes? What is here that gets in the way of those purposes?"

# Form Templates

See the *US Web Design Standards* for form templates related to name, address, sign-in, and password reset (<https://playbook.cio.gov/designstandards/form-controls/>).

## Application Filter

Used on pages where content spans multiple applications wherein a front-end user may wish to include or exclude any of the content related to the applications.

![Application Filter](http://gsaiae.confluence.micropaas.io:8090/download/attachments/6722902/UI%20Component%20-%20Simple%20-%20Services%20Filter.png?version=1&modificationDate=1440527728977&api=v2)
\\[Application Filter Image]

# Header

The header consists of the branded home button, main navigation, and application navigation elements (only when within an application). The branded home button consists of the [transition.SAM.gov](https://transition.SAM.gov/) logo with a link to <https://transition.SAM.gov/> allowing users to go to <https://transition.SAM.gov> from anywhere within the site.

\\[Unauthenticated variation]

\\[Authenticated variation]

## Application Navigation

The application navigation allows each service to create pages within the application's area within [transition.SAM.gov](https://transition.SAM.gov/). For example, <https://transition.SAM.gov/wages/resources> would be a page consisting of links to resources related to Wage Determinations and available within the Application Navigation element when a user is anywhere within <https://transition.SAM.gov/wages>.

\\[representation of navigation]

# Footer

The *SAM Web Standards* uses the "big footer" defined by the *US Web Design Standards* as a base.

\\[representation of footer]

# Pagination

The pagination element is used in circumstances where the content being displayed within a site area that cannot be fit on one page (search results, for example). If JavaScript is enabled, continuous scrolling methods can be used in place of the pagination element; however, this element should exist in case JavaScript is disabled.![Pagination](http://gsaiae.confluence.micropaas.io:8090/download/thumbnails/6722902/UI%20Component%20-%20Simple%20-%20Pagination.png?version=1&modificationDate=1440526726366&api=v2)
\\[pagination]

## Widgets

The *SAM Web Standards* uses the X standard [link to reference](http://gsaiae.confluence.micropaas.io:8090/pages/createpage.action?spaceKey=UX&title=link+to+reference&linkCreation=true&fromPageId=6722902) ."Widgets are an essential aspect of home screen customization. You can imagine them as "at-a-glance" views of an app's most important data and functionality that is accessible right from the user's home screen."

## Confirming and Acknowledging

The SAM Web Standards uses ...TBD.

Confirming is asking the user to verify that they truly want to proceed with an action they just invoked. In some cases, the confirmation is presented along with a warning or critical information related to the action that they need to consider.

\\[representation of Confirming]

Acknowledging is displaying text to let the user know that the action they just invoked has been completed. This removes uncertainty about implicit operations that the system is taking. In some cases, the acknowledgment is presented along with an option to undo the action.

\\[representation of Acknowledging]

## Icons

The application of standard icons follows the guidance of Font Awesome. <https://fortawesome.github.io/Font-Awesome/icons/>

\\[representation of common icons such as 'share' or 'new']

# Page Templates

## Default

# Use 18F Content Guide for...

For the following the *SAM Web Standards* follow the 18F Content Guidance <https://pages.18f.gov/content-guide/> when writing content for the web.

* active voice (<https://pages.18f.gov/content-guide/active-voice/>),
* acronyms and abbreviations (<https://pages.18f.gov/content-guide/acronyms-and-abbreviations/>),
* address the user (<https://pages.18f.gov/content-guide/address-the-user/>),
* avoid duplication (<https://pages.18f.gov/content-guide/avoid-duplication/>),
* be concise (<https://pages.18f.gov/content-guide/be-concise/>),
* conscious style (<https://pages.18f.gov/content-guide/conscious-style/>),
* plain language (<https://pages.18f.gov/content-guide/plain-language/>),
* capitalization (<https://pages.18f.gov/content-guide/capitalization/>),
* legal and technical content (<https://pages.18f.gov/content-guide/legal-and-technical-content/>),
* URLs and filenames (<https://pages.18f.gov/content-guide/urls-and-filenames/>),
* punctuation (<https://pages.18f.gov/content-guide/punctuation/>),
* headings and titles (<https://pages.18f.gov/content-guide/optimize-headings-and-titles/>),
* FAQs (<https://pages.18f.gov/content-guide/faqs/>),
* trademarks (<https://pages.18f.gov/content-guide/trademarks-and-brands/>),
* imagery (<https://pages.18f.gov/content-guide/images/>),
* voice and imagery (<https://pages.18f.gov/content-guide/voice-and-tone/>),
* common words and phrases (<https://pages.18f.gov/content-guide/specific-words-and-phrases/>), and
* references (<https://pages.18f.gov/content-guide/references/>).

# Reading-Level

The *SAM Web Standards* attempts to use a fifth grade reading level.

\\[link to site for determining reading level]

# "Words Not To Use"

Guidance as to terminologies that will not be included. (Possibly customize/add onto the common words and phrases in 18F Content Guide)

\\[listing of terms and acceptable alternative or guidance]

# Addressing the Integrated Award Environment

The *SAM Web Standards* attempts to use a fifth grade reading level.

[IAE Editorial Style Guide](http://gsaiae.confluence.micropaas.io:8090/display/IESG/IAE+Editorial+Style+Guide)

The IAE Editorial Style Guide has been developed using the most recent guidelines established by GSA and the federal government.  The guide outlines how we write and talk about the Integrated Award Environment and all work and products that come from this office, including (but not limited to):

* All 10 current IAE systems content updated from October 2015- forward
* [www.Transition.SAM.gov](http://www.transition.sam.gov/)
* The future SAM.gov 

This guide serves as a reference for any IAE staff member or contractor who is creating content in support of the program.

Please contact Ken Goldman with any questions, comments, or feedback about the style guide.