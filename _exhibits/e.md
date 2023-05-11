---
layout: exhibit
title: 'The Project'
permalink: /exhibits/e/
---

The Paris Project is a collaboratively created digital edition of Hope Mirrlees's modernist long poem *Paris,* edited by [Melanie Micir](https://english.wustl.edu/people/melanie-micir) and [Anna Preus](https://english.washington.edu/people/anna-preus) and supported by the [Humanities Digital Workshop](https://hdw.wustl.edu/) at Washington University in St. Louis. The text of the digital edition represents a diplomatic transcription of a copy of the first edition held by Washington University Libraries.


**Contributors**

[Jaleen Grove](https://www.risd.edu/academics/illustration/faculty/jaleen-grove)<br>
[Ann Marie Jakubowski](https://english.wustl.edu/people/ann-marie-jakubowski)<br>
[Douglas Knox](https://computing.artsci.wustl.edu/people/douglas-knox)<br>
[Stephen Pentecost](https://computing.artsci.wustl.edu/node/13151)<br>
[Anwesha Kundu](https://www.centre.edu/about/faculty-staff/anwesha-kundu)<br>
[Sophie Levin](https://english.wustl.edu/people/sophie-levin)<br>
[Nikita Willeford Kastrinos](https://english.washington.edu/people/nikita-willeford-kastrinos)<br>


**Process**

In 2017, we set out to create a digital edition of *Paris* that would make the poem more accessible for contemporary readers. With an explicit investment in feminist digital approaches, and with assistance from an interdisciplinary team of faculty, postdoctoral fellows, library staff, and both undergraduate and graduate students, we have worked to recreate the Hogarth edition of Mirrlees’s poem in digital form. Just as Mirrlees’ writing challenged printing conventions in its time, the poem challenges systems for representing texts digitally today, and attempting to recreate its complex visual design required us to think creatively about how to use digital systems to mimic typesetting decisions made a century ago. What follows is a short description of the process through which we digitized the text. 

{% include inline_image.html collection='paris-project-exhibition' pid='pci_163' %}

In the first year of this project we were fortunate to work with Jaleen Grove, a historian of illustration and graphic design, who encouraged us to look not just at the words on the page, but to see each page as a visual construction in its own right. Given the poem’s layout, the idea that it existed as both text and image conceptually made sense, but it was hard to build that idea into the structure of our digital edition, the basis of which is an XML file that adheres to the Text Encoding Initiative (TEI) Guidelines–a collaboratively built schema for marking up texts in a form that is both human- and machine-readable. Recording the poem’s original layout within the TEI guidelines for encoding verse turned out to be quite difficult, though, since the spacing and layout was so varied. 

{% include inline_image.html collection='paris-project-exhibition' pid='pci_163' %}

Ultimately, what helped us address this issue was a return to the methods that Woolf used when publishing *Paris*. She printed the book on a small press in her dining room, and all she had to work with when creating the layouts for each page were pieces of moveable type that, when inked, made impressions on rectangular surfaces. Focusing on the typesetting process in turn brought our attention to something we did not initially see: whitespace. In letterpress-printed text, whitespace is created through the insertion of individual pieces of spacing material, which function just like regular type but do not make a mark on the page. Wherever Woolf wanted to create spaces in Mirrlees’s poem, she had to insert spacing material, and it was the insertion of these pieces of spacing material that made the complicated layout of the poem possible. In order to copy her layout while preserving the poem as text, we would have to insert individual blocks of digital spacing “material” in our edition as well.

{% include inline_image.html collection='paris-project-exhibition' pid='pci_163' %}

Jaleen began measuring the placement of each line of text and each character within the lines, but promptly ran into issues because all the pages were slightly different sizes and the binding was wonky. To deal with this, she scanned and measured each page, averaged the measurements, and established an idealized page size for our edition.

{% include inline_image.html collection='paris-project-exhibition' pid='pci_163' %}

Meanwhile, Anna started trying to figure out how to encode Jaleen’s meticulous measurements in XML. However, because we were capturing so many typographic irregularities, ran into issues using the TEI standards for encoding printed texts and had to turn to manuscript studies conventions. Moreover, because we were measuring to the typographic point–which is 1/72 of an inch–our measurements varied on a smaller scale than could be represented through standardized spacing in modern digital typefaces–another thing we had to figure out. Throughout all of this, Melanie, who was handling content-related editorial work at the time, made sure we were connecting our focus on whitespace back to the text of the poem and to our overall goal of making it more accessible to contemporary readers.

{% include inline_image.html collection='paris-project-exhibition' pid='pci_163' %}

After a lot of discussion, measuring, encoding, re-measuring, and re-encoding, we ended up with a transcription of the poem that included customized space tags with exact dimensions for each bit of whitespace on each of the 23 pages in the printed book. 

{% include inline_image.html collection='paris-project-exhibition' pid='pci_163' %}

We also transcribed Julia Briggs's original notes to the poem into TEI. We then used TEI Boilerplate to translate the TEI files into HTML for web display. Later, we wrote hundreds of CSS rules, so a browser could interpret each of the custom space tags we had created. Doug Knox and Steve Pentecost then helped us create a customized platform that would allow users to select different views of the poem. For example, the default view for the digital edition presents the poem as a continuous scroll, but readers can view the original page breaks, margins, and numbers by selecting the "pages" view.  

{% include inline_image.html collection='paris-project-exhibition' pid='pci_163' %}

Once we had mounted the poem online, we were able to begin thinking about our initial goals again and started thinking about how to create a website that was useful and engaging to contemporary readers. To this end, we gathered historical images to include in the edition, added Briggs's notes, built a website using the minimal computing platform Wax, added contextual essays, and created more display options for the poem, including a facsimile of the copy of the 1920 first edition held by the Librares at Washington University in St. Louis. The project has been shaped throughout by the labor and insights of a tremendously generous group of collaborators without whose contributions this edition would not have been possible.

*By Melanie Micir and Anna Preus* 


**Credits**

The website was created using [Wax](https://minicomp.github.io/wax/). The digital edition was created using [TEI Boilerplate](https://dcl.ils.indiana.edu/teibp/). The notes included in the digital edition were written by Julia Briggs. 

All the files and code used for the project are available on [Github](https://github.com/apreus).