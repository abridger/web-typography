Web Typography
==============

Type Basics
-----------

###Font Face / Font Family
`font-family`
* A font is a specific alphabet (set of glyphs) in a specific face, weight and size. So 10pt Garamond Bold would be one font, 12pt Garamond Italic would be another. Fonts are grouped together in collections of similarly designed faces called font families or typefaces - what we generally think of as a font (Arial, Helvetica, Caslon, Bodoni, etc.)


###Serif, Sans-serif and Monospace
* Serifs are small projections attached to the ends of strokes that make up each character. Serifed fonts were generally used for print body text, as they were thought to increase readability, although there is now debate about this. Sans-serif fonts have generally been thought to be more readable on screen, as serifs aren&rsquo;t always rendered well on lower resolution screens.
* Sans-serif fonts obviously don&rsquo;t have serifs.
* Monospace fonts are those in which every glyph occupies the same width (unlike other fonts in which glphs are different widths).


###Glyphs
* A glyph is an unique symbol within a font to represent a letter, number or punctuation.
* Different glyphs can be used to represent the same character or set of characters &ndash; uppercase, lowercase, ligatures, stylistic variations.
* Not all fonts or families will have a complete set of glyphs, so it&rsquo;s possible that some of the characters you would like to used may be missing.
* Some specialised typefaces have very specific sets of glyphs &ndash; icon fonts are becoming much more common in order to handle high resolution displays.


###Font Size
`font-size`
* In print, this is described in points or picas, but on the web it is described in pixels or ems.
* This can be set with pixel height, but it&rsquo;s recommended to use em rather than pixels to allow users to resize the text in the browser menu. Em units are recommended by W3C. 1em is equal to the current font size. The default text size in browsers is 16px. So, the default size of 1em is 16px.
* Unfortunately, there is still a problem with older versions of IE and ems. The text becomes larger than it should when made larger, and smaller than it should when made smaller. The solution that works in all browsers, is to set a default font-size in percent for the <body> element and then use ems to set the size of specific elements in the body:

`body {font-size: 100%;}`

`h1 {font-size: 2.5em;}`

[W3Schools] [1]

###X-Height
* This is the distance between the baseline and the mean line of lower-case letters in a typeface, which is generally the height of the letter x.
* Different fonts will have different x heights at a similar size, which will affect their readability and overall impact.
* CSS does have an `ex` unit, which is realtive to the x-height of the current font, but different browsers handle this extremely differently and it&rsquo;s rarely used.

###Measure & Responsive Typography
* The length of a line of text.
* For a singe column layout, the measure should be between 45 and 75 characters, with the optimimum generally considered to be 65 characters per line.

[Smashing Magazine] [2]

###Font Style
`font-style: normal`

`font-style: italic`

###Leading/Line-height
`line-height`
* The space between lines of text is referred to as leading in print typography, and refers to the distance between the baselines of successive lines of type. Strips of lead used to be used to separate the lines of type from another and increase the line height.
* Leading or line-height can be used to increase readability of type. Greater space between lines of type means that the eye can more easily pick out type with a smaller x-height, and follow long-form type better.
* The key difference between print leading and web line-height is that leading is measured from baseline to baseline (type is aligned on the baseline) whereas CSS `line-height` aligns type evenly between baselines. Increasing leading therefore increases the space only below a line of type; increasing `line-height` increases the space above and below a line of type.
* Set using line-height in CSS: `line-height: 1.2em;` or `line-height: 120%`
* `line-height` can be used to set an approximation of the baseline grid for a page, and to control vertical rythmn. Guy Routledge recommends setting a line-height measure on the `body` tag, which is then inherited by child elements. Setting a unit-less line-height means that, in child elements, the line-height will be a factor of of the initial line-height and the element&rsquo;s font-size. This gives a consistent vertical rhytmn across the document. 

[A to Z CSS] [3]

###Kerning
The space between individual characters, adjusted to increase readability and improve visual appeal. Particularly in letter combinations such as AW, AV, Yo, and with punctuation that is often brought under overhanging parts of other characters.

###Tracking
`letter-spacing`
Tracking is the space between all characters in a line or paragraph, which can be set with the `letter-spacing` CSS attribute, adding or subtracting space between characters:

`h1 { letter-spacing: 2px; }`
`h2 { letter-spacing: -3px; }`

[W3 Schools] [4]

###Typographic Hierarchy
Documents should be structured typographically, as well as semantically using different sizes and weights for the different heading levels:

`<h1> <h2> <h3> <h4> <h5> <h6>`


###Readability
Readability is a combination of font face and size, leading, and measure. The appropriate font size will depend on the x-height of the chosen font family and the weight of stroke in individual faces.

Leading also needs to be adjusted depending on x-height and weight to provide sufficient white space between lines of text. Too much leading however, and it becomes difficult for the eye to follow. Tracking or letter spacing can also be used to increase the readability of particularly heavy, or small faces.

As mentioned above, measure should be between 45 and 75 characters, although can vary within this depending on the chosen font family and leading.

The right level of contrast also affects readability. A heavy, black face on a stark white background will be harder to read for long periods of time. Consider lower levels of contrast, with less heavy faces, or slightly tinted backgrounds &ndash; as with the creamy paper of many books.


###Column Layouts
`column-count`

`column-width`

`columns`

`column-gap`

There are two CSS properties to control whether and how many columns will appear. `column-count` sets the number of columns to a particular number, and `column width` sets the minimum desier column width. If `column-count` isn&rsquo;t set, the browser will automatically make as many columns to fit the available width. These can both be replaced or combine in `columns`. To set the gap between columns, you can use `column-gap`.

[MDN Developer Network] [5]


####Typographer&rsquo;s Quotes
Text should use typographer&rsquo;s quotes/smart quotes/curly quotes wherever possible:

* Single opening quote: `&lsquo;` or `&#8216;`
* Single closing quote: `&rsquo;` or `&#8217;`
* Double opening quote: `&ldquo;` or `&#8220;`
* Double closing quote: `&rdquo;` or `&#8221;`


For measurements map coordinates, time and measurements in feet and inches, you should use primes &ndash; eg. 40&deg; 44&prime; 54.3588&Prime; N, 73&deg; 59&prime; 8.3616&Prime; W.

* Single prime: `&prime;` or `&#8242;`
* Double prime: `&Prime;` or `&#8243;`

####Hyphens and Dashes
Hyphens are a punctuation mark, used to combine compound words, and separate words across lines. They shouldn&rsquo;t be confused with the two typographic dashes, N and M dashes.

An en dash or N dash is typically the width of the capital N character in a given typeface. En dashes indicates range of values (eg. 2014&ndash;2015) or connection between words (eg. Anglo&ndash;American relations), both unspaced. It can also be used parenthetically, with spaces (eg. She looked &ndash; with deep regret &ndash; at the terrible punctuation). En dashes are much more common in the UK, and em dashes are rarely used.
* N dash: `&ndash;` or `&#8211;`

An em dash or M dash is typically the width of the capital M character in a given typeface. Em dashes are much more common in the US, where they are used un-spaced to break up parts of a sentence/in place of parentheses (eg. She looked&mdash;with deep regret&mdash;at the terrible punctuation).
* M dash: `&mdash;` or `&#8212;`

Hyphenation can be controlled in CSS in Chrome with the `word-break` property, although this isn&rsquo;t implemented in Firefox:
* `break-all` &ndash; lines are allowed to break between any two letters
* `keep-al` &ndash; lines cannot break

The CSS `hyphens` property is supported in Firefox and other Webkit browsers which ship with hyphenation dictionaries. This is dependent on the hyphenation dictionary though (not available in all languages), and requires the language to be specified inthe HTML or article tag: `<html lang="en">` / `<article lang="en">`:
`-webkit-hyphens: auto;`

`-moz-hyphens: auto;`

`-ms-hyphens: auto;`

`-o-hyphens: auto;`

`hyphens: auto;`

There is also a Javascript library available for injecting hyphens into documents, hyphenator.js (more below).

[Practical Typography] [6]

####A Hyphen is not a Minus Sign...
Yep, that&rsquo;s right, subtraction operators are distinct from hyphens, and multiplication symbols are distinct from Xs:

* Addition: `&#43;`
* Subtraction: `&minus;` or `&#8722;`
* Multiplication: `&times;` or `&#215;`
* Division: `&divide;` or `&#247;`

Fractions should also be rendered in their &lsquo;vulgar&rsquo; form if possible, rather than written out with a slash &ndash; eg. &frac12; rather than 1/2 or &#8531; rather than 1/3.

* One half: `&frac12;` or `&#189;`
* One third: `&#8531;`
* Two thirds: `&#8532;`
* One quarter: `&frac14;` or `&#188;`
* One tenth: `&#8530;`

Past Limitations on Web Typography
-------------------------

###Font Availability
Few fonts are available across almost all  systems, and therefore guaranteed to display consistently for all users. The following can probably br relied upon &ndash; all others should be provided via `@font-face`, depending on licensing:

####Sans-serif
* Arial
* Arial Black
* Tahoma
* Trebuchet
* Verdana

####Serif
* Georgia
* Times New Roman

####Monospaced
* Courier

[CSS Font Stack] [7]

###Screen Limitations
Popular web fonts (Arial, Verdana, Georgia, and Times New Roman) are such not only because of their wide availability, but because they are drawn with the screen’s limitations in mind. For example, Georgia reads better on screen than Garamond primarily because it has a higher x-height, and therefore a larger eye.

Computers only used to have 256 colours avaiable, and low resolution screens (the web is generally optimised for 72dpi). With almost all monitors now displaying 16million colours and rendering type edges much more smoothly, a greater range of fonts render better. Tablets and phones now also display at much closer to print quality.

Thanks to [David Kadavy] [8]


Using Webfonts
--------------
###Font Face
Font face is the CSS property used to specify a font and the URL where it can be found:

`@font-face {
	font-family: 'Open Sans';
	font-style: normal;
	font-weight: 400;
	src: url(http://fonts.gstatic.com/s/opensans/v10/K88pR3goAWT7BTt32Z01m5Bw1xU1rKptJj_0jans920.woff2) format('woff2');
	unicode-range: U+0460-052F, U+20B4, U+2DE0-2DFF, U+A640-A69F;
	}`

Font files can be stored locally, with the `src` property of the CSS tag pointing to the relative address, or externally hosted on a CDN, as above with the Google Font Open Sans.

If you are using a service like Google Fonts, which provides a link to an external stylesheet then you can use the `font-family` property as normal in your stylesheets:

* Stylesheet link: `<link href='http://fonts.googleapis.com/css?family=Open+Sans' rel='stylesheet' type='text/css'>`
* CSS import: `@import url(http://fonts.googleapis.com/css?family=Open+Sans);`

```h1 {
	font-family: 'Open Sans', sans-serif;
	font-weight: 400;
	}```

To maximise compatability across browsers, you can specify multiple source files for in the `@font-face` property:

		```src: url('fonts/FontName.eot');
		src: url('fonts/FontName.eot?#iefix') format('embedded-opentype'),
		url('fonts/FontName-webfont.woff') format('woff'),
		url('fonts/FontName-webfont.ttf') format('truetype'),
		url('fonts/FontName-webfont.svg#FontName') format('svg');```

#####Browser support as of 1/1/2015:
* EOT - Embedded OpenType fonts: IE8 upwards.
* WOFF - Web Open Type Format: all current browsers except Opera Mini.
* SVG fonts: Safari (desktop and mobile) and Android.
* TTF/OTF - TrueType and OpenType fonts: support in all current browsers, except Opera Mini. Partial support in IE.
* WOFF 2.0 - Web Open Type Format: support in newer versions of Chrome, Opera an Android. Can be enabled in newer developer versions of Firefox.


Doing More with Type Online
---------------------------

###General/All Purpose

####[Lettering.js](http://letteringjs.com/)
* A lightweight, easy to use Javascript span injector for radical Web Typography.
* Provides a solution for custom type headings, while keeping the text selectable.
* Allows styling to be applied to individual letters and allow for kerning using relative positioning and left/right margins.

#####Examples:
* http://trentwalton.com/2011/05/10/fit-to-scale/
* http://garann.com/allgirlhacknight/invite.html
* http://lostworldsfairs.com/atlantis/

###Responsive Text

####[FlowType.js](http://simplefocus.com/flowtype)
A jQuery plugin that changes the font size based on a specific element&rsquo;s width to try and maintain legibility and maintain the same character-per-line length. It sets minimum and maximum width threshholds.

####[Squishy](http://cmsauve.com/projects/squishy/)
A jQuery plugin that automatically resizes text to exactly fit the container.

####[FitText](http://fittextjs.com/)
A jQuery plugin for making scalable headlines that fill the width of a parent element. Only for headers, not paragraph text.

####[Slabtext](http://freqdec.github.io/slabText/)
A jQuery plugin for producing big, responsive headlines. It works by splitting headlines into rows before resizing each row to fill the available horizontal space.

####[Hatchshow](http://charliepark.org/hatchshow/)
A jQuery plugin to balance measures. Like Slabtext, it can be used to create big, bold headlines.

####[ResponsiveText](https://github.com/ghepting/jquery-responsive-text)
A jQuery plugin to set font sizes responsively based on its container width. Unlike Squishy, FitText or Slabtext, it can be used with paragraph text.

###Text Positioning and Wrapping

####[Bacon](http://baconforme.com/)
A jQuery plugin that allows for text to be wrapped around a bezier curve or a line.

####[jQSlickWrap](http://www.jwf.us/projects/jQSlickWrap/)
A jQuery plugin that allows for text to be wrapped around the content of floated images.

###Text Animations

####[Textillate](http://jschr.github.io/textillate/)
Built on top of animate.css and lettering.js libraries to apply CSS3 animations to text.

####[Animate.css](http://daneden.github.io/animate.css/)
A library of cross-browser CSS animations.

####[Super Simple Text Rotator](http://www.thepetedesign.com/demos/jquery_super_simple_text_rotator_demo.html#)
A quick and easy way to add rotating text.

####[Flipping Text](https://github.com/peachananr/flipping_text)
Creates a ticking intro animation.

###Kerning

####[Kerning.js](http://kerningjs.com/)
A jQuery plugin that allows for text to be kerned correctly.
* Allows letter placing to be individually adjusted for perfect kerning.
* Allows the adjustment of individual character sizes, and for transformations to be applied to individual characters.
* Selective colouring, and conditional formatting.

####[Type Butter](http://typebutter.com/)
A jQuery plugin that allows for optical kerning for webfonts.

###Hyphenation
####[Hyphenator JS](https://code.google.com/p/hyphenator/)
A Javascript library that injects hypehns using a large hyphenation dictionary.

###Identifying fonts

####[ffffallback](http://ffffallback.com/)
Bookmarklet that allows you to identify webfonts on a site and test different fallback font choices.

####[Fontface Ninja](http://www.fontface.ninja/)
Chrome plugin for identifying fonts on a page. Slightly slicker and more detailed than WhatFont below.

####[WhatFont](https://chrome.google.com/webstore/detail/whatfont/jabopobgcpjmedljpbcaablpmlmfcogm?hl=en)
Another Chrome plugin for identifying fonts on a pge.

Type Sources
-----------------

###[Typekit](http://typekit.com)
* Subscription based service providing commercial typefaces. Now part of Adobe&rsquo;s Creative Cloud offering.
* Limited range of type foundries, although this does appear to be growing. Does not include Monotype of Linotype typefaces (separate services).
* Javscript based font availability: typekit-generated JS allows selected font-faces to be used in CSS.

###[MyFonts](http://www.myfonts.com)
* Selling one-off perpetual licenses to use commercial typefaces online. Allows you to download a webfont kit and host on your sites.
* Typefaces from Monotype and Linotype are provided on a pay-as-you-go basis, rather than one-off licences.

###[Fonts.com](http://www.fonts.com/web-fonts)
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


Identifying Fonts (and pinching ideas)
-----------------

###[What the Font] (http://www.myfonts.com/WhatTheFont/)
* Useful for identifying typefaces from images uploaded to the site.

###[Identifont] (http://www.identifont.com/)
* Useful for browsing and identifying typefaces by appearance, or similarity to others. The questionnaire for identifying typefaces is often quite accurate, or at least good for exploring other options.


[1]: http://www.w3schools.com/css/css_font.asp] "W3Schools"
[2]: http://www.smashingmagazine.com/2014/09/29/balancing-line-length-font-size-responsive-web-design/#more-202415 "Smashing Magazine - Size Matters: Balancing Line Length And Font Size In Responsive Web Design"
[3]: http://www.atozcss.com/the-css-line-height-property/ "Line-height"
[4]: http://www.w3schools.com/cssref/pr_text_letter-spacing.asp "CSS letter-spacing Property"
[5]: https://developer.mozilla.org/en-US/docs/Web/Guide/CSS/Using_multi-column_layouts "Using CSS multi-column layouts"
[6]: http://practicaltypography.com/hyphens-and-dashes.html "hyphens and dashes"
[7]: http://www.cssfontstack.com/
[8]: http://kadavy.net/blog/posts/design-for-hackers-why-you-dont-use-garamond-on-the-web/ "David Kadavy"
