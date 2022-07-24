INTRODUCTION: All the style sheets used in this framework are in this one folder. They should always be kept together here in this one "styles" folder so everyone in your team has access. Grouping all these CSS files together in one folder allows you to keep all your design files together and makes web redesigns extremely simple and portable.

WARNING: Feel free to manually remove all my comments from these CSS files to reduce size, but do NOT use a minimizer, preprocessor, SASS, or script to do so as there are very carefully placed CSS hacks inside each file that are used for showing and hiding rules from older browsers. If you do so, these rules will get stripped out by accident and this style sheet framework will then fail. You may use custom 3rd party tools to change the Styles, Mobile, and Print CSS files.

----------------------------------------


HOW DOES THIS STYLE SHEET SYSTEM WORK?

It is very simple.

First, this CSS system resets or restyles all known HTML elements (HTML3.2/HTML4.1/HTML5), supported or not, to clean, stable designs. It does NOT restructure or radically change the HTML elements. It simply aligns their CSS designs across all known browsers to a single, cross-browser design set that works in the widest range of web browsers going back over 20 years!

In redesigning the elements, it makes sure a few simple CSS design features are added that allow very old browsers (pre-2001) and many medium range ones (like IE 1-7) to display text content in clean, stacked, vertical blocks of text. It essentially delivers to all browsers a plain white set of HTML elements and layout styles for the core HTML elements that display all your text and media files in a clean, white page with minimal margins and padding, and with plain black text in a simple san-serif font set at a universal, readable, medium size. This then allows a large range of older browsers built prior to 2010 to see your pages of web content and images in white vertical pages so the text is readable, scrollable, and accessible.

Instead of struggling to force dozens of older browsers to figure out complicated HTML5 layouts, floats, and flex boxes that fail, you now degrade layouts to plain HTML elements only. That simple idea is critical, as you do NOT want to struggle to try and force say old Internet Explorer to try and fix crazy flex or floating layouts, or fail to display complex fonts, or read CSS variables they dont understand, when they likely will all fail due to incomplete CSS support and broken box model interpretation. So, using this old reset sheet system, a wide range of browsers are given a standard, clean but gracefully degraded vertical, block-level layout these old browsers can now access and read. This old element sheet is give to hundreds of older browsers and versions going back to the 1990's. This system even allow 1990's browsers who ignore Cascading Style Sheets to see you content in even simpler blocks. By using my prefered HTML5 Tutorial example (see below), even those ancient early browsers will now be able to read your web content!

Lastly, the system then applies a NEW modern reset HTML element sheet. This new sheet is hidden from the old browsers above using a special @import style sheet trick all known modern browsers understand but older ones do now. THis new reset element sheet then cascades over the old one above with newer CSS3 element designs and features the old browser would not understand, allowing you to now use a solid modern HTML element foundational design for all know HTML elements used in your website. With this modern reset you now can apply custom cutting-edge CSS3 designs using the same @import system above, which is also hidden from the older browsers. So now, you can safely apply newer CSS3 layouts like grid of flex layout designs, knowing they would fail in older browsers but now safely hidden from them.

You now deliver plain black and white text-based content in clean fast HTML to older browsers, and fast, cutting-edge CSS3 layouts and HTML5 element sets to newer browsers going forward. You never have to ever design for old browsers like Internet Explorer 6, Netscape 4, Opera 4, or IE for the old Macs ever again. You can forget about the older browsers forever, yet know your web page content is still viewable by every single one of those older browsers going forward. 

You can now safely focus 100% of your time on newer HTML5 web design!

* Note: Because Internet Explorer 8-11 are seen by the newer CSS you add to the modern CSS pages, you may still have to add a few custom hacks or CSS to code for a few browser bugs. But those now are isolated and can be given fixes that address things like flex boxes, grids, HTML5 elements like "main", etc. But you can now safely target these last old buggy browsers very easily from the wider range of much older ones. I have included some sample CSS hacks that target these old browsers in my "OldBrowsersFix2.css" sheet. My HTML5 tutorial also has sample flex boxes and other goodies for those IE browsers.

* Note: If you want to maximize your cross-browser abilities even more so your pages support even more out-dated browsers and HTML elements, go read my extensive HTML5 tutorial which not only addresses the cutting-edge HTML5 elements and best cross-browser choices you should use today, but picks the best ones that work in older browsers, as well. Here is the link:

https://mitchellstokely.com/HTML5Tutorial/

I also include custom HTML and CSS for building grids in Internet Explorer versions 8-11, as well as cross-browser flex code for them with full HTML and CSS code you can cut-and-paste. I also have solid HTML5 templates that work with my CSS system in modern browsers, but that also work well in many older browsers, as well. If you combine my HTML code with my CSS system, most of your layout and web design issues in all known browsers are solved for you, so you can now put 100% focus on doing cutting-edge CSS3 and HTML5 in your web projects. How fun is that idea! This will save you thousands of hours struggling with cross-browser issues going forward. That was why I built this CSS and HTML system...it is simply a huge time saver! And we all know time is money!!

- Mitchell Stokely


----------------------------------------

HOW TO INSTALL AND LINK TO THE CSS FRAMEWORK IN YOUR WEBSITE

1. Copy and paste the "default" folder of files into your website. 
2. Optional: I recommend you create a "css" parent folder and move the "default" folder inside it in case you want copies of the default folder as a skin later.
3. Add the HTML code below to the <head> section of your HTML page after pasting in the "default" folder of files into your website. Be sure to customize the paths below depending on the final path to your CSS files.

Below is the starting link set I recommend you use. It does not include the Netscape custom style page or the optional Bootstrap cleaner/import set. Only user those if you need them.

    <link media="print" rel="stylesheet" type="text/css" href="css/default/styles/Print.css?v=2.0" />
    <link media="screen" rel="stylesheet" type="text/css" href="css/default/styles/NewBrowsersImporter.css?v=2.0" />
    <link media="screen" rel="stylesheet" type="text/css" href="css/default/styles/OldBrowsers.css?v=2.0" />

Optional: Add these optional styles if designing for old Netscape or need to clear out Bootstrap's reboot element styles, which are incomplete:

    <link media="screen" rel="stylesheet" type="text/css" href="css/default/styles/NetscapeOnly.css" />
    <link media="screen" rel="stylesheet" type="text/css" href="css/default/styles/BootstrapImporter.css?v=2.0" />

----------------------------------------

WHAT DOES EACH CSS FILE DO?

Put all your modern and/or custom CSS in these three (3) files listed below.

These style sheet only affect newer browsers and is where you will place your custom website CSS designs. These files you can also safely minify, compress, use SASS with, customize with classes, use with JavaScript API's, etc. The styles in these three sheets are only seen by newer browsers, including IE 9-11, Edge, Chrome, Firefox, Safari, all mobile browsers, etc. Note that some of the starter CSS code in these sheets works with my new HTML5 template system. You can use my "README.html" source code with these styles and get up and running with my CSS framework fast. Mobile and print designs are built in!

Styles.css - Put all your projects modern web page CSS design code in here, including fonts, classes, etc.

Mobile.css - Put all styles that affect mobile browsers and smart phone browsers in here. Note that the sample code inside is designed to work with my README.html sample page and HTML so try and use that code to make your website fully mobile-friendly!

Print.css - This system comes with a print design framework that allows your whole website to be fully printable. The sample code inside is designed to work with my README.html sample page and HTML so try and use that code to make your website fully printable!

* Note, in addition to the three sheets above, you can customize the HTML element reset sheet listed below - "NewBrowsers.css". It simply enhances/resets the basic HTML element designs for all modern browsers. However, I do not recommend it as I have carefully designed that sheet to style browsers post-2001 to present with styles that work with non-conforming CSS3 agents.

----------------------------------------

DO NOT MODIFY THE SHEETS BELOW

The files below control the designs for all older browsers, resetting their elements, then importing in the style sheets above for newer browsers as well as a modern reset element sheet only they can see.

WARNING: DO NOT MODIFY the CSS files below except to remove comments! That will reduce their size. DO NOT MINIFY OR COMPRESS or the CSS will become corrupted as it uses many custom CSS rules and code that most browsers understand but most modern tools will not understand and corrupt!



OldBrowsers.css - Required. This is the main element reset style sheet for all browsers, old and new. This is one of the files you directly link to in the <link> list above.

OldBrowsersFix1.css - Required. This is is imported by "NewBrowsersImporter" and fixes bugs only for old IE for Macs. This sheet is imported by "NewBrowsersImporter" below.

OldBrowsersFix2.css - Required. This is is imported by "NewBrowsersImporter" and fixes bugs only for old IE 1-7 for Windows. This sheet is imported by "NewBrowsersImporter" below.

NewBrowsers.css - Required. This sheet cleans up and restyles all known HTML5 elements for newer browsers. Note, this sheet is only seen by modern user agents and cascades over the "OldBrowsers" sheet above with more modern element styles tailored for HTML5. It does include a limited CSS style set that works well with a wide range of browsers built since 2001. You can customize or enhance those in this sheet if you like, but it is not recommended. You could enhance an element with new CSS3 styles that then fails in a long list of older browsers. This sheet is imported by "NewBrowsersImporter" below.

NewBrowsersImporter.css - Required. This is the main "importer" style sheet that loads in newer styles sheets for more modern browsers, hiding them for a long list of older browsers, including Internet Explorer 1-7, Netscape series, Old Opera, IE for Mac, and a list of others. This sheet also loads in the styles, mobile, and print sheet pages listed above so they are hidden from older browsers. This is one of the files you directly link to in the <link> list above.


----------------------------------------

OPTIONAL SHEETS 

As above, do NOT modify these sheets below except to remove comments:

BootstrapImporter.css - optional. This sheet imports in the "cleaner" for newer browers only. It then resets the elements back to the browser's cleaner defaults so my style resets work better.

BootstrapCleaner.css - optional. The import sheet above loads this cleaner that resets bootstraps HTML element changes back to the browsers default styles so you start with a clean, uncorrupted element styling.

NetscapeOnly.css -optional. Do not use this sheet unless you really want to custom the base design for old Netscape series (pre-2006). The base oldbrowsers sheet will fix most of netscapes issues.



----------------------------------------

ADDITIONAL COMMENTS: Each of the CSS files in this folder has more detailed comments about how they work, why each selector or CSS rule was chosen, how to import files, how the reset element sheets work, etc. If you want the dirty details, I have added a rich set of instructions inside each. Feel free to delete all my comments when you are ready to move to production. But do NOT minimize or prepreprocess them or the CSS hacks in them will fail.

GOODIES: The "goodies" file has extra code for legacy browsers and tricks you might find helpful.

CREATING SKINS: If you want to create multiple "skins" or theme for your website, just copy the parent "default" folder, give it a new name, change its "styles.css" styles, and link to the folder. That is it! Everything you need to create a new web design is now grouped under one folder. You can even hand this folder of styles, fonts, and images to a designer and they can start customizing the design instantly.
