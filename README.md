# adapt-textWithCode  

**Text with Code** is a *presentation component* for the [Adapt framework](https://github.com/adaptlearning/adapt_framework).  


**Text with Code**'s simple purpose is to present text. The text may include HTML, code wrapped in `<pre><code class="language-[language name]">` tags, and infoboxes (divs marked with the class "infobox" and "idea", "note", or "warning").

## Installation

### Installing Text with Code
With the [Adapt CLI](https://github.com/adaptlearning/adapt-cli) installed, run the following from the command line:  
`adapt install adapt-textWithCode`

Alternatively, this component can also be installed by adding the following line of code to the *adapt.json* file:  
`"adapt-textWithCode": "*"`  
Then running the command:  
`adapt install`  
(This second method will reinstall all plug-ins listed in *adapt.json*.)  

### Installing Prism
Text with Code works based on the [Prism](https://prismjs.com) highlighter. To keep the code small, you will have to install this library and css yourself based on which languages and style you want to have. To do so, visit the [Prism download page](https://prismjs.com/download.html) and select the languages and theme you want. Place the resulting prism.js file in src/core/js/libraries. Rename the css file as "prism.less" and place it in src/core/less.

## Settings Overview

The attributes listed below are used in *components.json* to configure **Text with Code**, and are properly formatted as JSON in [*example.json*](https://github.com/adaptlearning/adapt-contrib-text/blob/master/example.json). Visit the [**Text** wiki](https://github.com/adaptlearning/adapt-contrib-text/wiki) for more information about how they appear in the [authoring tool](https://github.com/adaptlearning/adapt_authoring/wiki).

### Attributes

[**core model attributes**](https://github.com/adaptlearning/adapt_framework/wiki/Core-model-attributes): These are inherited by every Adapt component. [Read more](https://github.com/adaptlearning/adapt_framework/wiki/Core-model-attributes).

**_component** (string): This value must be: `textWithCode`.

**_classes** (string): CSS class name to be applied to **Text with Code**’s containing `div`. The class must be predefined in one of the Less files. Separate multiple classes with a space.

**_layout** (string): This defines the horizontal position of the component in the block. Acceptable values are `full`, `left` or `right`.  

**title** (string): A reference title for the component. **title** is distinct from the **displayTitle** which, if present, appears above the component. **title** provides the opportunity to use a shortened form in tighter spaces, such as in menus or in the drawer.  

**displayTitle** (string): Optional text that will display as a title or header above the component. It can be used as a headline.   

**instruction** (string): This optional text appears above the component. It is frequently used to
guide the learner’s interaction with the component.

**body** (string): Although optional, this text constitutes what is thought of as the primary *text* of the **Text with Code** component. HTML is permitted and code properly wrapped will be automatically highlighted.  
<div float align=right><a href="#top">Back to Top</a></div>

## Limitations

No known limitations.   


----------------------------
**Version number:**  1.0.0 
**Framework versions:** 2+  
**Author / maintainer:** [Aaron Collier](https://github.com/CollierCZ). Forked in June 2018 from the [Text component](https://github.com/adaptlearning/adapt-contrib-text) written by the Adapt Core Team with [contributors](https://github.com/adaptlearning/adapt-contrib-text/graphs/contributors)    
