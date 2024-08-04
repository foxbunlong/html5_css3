# NOTES

## Groups

- `Article` is a `semantic element` (element clearly describes its meaning to both the browser and the developer) in html5. It is considered as `Flow` Content, `Sectioning` Content or `Palpable` Content.
- Comparision between `article` and `section` in [HTML Semantic Elements](https://www.w3schools.com/html/html5_semantic_elements.asp)
- `Aside` is also a `semantic element` which is tangentially related to content around it but being separated from that content.
- `Header` and `Footer` are used to contain section's heading area and footer area for nearest ancestor.
- `Address` is simple - Just contact details related to nearest ancestor.
- `Paragraph` is a block of text with one or more sentences of a particular topic.
- `Unordered Lists` is list of items without order.
- `Ordered Lists` is list of item with intential order.
- `Association Lists` have 3 elements: `dl` consists of zero or more name-value groups. `dt` represents the term or name of term-description group. `dd` represents the description, definition or value of term-description group.
- `Table` is an element to show multidimentional content - nothing changed in html5, still includes rows, columns and cells.
- `Main` elememt represents the dominant content of the document.
- `Div` element has no special meaning and only represents its children. When no other element is suitable, `div` comes last.

## Texts

- `Em` element is emphasis text in a sentense.
- `Strong` represents strong importance, seriousness or urgency for its contents.
- `Small` represents side comments (e.g. small print).
- `Br` represents a line break.
- `Self-closing tag` is a tag that is both a start and end tag at the same time.
- `Author's comments` is comments inside html code.
- `Span` has no special meaning and only represents its children. It's useful when used together with particular attributes.

## Browser and DOM

- `Links` are a conceptual construct, created by `a`, `area`, `form` and `link`. They represent a connection between 2 resources (current document and another)
- `Rendering engine` is a computer program that transform an HTML doc into a visual, interactive representation. [`Blink`](https://www.chromium.org/blink/) is rendering engine inside Google Chrome. [`Gecko`](https://firefox-source-docs.mozilla.org/overview/gecko.html) is rendering engine inside Mozilla Firefox. [`WebKit`](https://webkit.org/) is rendering engine inside Safari.
- `Parse` is analyze text, character by character.
- `Named Character References` are a [set of special character reference names](https://html.spec.whatwg.org/multipage/named-characters.html) that are supported by html.
- `Object` is a collection of data and code to represent something.
- `Model` is a representation of a thing. `Object Model` is a collection of objects that represent a thing and provide access to examine and change that thing.
- `Document Object Model` - DOM is an object model that represents and HTML document. It provides the ability to examine and change the document as presented via the user agent.
- Browser will read the document character by character and build up the DOM.
- Developer tools: `Chrome DevTools`.
- `Inspector` allows you to review and modify the DOM. It leaves html untouch.
- `Id` of element is unique identity in the DOM.

## Accessibility
- Using Semantics structure will make screen reader easier to understand your document.

## Interactivity
- `Nav` element represents a section of a page that links to other pages or to parts within the page.
- In http request, there might be query string consists of name/value pair separated by ampersand to be sent via HTTP. It's called `Forms`.
- `Form` element represents a hyperlink that can be manipulated through a collection of form-associated elements (editable and able to be submitted to a server for processing). The data is called `payload`. Method can be `post` (payload is form data) or `get` (payload is query string).
- `Field` or `Control` is an element that allows user to input information (in context of a form element). Value in field is used to generated query string.
- `Button` is used to submit the data.
- `Radio` element in `group` can only have 1 control set its checkedness to true.
- `Checkbox` element can only have 2 states: `on` or `off`.
- `Fieldset` element represents a set of form controls grouped together. The caption is given by the 1st `legend` element.

## Javascript framework
- `DOM manipulation` is changing the DOM tree after HTML document has been parsed and the DOM has been created.

## Stylesheets and Querying Trees
- `Stylesheet` is a collection of stylistic rules.
- `User agent stylesheet` is a collection of stylistic rules that the user agent follows when displaying an HTML document. Each browser has its own css.
- `Type selector` is to find and match elements in the DOM by their type.
- `Inheritance` of CSS - all children will inherit the properties of their parent.
- `Universal selector` is written as a CSS qualified name with an asterisk as local name, represents the qualified name of an element type.
- `Attribute selectors` find element based on attribute.
- `Id selectors` find element based on id, represented by `#`in css file.
- `Class selectors` find element until they equal to the notation. Thus, for HTML, div.value and div[class~=value] have the same meaning.
- We can `group selectors` by placing comma between them to share the same style.
- `Descendant combinator` - authors may want selectors to describe an element that is the descendant of another element in the document tree. Separated by whitespace.
- `Child combinator` describes a childhood relationship between 2 elements. Conducted by a greater-than sign `>` to separate 2 sequences of simple selectors. Child and descendant combinators can be used in a single selector (e.g `div ol>li p` - read from right to left).
- `Next-sibling combinator` is made of the plus sign `+` that separates 2 sequences of simple selectors to represent elements that share the same parent in document tree. Immediately precedes to 1st element.
- `Subsequent-sibling combinator` is made of the tildle `~` the separates 2 sequences of simple selectors to represent elements that share the same parent in document tree. Not necessarily immediately precedes to 1st element.
- `Child-indexed pseudo-classes` select elements which are sibling of each others. Made of `nth-child`.
- `Typed child-indexed pseudo-classes` select same as `Child-indexed pseudo-classes` but with type specific.
- `Location pseudo-classes` support to make selection based on link. In particular, state of link. Commonly `:link` and `:visited` pseudo classes.
- `User action pseudo-classes` support to make selection based on user behavior. Most commonly used are `:hover` and `:focus`.
- `Negation pseudo-classes` (matched none) find elements that is not something. Made of `:not`.
- `Pseudo-elements` represents abstract elements of the document beyond those elements explicitly created by the document language. Example: `::first-letter`.

## Order of cascade
1. Important user agent declarations
2. Import author declarations
3. Normal author declarations
4. Norma user agent declarations

- Importance in css is represented by `!important`. This should not be overly used.

## Sources
- [MDN](https://developer.mozilla.org/en-US/) and [Can I Use](https://caniuse.com/) - Trusted source for browser support