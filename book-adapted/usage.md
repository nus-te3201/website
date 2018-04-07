<link rel="stylesheet" href="{{baseUrl}}/css/textbook.css">

<div class="website-content">
<div id="body">

# Using This Book

<div id="text-only">

* [Browser Compatibility](#browsers)
* [Information Layers](#layers)
* [Conventions Used](#conventions)
* [Saving as PDF files](#saving)
* [Printing](#printing)

<div id="browsers">

### Browser Compatibility

This book is best viewed using the ==Chrome browser==.

</div>
<div id="layers">

### Information Layers

The book tries to _layer_ information so that readers can decide to omit less important layers if they wish to. 

**More important information are in bold** or ==highlighted== while %%less important information are dimmed%% or in collapsed panels such as the below.

<panel header="%%Some less important info in a panel%%">

Less important info

</panel><p/>
<panel header="%%Some less important info in a boarder-less panel%%" type="seamless">

Less important info

</panel><p/>

**Tabs indicate alternative formats of the same content** (e.g. video vs text). You can choose the one you like and ignore the other tabs. 

<tip-box>

<tabs> 
  <tab header=":abc:">
  
Some textual description of X

  <hr></tab>
  <tab header=":tv:">

Video describing X

  <hr></tab>
</tabs>

</tip-box>

**Dotted underlines indicate <trigger for="pop:tooltip-example">tool tips</trigger>** (activated by hovering over it) and **dashed underlines indicate <trigger for="modal:modal-example" trigger="click">modal windows</trigger>** (activated by clicking) containing additional information.

<popover id="pop:tooltip-example" title="Tooltip Example" placement="top">
  <div slot="content">
    Additional information
  </div>
</popover>

<modal title="Modal Example" id="modal:modal-example">
  Additional information
</modal>

**Sections tagged as :zero: can be ignored because they are tangential info** that are strictly not within the scope of the topic.

</div>
<div id="conventions">

### Conventions Used

Meaning of some shortened headings:

* **What** : the **meaning** of the concept in concern 

  <include name="%%Example%%" src="../book/refactoring/what/full.md" dynamic />

* **Why** : the **motivation** behind the concept in concern

  <include name="%%Example%%" src="../book/documentation/guidelines/goTopDown/why/full.md" dynamic />
  
* **How** : the **usage** of the concept in concern 

  <include name="%%Example%%" src="../book/refactoring/how/full.md" dynamic />
  
* **When** : the **pros and cons** of the concept in concern, **when to use** the concept 

  <include name="%%Example%%" src="../book/refactoring/when/full.md" dynamic />
  

Boxed-text styles:

<tip-box type="info">
    additional info
</tip-box>
<tip-box type="warning">
    warning
</tip-box>
<tip-box type="success">
    positive message
</tip-box>
<tip-box type="important">
    important message
</tip-box>
<tip-box type="wrong">
    an error to avoid
</tip-box>
<tip-box type="tip">
    tip
</tip-box>
<tip-box type="definition">
    definition
</tip-box>

Meaning of icons:

* :one: :two: :three: :four: : indication of the depth of the topic, in order of increasing depth (:one: is the least depth)
* :zero: : tangential info, can be ignored if not interested
* <span class="glyphicon glyphicon-new-window" aria-hidden="true"></span> : direct link to the LO. `Ctrl+Click` to open the LO in new window/tab.
* :trophy: : learning outcomes
* :mortar_board: : prerequisite learning outcome
* :package: : examples
* :paperclip: : resources
* :muscle: : exercises
* :scroll: : printable version
* :mag: : preview/more info
* :tv: : video
* :abc: : textual description
* :bar_chart: : slides
* :arrow_heading_down: : output produced by running code
* :lock: question without answer
* :lock::key: question with answer

</div>
<div id="searching">

### Searching

The book currently does not have a _search_ feature. The workaround is to load the entire book into the web page (i.e. either the _full_ version or the _printer-friendly_ version) and use the Browser's search function.

</div>
<div id="saving">

### Saving as PDF Files

1. Use Chrome to load the page you want to save as pdf.

1. Click on the `Print` option in Chrome’s menu.

1. Set the destination to `Save as PDF`, then click `Save` to save a copy of the file in PDF format. For best results, use the settings indicated in the screenshot below.<br/>
  <img src="{{baseUrl}}/book/about/images/chromeSaveAsPdf.png" />

</div>
<div id="printing">
  
### Printing

A printer-friendly version of the entire book can be found [here]({{baseUrl}}/book-adapted/print.html)

</div>

</div> <!-- text-only -->
</div>
</div>
