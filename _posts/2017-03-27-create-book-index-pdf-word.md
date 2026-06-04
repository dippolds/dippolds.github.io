---
id: 1098
title: 'Create a book index from a PDF using Word manuscript'
date: '2017-03-27T12:43:14-04:00'
author: 'Sean Dippold'
excerpt: ''
layout: post
guid: 'http://seandippold.com/?p=1098'
permalink: /2017/03/27/create-book-index-pdf-word/
categories:
    - Tech
tags:
    - pdf
    - word
    - writing
format: false
---

Publishers often ask non-fiction book authors to create an [index](https://en.wikipedia.org/wiki/Index_(publishing)) of their work. Creating an index is a non-trivial task often performed by people who specialize in creating indexes using software designed for that purpose. Adding to the complexity is authors usually work in Microsoft Word while publishers work in Adobe PDF. The PDF generated as a proof will have different page numbers than the original Word document. If faced with indexing a PDF book, there is a less painful method whose trick is to match the proof PDF page numbers with the Word manuscript and use the indexing features of MS Word. **Create a Word document with the same page numbers** (a little tedious)

1. Make a copy of the original Word document to use for indexing. Make sure a page number is being shown on each page of this copied document.
2. If the PDF has more pages than the Word version, jump to step 4
3. If the PDF has fewer pages, reduce the spacing from double space to single space. This will prevent auto-pagination from adding page breaks where you don't want them
4. With the copy opened in Word and the PDF opened, insert page breaks in the Word document in the same places as the PDF Insert, Page Break. Repeat until the Word document has the same page number marking as the PDF.
5. The keyboard shortcut for Page Break is *fn+Shift+return* on Mac and *Ctrl-Enter* on Windows.
 
 **Flag each word/phrase desired in the index** (the laborious part) 1. Highlight the word or phrase to be indexed
2. On the References tab, in the Index group, click Mark Entry.
3. Repeat for the whole book including duplicates of word/phrases. The AutoMark feature will help find all entries for word if desired.
 
 Note you can have more complex indexes (subentries, etc.) by [marking things appropriately](https://support.office.com/en-us/article/Create-an-index-and-update-an-index-cc502c71-a605-41fd-9a02-cda9d14bf073#bm5). **Generate the index** (the quick part) 1. Goto the end of the document (to avoid harming the real page numbers)
2. References tab, in the Index group, click Insert Index.
3. If you go back and add or change index entries in the document, remember to click Update Index in the Index group on the References tab.
4. A variety of [formatting options is available](https://support.office.com/en-us/article/Create-an-index-and-update-an-index-cc502c71-a605-41fd-9a02-cda9d14bf073#__toc276464710).
 
 **Provide the index to the publisher** 1. Open a blank Word document
2. Select the generated index and copy it. In the blank Word document, Paste Values to avoid the index being recalculated on a blank document.
3. Save and provide this document to the publisher.
 
 Versions of Microsoft Word The menu commands vary between different version of Word. For example, Word 2008 on Mac uses Insert, Index and Tables to both mark entries and generate the index. [![](/wp-content/uploads/2017/03/Word_2008_Index.png)](/wp-content/uploads/2017/03/Word_2008_Index.png)### Other Tools

 Adobe Acrobat Pro - has an indexing feature but this has nothing to do with book indexs Google Docs - doesn't support indexing, only table of contents based on header levels [PDF Index Generator](https://www.pdfindexgenerator.com/) - $70 specialized tool for creating indexes from PDF files Converting from PDF to Work is not likely to work cleanly due to PDF formatting