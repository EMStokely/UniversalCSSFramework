Universal CSS Framework
===============================

Author: Mitchell Stokely

Version: 2.0

---

## License
GNU GENERAL PUBLIC LICENSE VERSION 3

---

## Description

This is a project I call the "Universal CSS Framework". This powerful cascading style sheet (CSS) system supports universal website design in all known web browsers going back to the birth of the World Wide Web in the 1990's. It is simply a small package of CSS files you drag-and-drop into your website and which "resets" the web browser's HTML element designs so they consistently display your website's elements in many types of web browsers. This CSS system also offers you a more advanced CSS system for managing how older and newer browsers view your website's HTML and CSS by hiding modern CSS designs from older browsers and degrading gracefully your HTML layouts for those older user agents. As such, this CSS system has been carefully designed to allow your websites to perform well in 99.99% of web browsers past and present without having to use eleborate custom CSS hacks, install complex JavaScript API libraries, struggle with half-baked polyfills, or implement styles sheet preprocessor dependencies. It uses plain CSS text!

Using this style sheet framework, older browsers will get plain white, vertical content pages with san-serif black fonts, while newer and more modern browsers will get your cutting-edge, CSS3 designs. This system achieves that using special CSS rules that older browsers do not understand. These newer style sheets are hidden from the old browsers using a special `@import` style sheet trick all known modern browsers understand but older ones do not. The older browsers get a simpler reset element style sheet, while modern browsers get a more advanced reset element sheet, plus your custom CSS layout styles. This includes full support for advanced mobile and print designs using CSS. The following older browsers are now hidden from these newer style sheets using `@import` rules in this CSS framework:

* Netscape 1-4.8 
* Opera 1-3.5
* Windows Internet Explorer 1-7.x
* Macintosh Internet Explorer 2-4.5
* Konqueror 1-2.1
* Windows Amaya 1-5.1
* iCab 1-2
* OmniWeb
* Many more antiquated browsers...

### Print, Mobile, and Web Accessibility Features

My solution also supports many other goodies most CSS frameworks leave out, including full print-to-paper website translation, small screen support, and accessibility.

The Universal CSS Framework allows your website to be fully printable! It comes with styles that turn on and off non-printing HTML5 structural elements in your web page, then adds enhancements that change HTML elements like tables and other features to a print-friendly design. Your customers or internal staff can now see your web content displayed perfectly on the printed page, as well! It comes with a fully customizeable print header, contact and copyright info, and landscape/portrait print-friendly design support. If your CSS is not helping your viewers print every page of your website content, then it is not a true CSS system. To support this feature you will need to use modern HTML5 layouts like those found in my README.HTML page or in my online HTML5 Tutorial (below).

This CSS system also has a build in mobile style sheet you can customize for smart phone or small device viewports. My version is supported in older browsers unlike many of the ones built today.

Finally, my code also enhances HTML5 and WAI-ARIA attributes when used with the HTML5 attributes found in the README.html file. My HTML5 Tutorial below demonstrates how to use ARIA the right way, as well.

With this CSS solution, I aim to deliver simple, cut-and-paste HTML and CSS code that new web developers can use with minimal customization. My CSS framework will allow you to deliver viewable content in 20+ years worth of historical browsers, while allowing your teams to safely move forward with cutting-edge web technology used in the browsers of tomorrow.

### Check Out My Modern HTML5 Tutorial

CSS requires knowledge of HTML. The two are brothers and must be carefully designed as one unit to balance and enhance each other. Too many new developers are not understanding how the two work together because they are not taught the 20 year history of HTML and CSS, which has evolved. I have posted a complete HTML5 Tutorial on my website to help you!

My online tutorial has HTML which works well with this CSS system and many others. the code there takes care of nearly all of the issues in outdated browsers and works well with the cutting-edge ones. It also "speeds up" parsing and rendering of the CSS/HTML in all browser displays, which is important.

It has a complete modern HTML5 element sample coding list, history of every HTML element since the 1990's, a "Best Practices" section, template web pages with cross-browser grids/flex examples, recommended markup attributes, WAI-ARIA attributes for the blind, and lists of HTML/CSS code to avoid that still is not supported in modern HTML5 browsers. What is even better is my HTML5 code works perfectly with this Universal CSS Framework! Using the two systems combined (HTML and CSS), you can deliver powerful cross-browser web pages that load lightning fast and parse perfectly in browsers, past and present. You can even use my README.html page in this project as an HTML5 template, as it has all the same "best practices" markup code. Or simply visit my HTML5 Tutorial link below for all the goodies!

[View my HTML5 Tutorial >>>](https://mitchellstokely.com/HTML5Tutorial/)

If you want to get more detailed information about this project, you will have to copy my code then view my "README.html" file. It is written in clean HTML5 markup, can be opened in any web browser, and is styled by the CSS system found in this project. It is superior to GitPages, Jekyll, Markdown, and all the other goofy new frameworks that require complicated coding, settings, and other routines to work. Stick with plan CSS and HTML and you always widen your viewing audience!

---

### How to Install

For more detailed information on the installation of these files, be sure to go to my README.html file, or the README.txt text file inside the Styles folder for more information.

This CSS solution is just "text files" so you do not install anything, just drag and drop the folder of files into your web project and link to a couple of them from the head of your web pages. That is it! But here is a few more details to guide you:

1. `Copy the CSS folder into your Web Project` - First copy-and-paste the "default" folder of files anywhere inside your website. I like to create a "css" folder first and drag the "default" folder into it. This allows you to make copies the the "default" folder of CSS files later and use them as a "skin" or theme.

2. `Add HTML links to the CSS` - Below is how you  link to the "Universal CSS Framework" from an HTML web page. Paste these links below into the head section of your HTML web page and modify the paths as needed so they link to the files show below:

&lt;html&gt;<br />
&lt;head&gt;

&lt;link media="print" rel="stylesheet" type="text/css" href="css/default/styles/Print.css?v=2.0" /&gt;<br />

&lt;link media="screen" rel="stylesheet" type="text/css" href="css/default/styles/NewBrowsersImporter.css?v=2.0" /&gt;<br />

&lt;link media="screen" rel="stylesheet" type="text/css" href="css/default/styles/OldBrowsers.css?v=2.0" /&gt;

&lt;/head&gt;<br />
...

That's it!

* Note that there are other optional CSS files you can add to the link list above but these are the basic ones you need. Go read my REAME.txt file inside the Styles Folder for more details.

### Add your CSS Code as Needed inside the 'Styles.css'

When adding your custom styles to the framework, just go to the "default/styles" folder and paste in your custom styles and classes into "Styles.css". Do the same for the "Mobile.css" layout version, and modify the "Print.css" file so your web pages are perfectly printable. Note that the project only comes with basic mobile-friendly and print-friendly layout designs. All these default designs match the HTML in my README.HTML layout code, or the one found inside my HTML5 Tutorial (link above). So use thuse HTmL web pages to get started with a clean markup template that works well with my CSS system.

Additionally, you can add your own mobile app images, print button, favicon, header logo, and high definition print logo inside the Images or Content folder. I have included samples in the "images" folder. There are lots of goodies to customize in the "styles" CSS folder.



## Go Read My HTML File

#### Sorry, Im not a fan of Markdown. *It is a redundant format when we have HTML as a superior static browser format with much better control.* Please view my "README.html" file instead of this "README.md" file for more project details. You will have to download the full project of files to your desktop to view it in your web browser as the GitHub "readme" system does not even understand basic HTML or CSS!

---