---
title: SAM Web Standards - Components
layout: sam_web_standards
---

# Components

## Header

The header consists of the branded home button, main navigation, and application navigation elements (only when within an application). The branded home button consists of the transition.SAM.gov logo with a link to https://transition.SAM.gov/ allowing users to go to https://transition.SAM.gov from anywhere within the site.

### Unauthenticated

![header with logo left side, sign on button on the right side and "Take me too..." button is below both]( {{site.baseurl}}/assets/img/components/unauthenticated_header.png "Unauthenticated Header"){: .iae-img }

### Authenticated

![header with logo left side. On the right side is "Hello Jane Smith", alerts badge with 5 alerts, and a user icon for more user options. "Take me too..." button is below both]( {{site.baseurl}}/assets/img/components/authenticated_header.png "Authenticated Header"){: .iae-img }

[Accordion with code sample]

[Accordion with technical description]

### Category Navigation

The category navigation allows each service to create pages within the category’s area within transition.SAM.gov. For example, https://transition.SAM.gov/wages/resources would be a page consisting of links to resources related to Wage Determinations and available within the Category Navigation element when a user is anywhere within https://transition.SAM.gov/wages.

[representation of navigation]

## Footer

The SAM Web Standards uses the "big footer" defined by the *US Web Design Standards* as a base.

![]( {{site.baseurl}}/assets/img/components/footer.png "Footer"){: .iae-img }

## Page Templates

### Default

The default page template consists of the Header and Footer with a free-form content area between.

## Form Templates

See the *US Web Design Standards* for form templates related to name, address, sign-in, and password reset ([https://playbook.cio.gov/designstandards/form-controls/](https://playbook.cio.gov/designstandards/form-controls/)).

### Application/Category Search Forms

Most of the applications/categories within SAM, use search forms to retrieve data related to an application/category. The forms accommodate text-based search as well as the optional application of filters. Filters are applied using a dropdown menu of options; multiple selections are allowed. Users can then deselect identified filters.

[Need image or live coded results, with technical description - until then, see [https://www.healthcare.gov/see-plans/#/plan/results](healthcare.gov)]

### Application/Category Filter

Used on pages where content spans multiple applications wherein a front-end user may wish to include or exclude any of the content related to the applications.

[Need image or live coded result, with technical description]

## Search Result

Used to display an individual results within a list of search results. Contains content information/summary and metadata related to the content. Metadata generally represent optional filters, which can be applied by the user, and are grouped together to easily discern between result content and metadata.

[Need image or live coded results, with technical description]

## Pagination

The pagination element is used in circumstances where the content being displayed within a site area that cannot be fit on one page (search results, for example). If JavaScript is enabled, continuous scrolling methods can be used in place of the pagination element; however, this element should exist in case JavaScript is disabled.

[representation of pagination mechanism]

## Widgets

The *SAM Web Standards* uses the ________ standard [link to reference](). "Widgets are an essential aspect of home screen customization. You can imagine them as "at-a-glance" views of an app's most important data and functionality that is accessible right from the user's home screen."

## Confirmation and Acknowledgement

The *SAM Web Standards* uses the alert concepts from the *US Web Standards* as a base.

### Confirmation (prior to action)

Confirming is asking the user to verify that they truly want to proceed with an action they just invoked. In some cases, the confirmation is presented along with a warning or critical information related to the action that they need to consider.

[representation of Confirming]        

### Acknowledgement (following action)

Acknowledging is displaying text to let the user know that the action they just invoked has been completed. This removes uncertainty about implicit operations that the system is taking. In some cases, the acknowledgment is presented along with an option to undo the action.

[representation of Acknowledging]

## Icons

The application of standard icons follows the guidance of [Font Awesome](https://fortawesome.github.io/Font-Awesome/icons/) for common icons.

[representation of common icons such as 'share' or 'new']