# adithyanair2001.github.io
HTML markup consists of several key components, including those called tags (and their attributes), character-based data types, character references and entity references. HTML tags most commonly come in pairs like <h1> and </h1>, although some represent empty elements and so are unpaired, for example <img>. The first tag in such a pair is the start tag, and the second is the end tag (they are also called opening tags and closing tags).

Another important component is the HTML document type declaration, which triggers standards mode rendering.

The following is an example of the classic "Hello, World!" program:

<!DOCTYPE html>
<html>
  <head>
    <title>This is a title</title>
  </head>
  <body>
    <div>
        <p>Hello world!</p>
    </div>
  </body>
</html>
The text between <html> and </html> describes the web page, and the text between <body> and </body> is the visible page content. The markup text <title>This is a title</title> defines the browser page title, and the tag <div> defines a division of the page used for easy styling.

The Document Type Declaration <!DOCTYPE html> is for HTML5. If a declaration is not included, various browsers will revert to "quirks mode" for rendering.[70]

Elements
Main article: HTML element
HTML documents imply a structure of nested HTML elements. These are indicated in the document by HTML tags, enclosed in angle brackets thus: <p>.[71][better source needed]

In the simple, general case, the extent of an element is indicated by a pair of tags: a "start tag" <p> and "end tag" </p>. The text content of the element, if any, is placed between these tags.

Tags may also enclose further tag markup between the start and end, including a mixture of tags and text. This indicates further (nested) elements, as children of the parent element.

The start tag may also include attributes within the tag. These indicate other information, such as identifiers for sections within the document, identifiers used to bind style information to the presentation of the document, and for some tags such as the <img> used to embed images, the reference to the image resource in the format like this: <img src="example.com/example.jpg"

Some elements, such as the line break <br>, or <br /> do not permit any embedded content, either text or further tags. These require only a single empty tag (akin to a start tag) and do not use an end tag.

Many tags, particularly the closing end tag for the very commonly used paragraph element <p>, are optional. An HTML browser or other agent can infer the closure for the end of an element from the context and the structural rules defined by the HTML standard. These rules are complex and not widely understood by most HTML coders.

The general form of an HTML element is therefore: <tag attribute1="value1" attribute2="value2">''content''</tag>. Some HTML elements are defined as empty elements and take the form <tag attribute1="value1" attribute2="value2">. Empty elements may enclose no content, for instance, the <br> tag or the inline <img> tag. The name of an HTML element is the name used in the tags. Note that the end tag's name is preceded by a slash character, /, and that in empty elements the end tag is neither required nor allowed. If attributes are not mentioned, default values are used in each case.

Element examples
See also: HTML element
Header of the HTML document: <head>...</head>. The title is included in the head, for example:

<head>
  <title>The Title</title>
  <link rel="stylesheet" href="stylebyjimbowales.css" /> <!-- Imports Stylesheets -->
</head>
Headings: HTML headings are defined with the <h1> to <h6> tags with H1 being the highest (or most important) level and H6 the least:

<h1>Heading level 1</h1>
<h2>Heading level 2</h2>
<h3>Heading level 3</h3>
<h4>Heading level 4</h4>
<h5>Heading level 5</h5>
<h6>Heading level 6</h6>
The Effects are:

Heading Level 2
Heading Level 3
Heading Level 4
Note that CSS can drastically change the rendering.

Paragraphs:

<p>Paragraph 1</p> <p>Paragraph 2</p>
Line breaks: <br>. The difference between <br> and <p> is that <br> breaks a line without altering the semantic structure of the page, whereas <p> sections the page into paragraphs. The element <br> is an empty element in that, although it may have attributes, it can take no content and it may not have an end tag.

<p>This <br> is a paragraph <br> with <br> line breaks</p>
This is a link in HTML. To create a link the <a> tag is used. The href attribute holds the URL address of the link.

<a href="https://www.wikipedia.org/">A link to Wikipedia!</a>
Inputs:

There are many possible ways a user can give input/s like:

<input type="text" /> <!-- This is for text input -->
<input type="file" /> <!-- This is for uploading files -->
<input type="checkbox" /> <!-- This is for checkboxes -->
Comments:

<!-- This is a comment -->
Comments can help in the understanding of the markup and do not display in the webpage.

There are several types of markup elements used in HTML:

Structural markup indicates the purpose of text
For example, <h2>Golf</h2> establishes "Golf" as a second-level heading. Structural markup does not denote any specific rendering, but most web browsers have default styles for element formatting. Content may be further styled using Cascading Style Sheets (CSS).[72]
Presentational markup indicates the appearance of the text, regardless of its purpose
For example, <b>boldface</b> indicates that visual output devices should render "boldface" in bold text, but gives little indication what devices that are unable to do this (such as aural devices that read the text aloud) should do. In the case of both <b>bold</b> and <i>italic</i>, there are other elements that may have equivalent visual renderings but that are more semantic in nature, such as <strong>strong text</strong> and <em>emphasized text</em> respectively. It is easier to see how an aural user agent should interpret the latter two elements. However, they are not equivalent to their presentational counterparts: it would be undesirable for a screen-reader to emphasize the name of a book, for instance, but on a screen such a name would be italicized. Most presentational markup elements have become deprecated under the HTML 4.0 specification in favor of using CSS for styling.
Hypertext markup makes parts of a document into links to other documents
An anchor element creates a hyperlink in the document and its href attribute sets the link's target URL. For example, the HTML markup <a href="https://www.google.com/">Wikipedia</a>, will render the word "Wikipedia" as a hyperlink. To render an image as a hyperlink, an img element is inserted as content into the a element. Like br, img is an empty element with attributes but no content or closing tag. <a href="https://example.org"><img src="image.gif" alt="descriptive text" width="50" height="50" border="0"></a>.
Attributes
Main article: HTML attribute
Most of the attributes of an element are name-value pairs, separated by = and written within the start tag of an element after the element's name. The value may be enclosed in single or double quotes, although values consisting of certain characters can be left unquoted in HTML (but not XHTML).[73][74] Leaving attribute values unquoted is considered unsafe.[75] In contrast with name-value pair attributes, there are some attributes that affect the element simply by their presence in the start tag of the element,[6] like the ismap attribute for the img element.[76]

There are several common attributes that may appear in many elements :

The id attribute provides a document-wide unique identifier for an element. This is used to identify the element so that stylesheets can alter its presentational properties, and scripts may alter, animate or delete its contents or presentation. Appended to the URL of the page, it provides a globally unique identifier for the element, typically a sub-section of the page. For example, the ID "Attributes" in https://en.wikipedia.org/wiki/HTML#Attributes.
The class attribute provides a way of classifying similar elements. This can be used for semantic or presentation purposes. For example, an HTML document might semantically use the designation <class="notation"> to indicate that all elements with this class value are subordinate to the main text of the document. In presentation, such elements might be gathered together and presented as footnotes on a page instead of appearing in the place where they occur in the HTML source. Class attributes are used semantically in microformats. Multiple class values may be specified; for example <class="notation important"> puts the element into both the notation and the important classes.
An author may use the style attribute to assign presentational properties to a particular element. It is considered better practice to use an element's id or class attributes to select the element from within a stylesheet, though sometimes this can be too cumbersome for a simple, specific, or ad hoc styling.
The title attribute is used to attach subtextual explanation to an element. In most browsers this attribute is displayed as a tooltip.
The lang attribute identifies the natural language of the element's contents, which may be different from that of the rest of the document. For example, in an English-language document:
<p>Oh well, <span lang="fr">c'est la vie</span>, as they say in France.</p>
The abbreviation element, abbr, can be used to demonstrate some of these attributes:

<abbr id="anId" class="jargon" style="color:purple;" title="Hypertext Markup Language">HTML</abbr>
This example displays as HTML; in most browsers, pointing the cursor at the abbreviation should display the title text "Hypertext Markup Language."

Most elements take the language-related attribute dir to specify text direction, such as with "rtl" for right-to-left text in, for example, Arabic, Persian or Hebrew.[77]

Character and entity references
See also: List of XML and HTML character entity references and Unicode and HTML
As of version 4.0, HTML defines a set of 252 character entity references and a set of 1,114,050 numeric character references, both of which allow individual characters to be written via simple markup, rather than literally. A literal character and its markup counterpart are considered equivalent and are rendered identically.

The ability to "escape" characters in this way allows for the characters < and & (when written as &lt; and &amp;, respectively) to be interpreted as character data, rather than markup. For example, a literal < normally indicates the start of a tag, and & normally indicates the start of a character entity reference or numeric character reference; writing it as &amp; or &#x26; or &#38; allows & to be included in the content of an element or in the value of an attribute. The double-quote character ("), when not used to quote an attribute value, must also be escaped as &quot; or &#x22; or &#34; when it appears within the attribute value itself. Equivalently, the single-quote character ('), when not used to quote an attribute value, must also be escaped as &#x27; or &#39; (or as &apos; in HTML5 or XHTML documents[78][79]) when it appears within the attribute value itself. If document authors overlook the need to escape such characters, some browsers can be very forgiving and try to use context to guess their intent. The result is still invalid markup, which makes the document less accessible to other browsers and to other user agents that may try to parse the document for search and indexing purposes for example.

Escaping also allows for characters that are not easily typed, or that are not available in the document's character encoding, to be represented within element and attribute content. For example, the acute-accented e (é), a character typically found only on Western European and South American keyboards, can be written in any HTML document as the entity reference &eacute; or as the numeric references &#xE9; or &#233;, using characters that are available on all keyboards and are supported in all character encodings. Unicode character encodings such as UTF-8 are compatible with all modern browsers and allow direct access to almost all the characters of the world's writing systems.[80]

Example HTML Escape Sequences[clarification needed]
Named	Decimal	Hexadecimal	Result	Description	Notes
&amp;	&#38;	&#x26;	&	Ampersand	
&lt;	&#60;	&#x3C;	<	Less Than	
&gt;	&#62;	&#x3e;	>	Greater Than	
&quot;	&#34;	&#x22;	"	Double Quote	
&apos;	&#39;	&#x27;	'	Single Quote	
&nbsp;	&#160;	&#xA0;		Non-Breaking Space	
&copy;	&#169;	&#xA9;	©	Copyright	
&reg;	&#174;	&#xAE;	®	Registered Trademark	
&dagger;	&#8224;	&#x2020;	†	Dagger	
&Dagger;	&#8225;	&#x2021;	‡	Double dagger	Names are case sensitive
&ddagger;	&#8225;	&#x2021;	‡	Double dagger	Names may have synonyms
&trade;	&#8482;	&#x2122;	™	Trademark	
Data types
HTML defines several data types for element content, such as script data and stylesheet data, and a plethora of types for attribute values, including IDs, names, URIs, numbers, units of length, languages, media descriptors, colors, character encodings, dates and times, and so on. All of these data types are specializations of character data.

Document type declaration
HTML documents are required to start with a Document Type Declaration (informally, a "doctype"). In browsers, the doctype helps to define the rendering mode—particularly whether to use quirks mode.

The original purpose of the doctype was to enable parsing and validation of HTML documents by SGML tools based on the Document Type Definition (DTD). The DTD to which the DOCTYPE refers contains a machine-readable grammar specifying the permitted and prohibited content for a document conforming to such a DTD. Browsers, on the other hand, do not implement HTML as an application of SGML and by consequence do not read the DTD.

HTML5 does not define a DTD; therefore, in HTML5 the doctype declaration is simpler and shorter:[81]

<!DOCTYPE html>
An example of an HTML 4 doctype

<!DOCTYPE HTML PUBLIC "-//W3C//DTD HTML 4.01//EN" "https://www.w3.org/TR/html4/strict.dtd">
This declaration references the DTD for the "strict" version of HTML 4.01. SGML-based validators read the DTD in order to properly parse the document and to perform validation. In modern browsers, a valid doctype activates standards mode as opposed to quirks mode.

In addition, HTML 4.01 provides Transitional and Frameset DTDs, as explained below. Transitional type is the most inclusive, incorporating current tags as well as older or "deprecated" tags, with the Strict DTD excluding deprecated tags. Frameset has all tags necessary to make frames on a page along with the tags included in transitional type.[citation needed]

Semantic HTML
Main article: Semantic HTML
Semantic HTML is a way of writing HTML that emphasizes the meaning of the encoded information over its presentation (look). HTML has included semantic markup from its inception,[82] but has also included presentational markup, such as <font>, <i> and <center> tags. There are also the semantically neutral span and div tags. Since the late 1990s, when Cascading Style Sheets were beginning to work in most browsers, web authors have been encouraged to avoid the use of presentational HTML markup with a view to the separation of presentation and content.[83]

In a 2001 discussion of the Semantic Web, Tim Berners-Lee and others gave examples of ways in which intelligent software "agents" may one day automatically crawl the web and find, filter and correlate previously unrelated, published facts for the benefit of human users.[84] Such agents are not commonplace even now, but some of the ideas of Web 2.0, mashups and price comparison websites may be coming close. The main difference between these web application hybrids and Berners-Lee's semantic agents lies in the fact that the current aggregation and hybridization of information is usually designed in by web developers, who already know the web locations and the API semantics of the specific data they wish to mash, compare and combine.

An important type of web agent that does crawl and read web pages automatically, without prior knowledge of what it might find, is the web crawler or search-engine spider. These software agents are dependent on the semantic clarity of web pages they find as they use various techniques and algorithms to read and index millions of web pages a day and provide web users with search facilities without which the World Wide Web's usefulness would be greatly reduced.

In order for search-engine spiders to be able to rate the significance of pieces of text they find in HTML documents, and also for those creating mashups and other hybrids as well as for more automated agents as they are developed, the semantic structures that exist in HTML need to be widely and uniformly applied to bring out the meaning of published text.[85]

Presentational markup tags are deprecated in current HTML and XHTML recommendations. The majority of presentational features from previous versions of HTML are no longer allowed as they lead to poorer accessibility, higher cost of site maintenance, and larger document sizes.[86]

Good semantic HTML also improves the accessibility of web documents (see also Web Content Accessibility Guidelines). For example, when a screen reader or audio browser can correctly ascertain the structure of a document, it will not waste the visually impaired user's time by reading out repeated or irrelevant information when it has been marked up correctly.

Delivery
HTML documents can be delivered by the same means as any other computer file. However, they are most often delivered either by HTTP from a web server or by email.

HTTP
Main article: Hypertext Transfer Protocol
The World Wide Web is composed primarily of HTML documents transmitted from web servers to web browsers using the Hypertext Transfer Protocol (HTTP). However, HTTP is used to serve images, sound, and other content, in addition to HTML. To allow the web browser to know how to handle each document it receives, other information is transmitted along with the document. This meta data usually includes the MIME type (e.g., text/html or application/xhtml+xml) and the character encoding (see Character encoding in HTML).

In modern browsers, the MIME type that is sent with the HTML document may affect how the document is initially interpreted. A document sent with the XHTML MIME type is expected to be well-formed XML; syntax errors may cause the browser to fail to render it. The same document sent with the HTML MIME type might be displayed successfully, since some browsers are more lenient with HTML.

The W3C recommendations state that XHTML 1.0 documents that follow guidelines set forth in the recommendation's Appendix C may be labeled with either MIME Type.[87] XHTML 1.1 also states that XHTML 1.1 documents should[88] be labeled with either MIME type.[89]

HTML e-mail
Main article: HTML email
Most graphical email clients allow the use of a subset of HTML (often ill-defined) to provide formatting and semantic markup not available with plain text. This may include typographic information like coloured headings, emphasized and quoted text, inline images and diagrams. Many such clients include both a GUI editor for composing HTML e-mail messages and a rendering engine for displaying them. Use of HTML in e-mail is criticized by some because of compatibility issues, because it can help disguise phishing attacks, because of accessibility issues for blind or visually impaired people, because it can confuse spam filters and because the message size is larger than plain text.

Naming conventions
The most common filename extension for files containing HTML is .html. A common abbreviation of this is .htm, which originated because some early operating systems and file systems, such as DOS and the limitations imposed by FAT data structure, limited file extensions to three letters.[90]

HTML Application
Main article: HTML Application
An HTML Application (HTA; file extension ".hta") is a Microsoft Windows application that uses HTML and Dynamic HTML in a browser to provide the application's graphical interface. A regular HTML file is confined to the security model of the web browser's security, communicating only to web servers and manipulating only web page objects and site cookies. An HTA runs as a fully trusted application and therefore has more privileges, like creation/editing/removal of files and Windows Registry entries. Because they operate outside the browser's security model, HTAs cannot be executed via HTTP, but must be downloaded (just like an EXE file) and executed from local file system.

HTML4 variations
Since its inception, HTML and its associated protocols gained acceptance relatively quickly.[by whom?] However, no clear standards existed in the early years of the language. Though its creators originally conceived of HTML as a semantic language devoid of presentation details,[91] practical uses pushed many presentational elements and attributes into the language, driven largely by the various browser vendors. The latest standards surrounding HTML reflect efforts to overcome the sometimes chaotic development of the language[92] and to create a rational foundation for building both meaningful and well-presented documents. To return HTML to its role as a semantic language, the W3C has developed style languages such as CSS and XSL to shoulder the burden of presentation. In conjunction, the HTML specification has slowly reined in the presentational elements.

There are two axes differentiating various variations of HTML as currently specified: SGML-based HTML versus XML-based HTML (referred to as XHTML) on one axis, and strict versus transitional (loose) versus frameset on the other axis.

SGML-based versus XML-based HTML
One difference in the latest HTML specifications lies in the distinction between the SGML-based specification and the XML-based specification. The XML-based specification is usually called XHTML to distinguish it clearly from the more traditional definition. However, the root element name continues to be "html" even in the XHTML-specified HTML. The W3C intended XHTML 1.0 to be identical to HTML 4.01 except where limitations of XML over the more complex SGML require workarounds. Because XHTML and HTML are closely related, they are sometimes documented in parallel. In such circumstances, some authors conflate the two names as (X)HTML or X(HTML).

Like HTML 4.01, XHTML 1.0 has three sub-specifications: strict, transitional and frameset.

Aside from the different opening declarations for a document, the differences between an HTML 4.01 and XHTML 1.0 document—in each of the corresponding DTDs—are largely syntactic. The underlying syntax of HTML allows many shortcuts that XHTML does not, such as elements with optional opening or closing tags, and even empty elements which must not have an end tag. By contrast, XHTML requires all elements to have an opening tag and a closing tag. XHTML, however, also introduces a new shortcut: an XHTML tag may be opened and closed within the same tag, by including a slash before the end of the tag like this: <br/>. The introduction of this shorthand, which is not used in the SGML declaration for HTML 4.01, may confuse earlier software unfamiliar with this new convention. A fix for this is to include a space before closing the tag, as such: <br />.[93]

To understand the subtle differences between HTML and XHTML, consider the transformation of a valid and well-formed XHTML 1.0 document that adheres to Appendix C (see below) into a valid HTML 4.01 document. To make this translation requires the following steps:

The language for an element should be specified with a lang attribute rather than the XHTML xml:lang attribute. XHTML uses XML's built in language-defining functionality attribute.
Remove the XML namespace (xmlns=URI). HTML has no facilities for namespaces.
Change the document type declaration from XHTML 1.0 to HTML 4.01. (see DTD section for further explanation).
If present, remove the XML declaration. (Typically this is: <?xml version="1.0" encoding="utf-8"?>).
Ensure that the document's MIME type is set to text/html. For both HTML and XHTML, this comes from the HTTP Content-Type header sent by the server.
Change the XML empty-element syntax to an HTML style empty element (<br /> to <br>).
Those are the main changes necessary to translate a document from XHTML 1.0 to HTML 4.01. To translate from HTML to XHTML would also require the addition of any omitted opening or closing tags. Whether coding in HTML or XHTML it may just be best to always include the optional tags within an HTML document rather than remembering which tags can be omitted.

A well-formed XHTML document adheres to all the syntax requirements of XML. A valid document adheres to the content specification for XHTML, which describes the document structure.

The W3C recommends several conventions to ensure an easy migration between HTML and XHTML (see HTML Compatibility Guidelines). The following steps can be applied to XHTML 1.0 documents only:

Include both xml:lang and lang attributes on any elements assigning language.
Use the empty-element syntax only for elements specified as empty in HTML.
Include an extra space in empty-element tags: for example <br /> instead of <br>.
Include explicit close tags for elements that permit content but are left empty (for example, <div></div>, not <div />).
Omit the XML declaration.
By carefully following the W3C's compatibility guidelines, a user agent should be able to interpret the document equally as HTML or XHTML. For documents that are XHTML 1.0 and have been made compatible in this way, the W3C permits them to be served either as HTML (with a text/html MIME type), or as XHTML (with an application/xhtml+xml or application/xml MIME type). When delivered as XHTML, browsers should use an XML parser, which adheres strictly to the XML specifications for parsing the document's contents.

Transitional versus strict
HTML 4 defined three different versions of the language: Strict, Transitional (once called Loose) and Frameset. The Strict version is intended for new documents and is considered best practice, while the Transitional and Frameset versions were developed to make it easier to transition documents that conformed to older HTML specification or didn't conform to any specification to a version of HTML 4. The Transitional and Frameset versions allow for presentational markup, which is omitted in the Strict version. Instead, cascading style sheets are encouraged to improve the presentation of HTML documents. Because XHTML 1 only defines an XML syntax for the language defined by HTML 4, the same differences apply to XHTML 1 as well.

The Transitional version allows the following parts of the vocabulary, which are not included in the Strict version:

A looser content model
Inline elements and plain text are allowed directly in: body, blockquote, form, noscript and noframes
Presentation related elements
underline (u)(Deprecated. can confuse a visitor with a hyperlink.)
strike-through (s)
center (Deprecated. use CSS instead.)
font (Deprecated. use CSS instead.)
basefont (Deprecated. use CSS instead.)
Presentation related attributes
background (Deprecated. use CSS instead.) and bgcolor (Deprecated. use CSS instead.) attributes for body (required element according to the W3C.) element.
align (Deprecated. use CSS instead.) attribute on div, form, paragraph (p) and heading (h1...h6) elements
align (Deprecated. use CSS instead.), noshade (Deprecated. use CSS instead.), size (Deprecated. use CSS instead.) and width (Deprecated. use CSS instead.) attributes on hr element
align (Deprecated. use CSS instead.), border, vspace and hspace attributes on img and object (caution: the object element is only supported in Internet Explorer (from the major browsers)) elements
align (Deprecated. use CSS instead.) attribute on legend and caption elements
align (Deprecated. use CSS instead.) and bgcolor (Deprecated. use CSS instead.) on table element
nowrap (Obsolete), bgcolor (Deprecated. use CSS instead.), width, height on td and th elements
bgcolor (Deprecated. use CSS instead.) attribute on tr element
clear (Obsolete) attribute on br element
compact attribute on dl, dir and menu elements
type (Deprecated. use CSS instead.), compact (Deprecated. use CSS instead.) and start (Deprecated. use CSS instead.) attributes on ol and ul elements
type and value attributes on li element
width attribute on pre element
Additional elements in Transitional specification
menu (Deprecated. use CSS instead.) list (no substitute, though unordered list is recommended)
dir (Deprecated. use CSS instead.) list (no substitute, though unordered list is recommended)
isindex (Deprecated.) (element requires server-side support and is typically added to documents server-side, form and input elements can be used as a substitute)
applet (Deprecated. use the object element instead.)
The language (Obsolete) attribute on script element (redundant with the type attribute).
Frame related entities
iframe
noframes
target (Deprecated in the map, link and form elements.) attribute on a, client-side image-map (map), link, form and base elements
The Frameset version includes everything in the Transitional version, as well as the frameset element (used instead of body) and the frame element.

Frameset versus transitional
In addition to the above transitional differences, the frameset specifications (whether XHTML 1.0 or HTML 4.01) specify a different content model, with frameset replacing body, that contains either frame elements, or optionally noframes with a body.

Summary of specification versions
As this list demonstrates, the loose versions of the specification are maintained for legacy support. However, contrary to popular misconceptions, the move to XHTML does not imply a removal of this legacy support. Rather the X in XML stands for extensible and the W3C is modularizing the entire specification and opening it up to independent extensions. The primary achievement in the move from XHTML 1.0 to XHTML 1.1 is the modularization of the entire specification. The strict version of HTML is deployed in XHTML 1.1 through a set of modular extensions to the base XHTML 1.1 specification. Likewise, someone looking for the loose (transitional) or frameset specifications will find similar extended XHTML 1.1 support (much of it is contained in the legacy or frame modules). The modularization also allows for separate features to develop on their own timetable. So for example, XHTML 1.1 will allow quicker migration to emerging XML standards such as MathML (a presentational and semantic math language based on XML) and XForms—a new highly advanced web-form technology to replace the existing HTML forms.

In summary, the HTML 4 specification primarily reined in all the various HTML implementations into a single clearly written specification based on SGML. XHTML 1.0, ported this specification, as is, to the new XML defined specification. Next, XHTML 1.1 takes advantage of the extensible nature of XML and modularizes the whole specification. XHTML 2.0 was intended to be the first step in adding new features to the specification in a standards-body-based approach.
