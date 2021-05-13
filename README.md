# eGain-KM-Widgets

Empower and enable your website visitors to access the wealth of knowledge from your knowledge base on any website they visit in your domain with knowledge widgets. Knowledge Widgets allow specific eGain knowledge functionality to be embedded in a web page. Regardless of the content of the web page or the reason the user is accessing the site, knowledge widgets are versatile tools that can be placed on the web page to provide immediate answers to a customer's question. There are a variety of widgets to choose from, including:

  1. **Popular Articles Widget**: Renders a list of popular articles in an HTML page based upon initialization parameters in the HTML element. (Git Repository: https://github.com/snehaldatar/eGain-KM-Popular-Articles-Widget)
  1. **Search Widget**: Renders a list of articles matching the search parameter. The search widget does not consume a WSS license until a search is performed. (Git Repository: https://github.com/snehaldatar/eGain-KM-Search-Widget)
  1. **Search Field Widget**: Renders a text input, search button and a list of of articles matching the search parameter. (Git Repository: https://github.com/snehaldatar/eGain-KM-Search-Field-Widget)
  1. **List Widget**: Renders a list corresponding the list name parameter matching the name of the list in the portal configuration. The list widget consumes a WSS license to display the list of articles, regardless of whether the user clicks through to an article. (Git Repository: https://github.com/snehaldatar/eGain-KM-List-Widget)

These widgets can be configured in the customer's HTML page which can be rendered as desired (dynamically or page load). There is no restriction on combination of widgets i.e., the widgets can be combined with each other in any order in the page.

eGain Github library provides different examples on how to use these widget into your web application and quickly integrate with your web applications.

# Widget Library

eGain widget library is shipped with eGain application. The library must be included in the page(s) that are going to enable eGainUI Widgets. The recommendation is to deploy this reference in a global header or footer so the widgets can be deployed dynamically to any page without further site modifications.

```javascript
<script type="text/javascript" src="//your_egain_system_url_with-context_root/widgets/libs/egain-ui-2.0.0.min.js"></script>
```

All widgets can be configured in the customer's HTML page which can be rendered as desired (dynamically or page load). There is no restriction on combination of these widgets i.e., the widgets can be combined with each other in any order in the page.

Each widget follows a pattern in which the attributes of the placeholder HTML element can be configured. 

# Using eGain KM Widgets
This sample application uses Search Widget, Search Field Widget, List Widget and Popular Articles Widget. The Search widget is being used to fetch the corresponding articles from eGain knowledge matching the short description. Initially search will be done using pre populated short description. Search results will be updated dynamically as we change the short description.

## Configuring The Sample Application

1. Clone or download the Sample Application from git hub repository https://github.com/snehaldatar/eGain-KM-Widgets.
1. Change below attributes as required in the index html file.
    1. your_egain_system_url_with-context_root
    1. your_kb_portal_id
    1. list-name-configured-in-portal
    1. your_search_param
1. Now you should be able to fetch the search results from your eGain knowledge portal by loading the index html in browser.


