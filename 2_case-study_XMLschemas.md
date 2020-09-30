
# Case study: the Letters 1916-1923 schema for early 20th-century correspondence

XML schemas are templates that define XML elements specifally for one edition project or a series of related projects, e.g. editions of historical letters. Parsing XML files against the project schema ensures that the syntax and hierarchies of the files are correct and that the files will eventually display correctly on the web or in print.
However, defining a schema also comes with many pitfalls, one of them being the premature limitation of options to describe certain textual features. The challenge especially affects editions of historical sources as pre-modern texts often use inconsistent spelling, quotes from foreign languages such as Greek and Latin, or may contain many sections that are no longer legible.

Developing a model schema for editions of historical letters has been one joint project in the Digital Humanities, addressed by researchers of different disciplinary backgrounds and from different countries:

cf. ["Towards a Model for Encoding Correspondence in the TEI: Developing and Implementing <correspDesc>" by Peter Stadler, Marcel Illetschko and Sabine Seifert](https://journals.openedition.org/jtei/1433)

A custom XML schema was also developed for the [Letters 1916-1923](http://letters1916.maynoothuniversity.ie/) project, a collection of letters written in, to or about Ireland between the Easter Rising of 1916 and the end of the Irish Civil War in 1923. The focus of text encoding in Letters 1916-1923 was placed on the metadata, including the places where the letters were written or sent to. As a consequence, the elements of the initial Letters 1916-1923 schema were both adaptable to other collections of letters and project-specific:

https://raw.githubusercontent.com/bleierr/Letters-1916-sample-files/master/plain%20corresp%20templates/template.rng

One encoding decision that later proved to be problematic was the detailed specification of person names and place names within the XML/TEI schema as two many variations occurred over time.

!["persName" and values in the original Letters 1916 schema](https://github.com/MonikaBarget/DigitalEditing4Historians/blob/master/PersName_Letters1916_Schema.png)

The solution in the second phase of the project was to accept different spellings for towns, streets or people in the XML files but keep track of the variations in a separate spreadsheet which was then used to create normalised search filters and drop down menues in the new project infrastructure. This process may be referred to as "consecutive disambiguation", keeping the actual transcription and encoding workflow as lean and as possible.

# Task: 

Imagine that you are asked to create a digital edition of judicial regulations published in Mainz.

If you are able to read early modern print, look at the digitised [Untergerichts-Ordnung des Ertzstiffts Meyntz, Mainz, 1543](https://daten.digitale-sammlungen.de/~db/0002/bsb00029454/images/) and try to come up with elements that ought to be included in the schema for your digital edition.

![Title Page Gerichtsordnung](https://github.com/MonikaBarget/DigitalEditing4Historians/blob/master/GerichtsordnungMainzTitel_BSBM%C3%BCnchen.jpg)

Source URN: http://mdz-nbn-resolving.de/urn:nbn:de:bvb:12-bsb00029454-6
Licence: CC BY-NC-SA 4.0
Copyright: DFG, BSB München

What information must be included in every XML file created for a collection of early modern judicial regulations of this kind? What information is optional?
What "values" must be provided in normalised form, what "values" can be entered in several variations, reflecting usage in the original source?

You might want to put your considerations in a table and describe your thought process in a short text. The IEG DH Lab would be delighted to feature your contributions on our [blog](https://dhlab.hypotheses.org/).

