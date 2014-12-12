Web Typography
==============

Type Basics
-----------
* font face vs font family
* serif, sans-serif and monospace
* font classifations
* font weight
* x-height

###Font Size
`font-size`
* In print, this is described in points or picas, but on the web it is described in pixels or ems.
* This can be set with pixel height, but it's recommended to use em rather than pixels to allow users to resize the text in the browser menu. Em units are recommended by W3C. 1em is equal to the current font size. The default text size in browsers is 16px. So, the default size of 1em is 16px.
* Unfortunately, there is still a problem with older versions of IE and ems. The text becomes larger than it should when made larger, and smaller than it should when made smaller. The solution that works in all browsers, is to set a default font-size in percent for the <body> element and then use ems to set the size of specific elements in the body:

`body {font-size: 100%;}
h1 {font-size: 2.5em;}`


[W3Schools] [1]

###X-Height

###Measure & Responsive Typography
* The length of a line of text.
* For a singe column layout, the measure should be between 45 and 75 characters, with the optimimum generally considered to be 65 characters per line.

[Smashing Magazine] [2]

###Font Style
`font-style: normal`
`font-style: italic`

###Leading
`line-height`
* The space between lines of text is referred to as leading in print typography, and refers to the distance between the baselines of successive lines of type. Strips of lead used to be used to separate the lines of type from another and increase the line height.
* Leading or line-height can be used to increase readability of type. Greater space between lines of type means that the eye can more easily pick out type with a smaller x-height, and follow long-form type better.
* Set using line-height in CSS: `line-height: 1.2em;` or `line-height: 120%`;

###Decorative, Heading and Body Fonts


###Glyphs

###Typographic Hierarchy

###Readability

###A Couple of Pedantic Points...

####Typographer's Quotes
* Ideally, text should use typographer's quotes (curly quote marks)

####Hyphens, N-Dashes and M-Dashes


A Brief History of Typography
-----------------------------


History of Web Typography
-------------------------

###Font Availability



###Screen Limitations
Popular web fonts (Arial, Verdana, Georgia, and Times New Roman) are such not only because of their wide availability, but because they are drawn with the screen’s limitations in mind. For example, Georgia reads better on screen than Garamond primarily because it has a higher x-height, and therefore a larger eye.

Computers only used to have 256 colours avaiable, and low resolution screens (the web is generally optimised for 72dpi). With almost all monitors now displaying 16million colours and rendering type edges much more smoothly, a greater range of fonts render better. Tablets and phones now also display at much closer to print quality.

Thanks to [David Kadavy] [3]


Using Webfonts
--------------



Doing More with Type Online
---------------------------

###[Lettering.js](http://letteringjs.com/)
* A lightweight, easy to use Javascript span injector for radical Web Typography.
* Provides a solution for custom type headings, while keeping the text selectable.
* Allows styling to be applied to individual letters and allow for kerning using relative positioning and left/right margins.

####Examples:
* http://trentwalton.com/2011/05/10/fit-to-scale/
* http://garann.com/allgirlhacknight/invite.html
* http://lostworldsfairs.com/atlantis/


###[Kerning.js](http://kerningjs.com/)
* Allows letter placing to be individually adjusted for perfect kerning.
* Allows the adjustment of individual character sizes, and for transformations to be applied to individual characters.
* Selective colouring, and conditional formatting.

###[FlowType.js](http://simplefocus.com/flowtype/)
* Changes the font size based on a specific element's width to try and maintain legibility and maintain the same character-per-line length.
* Sets minimum and maximum width threshholds

###[ffffallback](http://ffffallback.com/)
* Bookmarklet that allows you to identify webfonts on a site and test different fallback font choices.

Type Sources
-----------------

###[Typekit](http://typekit.com)
* Subscription based service providing commercial typefaces. Now part of Adobe's Creative Cloud offering.
* Limited range of type foundries, although this does appear to be growing. Does not include Monotype of Linotype typefaces (separate services).
* Javscript based font availability: typekit-generated JS allows selected font-faces to be used in CSS.

###[MyFonts](http://www.myfonts.com)
* Selling one-off perpetual licenses to use commercial typefaces online. Allows you to download a webfont kit and host on your sites.
* Typefaces from Monotype and Linotype are provided on a pay-as-you-go basis, rather than one-off licences.

###[MyFonts](http://www.fonts.com/web-fonts)
* Commercial offering from Monotype.
* Allows web and print font packages.
* Provides JS, CSS and self-hosting options.

###[Google Fonts](http://www.google.com/fonts)
* Provides open-source fonts for free.
* Offers a wide range of font weights.
* Really good options to test drive typefaces, compare sets and examine character sets.
* Provides JS and CSS options for importing fonts to your site - either by specifying an external stylesheet, or importing font rules into your current stylesheet with `@import url`.

###[Fontdeck](http://fontdeck.com/)
* Subscription based option, with annual pricing per font, and a bandwidth supplement for sites with over 2 million page impressions a month.
* Typefaces from a range of small foundries and type designers.
* CSS based option.

###[Webtype](http://www.webtype.com/)
* Subscription service, with pricing levels based on the number of page impressions.
* Good range of fonts from the larger type foundries, including Monotype.
* CSS based option.

###[Typecast](http://typecast.com/)
* Test drive fonts from fonts.com, Google, MyFonts, TypeKit, Webtype and FontDeck.
* Paid for service, but Personal and Team packages include a Fonts.com plan.

###[Font Squirrel](http://www.fontsquirrel.com/)
* Open source webfont kit generator.
* Provides open source fonts for use on the web, as well as a webfont generator to assemble webfont packages from uploaded fonts.
* Good, well-tagged directory with samples and clear licensing.

###[The League of Movable Type](https://www.theleagueofmoveabletype.com/)
* Innovative font foundry providing well-made, free & open-source, @font-face ready fonts.
* Great source of interesting and distinctive fonts.



[1]: http://www.w3schools.com/css/css_font.asp] "W3Schools"
[2]: http://www.smashingmagazine.com/2014/09/29/balancing-line-length-font-size-responsive-web-design/#more-202415 "Smashing Magazine - Size Matters: Balancing Line Length And Font Size In Responsive Web Design"
[3]: http://kadavy.net/blog/posts/design-for-hackers-why-you-dont-use-garamond-on-the-web/ "David Kadavy"
