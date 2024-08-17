# How to Self-Publish a Book
This is a compilation of the knowledge I have acquired while writing my novels and self-publishing them on Google and Amazon.
My goal is to help those who wish to get started self-publishing an e-book and/or physical book.

In addition to these instructions, this repository contains a sample book that may be examined or used as a template for your own project.

Disclaimer: This guide is meant to provide general information based on my personal experiences and is not meant to serve as legal or business advice.

## Table of Contents
[My Novels](https://github.com/musicslayer/self_publish/blob/main/README.md#my-novels)<br/>
[Useful Resources](https://github.com/musicslayer/self_publish/blob/main/README.md#useful-resources)<br/>
[Creation Software](https://github.com/musicslayer/self_publish/blob/main/README.md#creation-software)<br/>
[Validation Software](https://github.com/musicslayer/self_publish/blob/main/README.md#validation-software)<br/>
[Steps to Make a Book](https://github.com/musicslayer/self_publish/blob/main/README.md#steps-to-make-a-book)<br/>
[Barcodes](https://github.com/musicslayer/self_publish/blob/main/README.md#barcodes)<br/>
[Additional Tips](https://github.com/musicslayer/self_publish/blob/main/README.md#additional-tips)

## My Novels
### How to Abuse Your Employee
https://play.google.com/store/books/details?id=Skp1EAAAQBAJ (e-book)<br/>
https://www.amazon.com/dp/B0B4X49L57 (e-book)<br/>
https://www.amazon.com/dp/B0B4L6VNNF (paperback)

### Finding Venus
https://play.google.com/store/books/details?id=wAuUEAAAQBAJ (e-book)<br/>
https://www.amazon.com/dp/B0BHRF5RSK (e-book)<br/>
https://www.amazon.com/dp/B0BHRFHDQ6 (paperback)<br/>
https://www.amazon.com/dp/B0BHMV2LR4 (hardcover)

### Defect
(Coming Soon)

## Useful Resources
### Fonts
https://fonts.google.com/<br/>
Contains high-quality, royalty-free fonts.

### ISBN
https://www.myidentifiers.com/identify-protect-your-book/isbn/buy-isbn<br/>
Can be used to purchase ISBNs if needed.

### Copyright
https://eservice.eco.loc.gov/siebel/app/eservice/enu?SWECmd=Login&SWECM=S&SWEHo=eservice.eco.loc.gov<br/>
The Electronic Copyright Office, where you can apply for copyright protection.

### Snappa
https://snappa.com/<br/>
Good for getting royalty-free artwork.

### Canva
https://www.canva.com/<br/>
Good for manipulating/formatting images.
			
### QuillBot
https://quillbot.com/grammar-check<br/>
Good for quickly checking your grammar/spelling.<br/>

### Thesaurus and RhymeZone
https://www.thesaurus.com/<br/>
https://www.rhymezone.com/<br/>
Useful tools when writing poetry.

## Creation Software
The following are various apps and websites that may be useful when creating your book.

### Sigil
https://sigil-ebook.com/<br/>
This is where you create the e-book (it will be an EPUB file).

### Microsoft Word 2007
After I am finished creating the e-book, I take the content and copy-paste it into a Word document.
> [!IMPORTANT]
> I've never tried more modern versions of Word or any of the free alternatives (Google Docs, Libre Office, etc.), so your mileage may vary if you don't use Word 2007.

### CutePDF Writer
https://www.cutepdf.com/products/cutepdf/writer.asp<br/>
This is a virtual printer that will take a Word document and "print" it to a PDF file. This is better than the built-in "Microsoft Print to PDF" option (which I find makes mistakes).

### Cover Calculator
https://kdp.amazon.com/en_US/cover-calculator<br/>
Used to generate a print cover template that will contain the front cover, back cover, and spine.
Once this is done, you can download the template file image as a PNG and PDF.

## Validation Software
The following are various apps and websites that may be useful when validating that your e-book is correct before shipping it.

> [!IMPORTANT]
> To validate a physical book, you can examine the PDF file, but otherwise you have to order proof copies from Amazon for the cost of printing.

### EPUBCheck
https://www.w3.org/publishing/epubcheck/<br/>
Used to validate your EPUB file.

### CSS Validator
https://jigsaw.w3.org/css-validator/<br/>
Validates the e-book's CSS file.

> [!IMPORTANT]
> You can access this from within Sigil, but unfortunately it defaults to validating against an older version of CSS, which will show a lot of bogus errors. It's better to go to the website and make sure "CSS Level 3 + SVG" is selected, and then use the option that lets you manually copy/paste the CSS file's contents.

### Play Books
Website: https://play.google.com/books<br/>
App: Download in the Play Store, or this may come on your Android device already.<br/><br/>
Upload the EPUB file and view it directly as a customer would.

### Kindle
Download the Kindle App to your Android or iOS device, or you can just use a Kindle device, and view your EPUB directly as a customer would.<br/>
Add the EPUB file to your Kindle library here: https://www.amazon.com/sendtokindle

### Kindle Previewer
https://www.amazon.com/Kindle-Previewer/b?ie=UTF8&node=21381691011<br/>
Install this desktop app and then you can open your e-book right inside the app. This is much quicker than using the regular Kindle app, and you can adjust the device size, orientation, font, font size, etc. to see how things look.

## Steps to Make a Book
This is a rough outline of what I do to create a book.
1. **(Optional) Create a pseudonym/pen name**
	- I use M. X.
	- Google and Amazon have no restrictions on what pseudonym you pick. In fact, there is another M. X. floating around! You may wish to pick something more unique than I did...	
	- Apple does NOT let you use pseudonyms unless you can show you legally own the name, which I have no clue how to do. Otherwise, you have to publish using your full legal name. For this reason, I don't bother with Apple.

2. **(Optional) Purchase an ISBN**
	- Physical books need an ISBN in order to create a barcode.
	- If you only plan to sell physical books on Amazon, you can use the free ISBN they give you, which will only work on Amazon and nowhere else.
	- If you want to sell physical books in other places as well, you have to pay for a real ISBN.

3. **Create an e-book in Sigil**
	- For my e-books, this is the order of sections I generally use:
		- Front Cover Image
		- Title Page
		- Table of Contents
		- Body (Prologue, Chapter 1, Chapter 2, ..., Chapter X, Epilogue)
		- Back Cover Image
	- An ebook is just a series of XHTML files, which are just like the HTML files that make up websites but stricter. Just like with websites, you can use CSS, but stay away from Javascript (e-reader support is very limited/inconsistent).<br/><br/>
	Note that within an e-book, a single XHTML file is basically displayed as one continuous stream of stuff. Different apps, devices, etc. will split the content differently, so 	don't worry about how things get divided too much within a single XHTML file.
	- E-books need a front-cover. There are three required steps:
		- Have the very first XHTML file in your ebook have the front cover image.
		- In Sigil, navigate to the "Images" folder, find the front cover image, right click it and select "Cover Image".
		- Inside "content.opf" there is a "guide" section at the bottom with an entry for the cover:
			```
			<guide>
				<reference type="toc" title="Table of Contents" href="Text/toc.xhtml"/>
				<reference type="cover" title="Cover" href="Text/front_cover.xhtml"/>
			</guide>
			```	
	- The Title Page - I keep mine really simple and just have the bare minimum.
		- The name of the book and the author's name, in the same font as they are on the cover (this is just a tradition, not a requirement).<br/>
		NOTE: If your friends want signed copies of your physical books, this is often a good place to sign it!
		- Any warnings (i.e. mature warning, content warning, trigger warning, etc. whatever phrase you wish to use).
		- Any disclaimers (i.e. this book is a work of fiction, not based on any real person, etc.).
	- The Table of Contents is tricky because you have to update multiple places.
		- There will be an actual XHTML file with your table of contents. It's basically a bunch of hyperlinks going to each chapter.
		- You have to create/update "toc.ncx".
		- As I mentioned with the front cover, inside "content.opf" there is a "guide" section at the bottom with an entry for the Table of Contents:
			```
			<guide>
				<reference type="toc" title="Table of Contents" href="Text/toc.xhtml"/>
				<reference type="cover" title="Cover" href="Text/front_cover.xhtml"/>
			</guide>
			```	
	- E-books don't really have a back cover. If you want to include one, just have the last XHTML file be the back cover image. Or you can omit this and make the back cover an exclusive to people who buy the physical edition of your book.
		
	- Fonts:
		- In an e-book, you MAY specify the exact font (good for things like headers, fancy titles, etc.), but for general text you typically specify a "font family" (i.e. serif, sans-serif) and then the e-reader will choose a font in that family for the user.
		- Note that most e-readers allow the user to completely override anything you specify in the e-book. Users can view your e-book in size 44 Wingdings if they want too!
		- For a physical book, you must specify the exact fonts you want for everything.
		- Make sure you only use fonts that are royalty-free so you don't get sued. Fonts that come with Microsoft Word (Times New Roman, Calibri) may not be licensed for you to publish a book, so you can get in trouble!
	
4. **Create a Word document in Microsoft Word**<br/>
Once the e-book is 100% finished, proofread, etc. And you are sure you won't make any other changes, then you create a Word document in Microsoft Word. You mostly copy/paste the content from the e-book (specifically the preview window in Sigil) into the Word document, but you have to make some adjustments:
	- You have to pick fonts as I say above, either because you didn't pick an exact font in the e-book, or sometimes certain fonts look good digitally but not in physical print.
	- The Table of Contents has to have actual page numbers and not hyperlinks. This means you have to have the entire book complete before you can fill in the Table of Contents.
	- The beginning of a chapter (or a prominent section) is traditionally on an odd-numbered page, so you might have to insert blank extra pages to make that happen.
	- You might want to manually space things so that certain content isn't split between pages.
	- Line spacing and font sizes may need to be adjusted even if the fonts are the same as the e-book.
	- Your physical pages will need a decent margin. I use 0.75 inches all around.
	- Page numbers:
		- In Word, you can add page numbers in the footers, and there is even a way to have all the odd-numbered footers look one way, and the even-numbered footers look another. Basically, if you are holding a book open, the left-hand pages need the page number at the left edge, and the right-hand pages need the page number at the right edge.
		- If you have to insert blank extra pages as I say above, then traditionally these pages are still counted, but the number should not be visible. To achieve this, I insert a big white rectangle shape to cover the entire page (it's safer to cover the entire page because "printing" to PDF might slightly adjust the location of the page number).
		- As far as where to start counting pages, consider that a book is divided into three sections:
			- Front Matter (Title Page, Table of Contents, etc.)
			- Body (The actual story)
			- Back Matter (Appendix, Index, etc.)
   
   		  A common convention is to number these as follows:
			- Use Arabic numerals for the body, starting with "1".
			- Use lowercase Roman numerals for the front matter and back matter, staring with "i" and using one continuous count across both sections.

> [!IMPORTANT]
> The Word document only contains the inside of the book, and excludes the front cover, back cover, and spine.
> Those will all be stored in a separate file.
	
5. **Create a PDF file using CutePDF Writer**<br/>
Once the Word document is 100% finished, then you "print" it to a PDF file using CutePDF Writer. What you see in this PDF is EXACTLY what the reader will see when the book is printed, so make sure it is correct!
	
7. **Upload to Google and Amazon**
	- Google will only allow you to sell e-books, whereas Amazon can sell e-books and physical books.
	- For both e-book and physical book, Google and Amazon will ask for a description, list of subjects, price, maturity rating, etc. which you have to provide. In the description, I also copy all of the warnings from the title page here as well so people can know what to expect before they buy.
	- For the e-book, you upload the EPUB file and the front cover image.
	- For the physical book, use the cover calculator to get a template file for the outer artwork i.e. front cover, back cover, and spine. You can upload this template file right to Canva and then arrange your artwork on top of it. When that's done, you give the template file to Amazon along with the PDF.
	
8. **(Optional) Apply for copyright protection**
	- In the US, any work is copyrighted the moment it is tangible, but if you ever want to sue someone (or you just want bragging rights), you need to file for copyright protection.
	- Once you are finished applying, then after a couple of months they mail you a fancy-looking piece of paper.

> [!CAUTION]
> If you obtain copyright protection, your legal name and your pseudonym will be tied together, meaning you can't stay anonymous. Anyone can look up your book and see the two names connected to each other.

## Barcodes
All physical books will need an ISBN 13 barcode printed on the front or back cover. Allowing Amazon to automatically add the barcode for you is by far the easiest option, however there may be situations where you wish to provide your own barcode. For example, in my latest book, "Defect", the Amazon-provided barcode would have covered up the gravestone poem, so I instead opted to place the barcode on the cover art myself.

Unfortunately, using your own barcode can be a complicated process. The steps below outline how you can do this without too much hassle and without spending any money.

### Getting an ISBN 13 number
As mentioned above, you can either purchase one yourself, or use the free one Amazon provides. Either way, you will end up with a thirteen-digit number.

### Getting an ISBN 13 barcode
Use the following websites to get the barcode:<br/>
https://bookow.com/resources.php#isbn-hyphenator to properly hyphenate the ISBN 13 number.<br/>
https://bookow.com/resources.php#isbn-barcode-generator<br/><br/>
For the price, I recommend entering 90000 ("no set price") to match what Amazon would use, or else enter your actual price.<br/><br/>
Make sure to download as a PDF so that the barcode is a vector image.

### Scaling the barcode
When you download the barcode PDF, you cannot decide what physical dimensions it will have. The following website allows you to adjust the PDF file to be whatever size you would like.<br/>
I recommend using a width of 2in and a height of 1.2in since that's what Amazon uses and recommends.<br/>

### Inserting the barcode into the cover art
Open up the cover art in your favorite PDF editor software (such as PDF-Exchange Editor) and decide where you would like to place the barcode, making sure to follow Amazon's placement requirements.<br/><br/>
The easiest way to do this is to insert the barcode as a stamp, which is essentially a type of comment. This lets you easily move around the barcode image and position it exactly where you would like it.<br/><br/>
Once you have decided on a position, save the PDF.

### Flattening the cover art
If you upload the cover art to Amazon now, the stamp will be discarded as an unprintable annotation. Thus, we first need to flatten the PDF.<br/><br/>
You can use PDF24 Creator or whichever software you prefer to do this. The result will be an identical PDF file, except this time the barcode will simply be part of the artwork and not a separate entity. This is the PDF that you will upload to Amazon as the cover art.<br/><br/>
To validate that the barcode is still a vector graphic, zoom in by a large amount, say 600%, and make sure that the barcode does not have any fuzziness or bluriness. A true vector image should remain sharp no matter how much you zoom in.

## Additional Tips
### Supported e-readers
Aside from Play Books and Kindle (and maybe Apple Books, I've never tried it), most e-reader apps will mangle your e-book, so I don't even bother trying to support them. Also, legitimate (non-pirate) customers shouldn't be using any other software anyway.

### Invisible spacing characters in Microsoft Word
If you are having trouble with spacing paragraphs, or inserting extra pages, etc. you can click the ¶ button (the "Pilcrow Sign" a.k.a. the backwards P looking thing) on the Home Ribbon to make all of the spacing characters visible. Generally, you might have to play around and finagle things to make everything spaced the way you want it. Word is finicky sometimes...

### Prohibited e-book elements
One common reason that an e-book may fail validation is because it contains prohibited elements.
Although some e-readers will allow you to open such an e-book, these elements may prevent you from uploading the e-book to Google or Amazon to sell.

1. \<text\>
The \<text\> element is completely prohibited everywhere. Luckily, the fix is often just to replace \<text\> with \<span\>.

	Bad:

	```
	<text>ABC</text>
	```
	
	Good:

	```
	<span>ABC</span>
	```

2. \<br\>
The \<br\> element (i.e. the \<br/\> tag) is disallowed in certain places, such as the following:
	- As a direct child of a list.

		Bad:
		
		```
		<ul>
			<li>First</li>
			<br/>
			<li>Second</li>
			<br/>
			<li>Third</li>
		</ul>
		```
		
		Good:
		
		```
		<ul>
			<li>First<br/><br/></li>
			<li>Second<br/><br/></li>
			<li>Third</li>
		</ul>
		```

 	- As a direct child of the \<body\> element

		Bad:
	
		```
		<body>
			<p>First</p>
			<br/>
			<p>Second</p>
		</body>
		```
	
		Good:
	
		```
		<body>
			<p>First<br/><br/><br/></p>
			<p>Second</p>
		</body>
		```

You may have to use two or even three \<br/\> tags to maintain the same (or similar) spacing. Some experimentation may be required.

### E-book Page Breaks
There are CSS properties that are supposed to guarantee that content in an e-book is not split between pages, however my experience is that none of these work consistently on every platform. In my opinion, it's not worth bothering with any of the following:
```
-webkit-page-break-inside: avoid;
break-inside: avoid;
page-break-inside: avoid;
```

### Creating a PDF of a Word Document With Fixed Physical Dimensions
Let's say you want to convert your Word document to a PDF with each page being 6in x 9in (this is a common trim size for books that are printed by Amazon):
1. In Word, go to the Page Layout Ribbon, and click Size -> More Paper Sizes. From there, select "Custom size" and enter 6in x 9in.
2. Set CutePDF Writer to use a paper size of 6in x 9in (See "Important" section below).
3. "Print" your document as you normally would. Choose "CutePDF Writer" as your printer, and make sure "Scale to paper size" is set to "No Scaling" and "Print to file" is NOT checked.

> [!IMPORTANT]
> Changing the size of the PDF that CutePDF Writer will create requires a few steps:
> 1. In the Windows start menu, go to "Settings".
> 2. Navigate to Bluetooth & Devices -> Printers & scanners -> CutePDF Writer -> Printer properties.
> 3. In the General Tab, click "Preferences".
> 4. In the Layout Tab, click "Advanced".
> 5. For "Paper Size", select "PostScript Custom Page Size" and then click "Edit Custom Page Size".
> 6. For "Width" enter 6, and for "Height" enter 9. Make sure "Unit" is set to "Inch".
> 7. Click OK, click OK, click Apply, and click OK.
>
> Note that you cannot do this directly in Word when printing. Even though it is possible to access these dialogs, for some reason there is no "Apply" button and the changes to the setting do not persist.

### Creating a PDF of an Image With Fixed Physical Dimensions
Unlike with Word documents, we will not be using CutePDF Writer as there is a much easier way. Let's say you have an image, but you wish to convert it to a PDF and have it be 12in x 14in:
1. Create a new 12in x 14in design in Canva.
2. Upload your image and insert it into the Canva design, making sure to proportionally stretch it out to fill the entire space.
3. Download the design as a PDF file (For "File Type", choose "PDF Print").

### Adding an Image to Sigil
In theory, is it easy to add an image to an e-book in Sigil. Just find the "Images" folder, right click, and select "Add Existing Files...".
Unfortunately, Sigil may automatically adjust the image size. If you add the image a second time (replacing the first file), this tends to use the correct image dimensions.

I assume this is some sort of bug in Sigil.

### Preventing E-book Bloat
Adding images to an e-book increases the file size. This can get out of hand if high-resolution images are used. In particular, Amazon and Google may limit the file size of your e-book, and a larger file size may cut further into your royalty payment.<br/><br/>
Here is my process for handling this:
1. Start with 1410px x 2250px images.
2. In Microsoft Paint, create a copy that is scaled down to 40% i.e. 564px x 900px.
3. This smaller image is what gets added to the e-book in Sigil.
4. When I go to place the image in an XHTML file, I use a viewport that is the original 1410px x 2250px.
```
<svg xmlns="http://www.w3.org/2000/svg" height="100%" preserveAspectRatio="xMidYMid meet" version="1.1" viewBox="0 0 1410 2250" width="100%" xmlns:xlink="http://www.w3.org/1999/xlink">
	<image width="1410" height="2250" xlink:href="../Images/front_cover.png"/>
</svg>
```

> [!TIP]
> This process of scaling down should only be used for images that are embedded within an e-book file. When uploading cover images directly to Google or Amazon, you should use the original image.

### Image Resolutions
When I create images in Snappa (for example, to use as the cover), I use a resolution of 1410px x 2250px for the original image, and then I can scale it up or down from there later as needed. There are various recommendations floating around out there, but I find this works fine for me.

### Using EPUBCheck
EPUBCheck is a command line tool, and can be tricky. The easiest way to use it is the following process:
1. Make sure Java is installed on your machine.
2. Make sure "epubcheck.jar" and a copy of your EPUB file are in the same folder.
3. Open a command prompt in that folder.
4. Execute the following command:
```
java -jar epubcheck.jar sample.epub
```

After a few seconds, you will see every issue enumerated and a total count of errors and warnings.
		
> [!TIP]
> This validation is really strict! Some e-readers won't care about some of the issues it finds. Despite this, I do recommend fixing your e-book so that there are no errors or warnings. Typically, the first time these issues cause a problem is when you upload the e-book to Google and they reject it.

### Spines
You can only customize the spine of your book if it is thick enough i.e. it has enough pages. If you are only a few pages away from the threshold, one trick is to insert blank pages at the end of the book (Amazon lets you add up to ten consecutive blank pages at the end).
