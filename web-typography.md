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



###Font Style
`font-style: normal`
`font-style: italic`

###Leading
`line-height`
* The space between lines of text is referred to as leading in print typography, and refers to the distance between the baselines of successive lines of type. Strips of lead used to be used to separate the lines of type from another and increase the line height.
* Leading or line-height can be used to increase readability of type. Greater space between lines of type means that the eye can more easily pick out type with a smaller x-height, and follow long-form type better.
* Set using line-height in CSS: `line-height: 1.2em; /  line-height: 120%`;

###Decorative, Heading and Body Fonts

###Glyphs

###Typographer's Quotes


A Brief History of Typography
-----------------------------


History of Web Typography
-------------------------

###Font Availability



###Screen Limitations
Popular web fonts (Arial, Verdana, Georgia, and Times New Roman) are such not only because of their wide availability, but because they are drawn with the screen’s limitations in mind. Georgia reads better on screen than Garamond primarily because it has a higher x-height (the height of an “x”), and – as a result – a larger eye.

Computers only used to have 256 colours avaiable, and low resolution screens (most of the web used to be optimised for 72dpi). With almost all monitors now displaying 16million colours and rendering type edges much more smoothly, a greater range of fonts render better. Tablets and phones now also display at much closer to print quality.
[David Kadavy] [2]


Using Type Online
-----------------

###Typekit
* Subscription based service providing commercial typefaces. Now part of Adobe's Creative Cloud offering.
* Limited range of type foundries, although this does appear to be growing. Does not include Monotype of Linotype typefaces (separate services).
* Javscript based font availability: typekit-generated JS allows selected font-faces to be used in CSS.
Find out more [typekit.com](http://typekit.com)

###MyFonts
* Selling one-off perpetual licenses to use commercial typefaces online. Allows you to download a webfont kit and host on your sites.
* Typefaces from Monotype and Linotype are provided on a pay-as-you-go basis, rather than one-off licences.
Find out more [myfonts.com](http://www.myfonts.com)

###MyFonts
* Commercial offering from Monotype.
* Allows web and print font packages.
* Provides JS, CSS and self-hosting options.
[fonts.com/web-fonts](http://www.fonts.com/web-fonts)

###Google Fonts
* Provides open-source fonts for free.
* Really good options to test drive typefaces, compare sets and examine character sets.

###Fontdeck
* Subscription based option, with annual pricing per font, and a bandwidth supplement for sites with over 2 million page impressions a month.
* Typefaces from a range of small foundries and type designers.
* CSS based option.
[fontdeck.com](http://fontdeck.com/)

###Webtype
* Subscription service, with pricing levels based on the number of page impressions.
* Good range of fonts from the larger type foundries, including Monotype.
* CSS based option.
[webtype.com](http://www.webtype.com/)


###Typecast
* Test drive fonts from fonts.com, Google, MyFonts, TypeKit, Webtype and FontDeck.
* Paid for service, but Personal and Team packages include a Fonts.com plan.

###Font Squirrel

###Cufon

###The League of Movable Type



***

References
----------
[1]: http://www.w3schools.com/css/css_font.asp] "W3Schools"
[2]: http://kadavy.net/blog/posts/design-for-hackers-why-you-dont-use-garamond-on-the-web/ "David Kadavy"
