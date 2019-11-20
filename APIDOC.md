## Functions

<dl>
<dt><a href="#parseArticle">parseArticle(options, socket)</a> ⇒ <code>Object</code></dt>
<dd><p>main article parser module export function</p>
</dd>
<dt><a href="#articleParser">articleParser(options, socket)</a> ⇒ <code>Object</code></dt>
<dd><p>article scraping function</p>
</dd>
<dt><a href="#spellCheck">spellCheck(text, options)</a> ⇒ <code>Object</code></dt>
<dd><p>checks the spelling of the article</p>
</dd>
<dt><a href="#getRawText">getRawText(html)</a> ⇒ <code>String</code></dt>
<dd><p>takes the article body and returns the raw text of the article</p>
</dd>
<dt><a href="#getFormattedText">getFormattedText(html, title, baseurl, options)</a> ⇒ <code>String</code></dt>
<dd><p>takes the article body and the derived title and returns the formatted text of the article with links made absolute.</p>
</dd>
<dt><a href="#getHtmlText">getHtmlText(text)</a> ⇒ <code>String</code></dt>
<dd><p>takes the formatted article body text and returns the &quot;clean&quot; html text of the article</p>
</dd>
</dl>

<a name="parseArticle"></a>

## parseArticle(options, socket) ⇒ <code>Object</code>
main article parser module export function

**Kind**: global function  
**Returns**: <code>Object</code> - article parser results object  

| Param | Type | Description |
| --- | --- | --- |
| options | <code>Object</code> | the options object |
| socket | <code>Object</code> | the optional socket |

<a name="articleParser"></a>

## articleParser(options, socket) ⇒ <code>Object</code>
article scraping function

**Kind**: global function  
**Returns**: <code>Object</code> - article parser results object  

| Param | Type | Description |
| --- | --- | --- |
| options | <code>Object</code> | the options object |
| socket | <code>Object</code> | the optional socket |

<a name="spellCheck"></a>

## spellCheck(text, options) ⇒ <code>Object</code>
checks the spelling of the article

**Kind**: global function  
**Returns**: <code>Object</code> - object containing potentially misspelled words  

| Param | Type | Description |
| --- | --- | --- |
| text | <code>String</code> | the string of text to run the spellcheck against |
| options | <code>Object</code> | [retext-spell options](https://github.com/retextjs/retext-spell) |
| options.dictionary | <code>Array</code> | by default is set to [en-gb](https://github.com/wooorm/dictionaries/tree/master/dictionaries/en-GB). |

<a name="getRawText"></a>

## getRawText(html) ⇒ <code>String</code>
takes the article body and returns the raw text of the article

**Kind**: global function  
**Returns**: <code>String</code> - raw text of the article in lower case  

| Param | Type | Description |
| --- | --- | --- |
| html | <code>String</code> | the html string to process |

<a name="getFormattedText"></a>

## getFormattedText(html, title, baseurl, options) ⇒ <code>String</code>
takes the article body and the derived title and returns the formatted text of the article with links made absolute.

**Kind**: global function  
**Returns**: <code>String</code> - formatted text of the article  

| Param | Type | Description |
| --- | --- | --- |
| html | <code>String</code> | the body html string to process |
| title | <code>String</code> | the title string to process |
| baseurl | <code>String</code> | the base url of the page being scraped |
| options | <code>Object</code> | the [htmltotext](https://github.com/werk85/node-html-to-text) formatting options |

<a name="getHtmlText"></a>

## getHtmlText(text) ⇒ <code>String</code>
takes the formatted article body text and returns the "clean" html text of the article

**Kind**: global function  
**Returns**: <code>String</code> - the clean html text of the article  

| Param | Type | Description |
| --- | --- | --- |
| text | <code>String</code> | the formatted text string to process |
