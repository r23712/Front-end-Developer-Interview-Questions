#JOB INTERVIEW QUESTIONNAIRE

@version 1.0
 
##Contributors

@bentruyman (http://bentruyman.com/), @roger_raymond (http://twitter.com/iansym), @ajpiano (http://ajpiano.com/), @paul_irish (http://paulirish.com/), @SlexAxton (http://alexsexton.com/), @boazsender (http://boazsender.com/), @miketaylr (http://miketaylr.com/), @vladikoff (http://vladfilippov.com/), @gf3 (http://gf3.ca/), @jon_neal (http://twitter.com/jon_neal), @wookiehangover (http://wookiehangover.com/) and @darcy_clarke (http://darcyclarke.me)

## General Questions:

* Are you on Twitter? 
	* Yes
	* If so, who do you follow on Twitter?
		* *Mostly web developers and designers.*

* Are you on GitHub? 
	* If so, what are some examples of repos you follow 
 		* *HTML5 Boilerplate*

* What blogs do you follow? 
	* *Lots. HTML5Weekly, JavaScript Weekly, CSS Tricks/Shoptalk, Javascript Jabber, The Web Ahead*

* What version control systems have you used (Git, SVN etc.)? 
	* *Git and SVN*

* What is your preferred development environment? (OS, Editor, Browsers, Tools etc.) 
	* *Mac, Sublime 2, Chrome Dev Tools, Firebug, Photoshop, Lots of online resources*

* Can you describe your workflow when you create a web page? 
	* *Usually start with my HTML5 Boilerplate fork, then markup, then styling, then JavaScript. I try to tackle the most challenging stuff first.*

* Can you describe the difference between progressive enhancement and graceful degradation?
	* *Progressive enhancement is starting from a baseline and then building enhancements for new browser tech on top.*
	* *Graceful degradation is starting with designing the most optimal browser experience, then designing fallbacks for older browsers.*
	* *Some methods for doing this are media queries, javascript polyfills and javascript detection libraries such as Modernizr*

* Explain what "Semantic HTML" means. 
	* *It means the opposite of using divs for everything. Taking advantage of new HTML5 elements like nav, article, header, footer, etc.*

* What browser do you primary develop in and what developer tools do you use?
	* *Chrome*

* How would you optimize a websites assets/resources?
	* *Use photoshop to compress image files, choosing the best format for the best compression, then use ysmush.it to get even more lossless compression.*
	* *Concatenate and minify JavaScript and CSS Files*
	* *Use sprite sheets and icon fonts*
	* *Use cdn for jquery and hosting video*		
	* *Cache static files (in the past this would be typically done with a php header, but now you could use a HTML5 Cache Manifest)*

* Why is it better to serve site assets from multiple domains? 
	* *Parallel downloads speed up the page load. Also, serving static files from a CDN (S3 for example) takes some load off your server.*

* How many resources will a browser download from a given domain at a time?  
	* *Depends on the browser. The recommendation is to stick to 2-4 hostnames (http://www.yuiblog.com/blog/2007/04/11/performance-research-part-4/)*

* Name 3 ways to decrease page load. (perceived or actual load time) 
	* *The best way is usually to reduce your image sizes. Minify and concatenate JS/CSS. Have JS at the bottom of the page. Use a CDN.*

* If you jumped on a project and they used tabs and you used spaces, what would you do? 
	* *Conform to the conventions (stay consistant)*

* Write a simple slideshow page 
	* Already did. (http://johnpolacek.github.com/scrolldeck.js/)

* What tools do you use to test your code's performance?
	* *Yahoo! YSlow (http://developer.yahoo.com/yslow/)*
 	* *Google PageSpeed (https://developers.google.com/speed/pagespeed/)*
  	* *Pingdom Tools (http://tools.pingdom.com/fpt/)*
   	* JSPerf (http://jsperf.com/)
	* Dromaeo (http://dromaeo.com/) 

* If you could master one technology this year, what would it be? 
	* *I put more importance on building cool things over any specific type of tech. People seem to be doing great stuff with Node.js + Arduino lately*

* Explain the importance of standards and standards bodies.  
	* *Standards are the only thing holding this crazy chaotic thing we call the web together. They make it possible for us to code up web stuff that works cross-browser/platform/device/screen*

## HTML-Specific Questions:

* What's a `doctype` do, and how many can you name? 
	* *Let's just do html and call it a day. This ain't 2007.*

* What's the difference between standards mode and quirks mode? 
	* *Quirks mode is for old (really old!) browsers. It essentially gives them permission to continue to follow their own busted way of rendering a web page as opposed to standards mode where all the browsers have come to an agreement about how to handle styling and markup. This question feels dated.*

* What are the limitations when serving XHTML pages? 
	* Are there any problems with serving pages as `application/xhtml+xml`?  
	* *Yes. Here's a nice article on this stuff (http://www.webdevout.net/articles/beware-of-xhtml/) These questions are giving me a headache. Let's just do html5.*

* How do you serve a page with content in multiple languages? 
	* *You would generally use a CMS for this, which would be wired up with different content for each language, but still output the same structure and styling.*

* What kind of things must you be wary of when design or developing for multilingual sites?
	* *Spacing is a biggie. You want to make sure you have a fluid design that can accommodate different sized type. This can be particularly noticeable in navigation buttons that might overlap content or break in the middle of a word.*

* Can you use XHTML syntax in HTML5? 
	* *Yes. (http://adactio.com/journal/1595/)*

* How do you use XML in HTML5? 
	* *I like the idea of HTML as a flavor of XML (XHTML) - i.e. quoted attr's and trailing slashes on br's, img's, etc.*

* What are `data-` attributes good for? 
	* *Storing data in the DOM. I love it.*

* What are the content models in HTML4 and are they different in HTML5? 
	* *In HTML4, there are 2 types of elements: Block and Inline. HTML5 emphasizes semantics and structure, so it has organized its elements into the categories of metadata, flow, sectioning, heading, phrasing, interactive & embedded*

* Consider HTML5 as an open web platform. What are the building blocks of HTML5? 
	* *HTML, CSS and JavaScript*

* Describe the difference between cookies, sessionStorage and localStorage. 
	* *Cookies are for storing small amounts of website data, such as a user name. HTML5 Web Storage is a faster, improved means of storing website data. sessionsStorage is for temporary data, and localStorage is for persistant data.*

## JS-Specific Questions

* Which JavaScript libraries have you used? 
	* *jQuery of course. Other ones I've used are jQuery UI, jQuery Mobile, Modernizr, Greensock and then lots of little utility ones*

* Have you ever looked at the source code of the libraries/frameworks you use?
	* *Yeah. Plenty of good stuff to learn in there. Such as https://vimeo.com/12529436 and https://vimeo.com/18901514*

* How is JavaScript different from Java? 
	* *They are very different. From what I've heard, the only reason they share the name is for marketing purposes. Java is a programming language that gets compiled then run as a standalone 'applet' in a VM or browser. Whereas JavaScript is a scripting language designed to be run only through a browser. They are both OOP, but Java is strictly typed while JS is loose.*

* What's a hashtable?
	* *A hashtable is an associative array of key/value pairs. JavaScript Objects are hashtables.*

* What are `undefined` and `undeclared` variables? 
	* *undeclared vars have not been declared by a var statement (considered null). undefined vars have been declared but have no value.*

* What is a closure, and how/why would you use one? 
	* *Closures provide a means of putting function definitions and expressions inside of other functions. A common use would be binding event handler functions so that 'this' refers to the event object. The Module Pattern is the classic example.*

* What's a typical use case for anonymous functions? 
	* *For single use methods, like when you need to pass a one-liner of code to another function. Or when you want to scope vars via a closure.*

* Explain the "JavaScript module pattern" and when you'd use it. 
	* *The module pattern is a way of organizing and encapsulating code via a closure. It allows you to create public/private functions and vars inside an object (the module). It lessens the likelihood of naming conflicts and unintended interactions with other functions/vars on the page. Modules should work independently and be easily extensible. Using modules enables to write widgets and plugins that interact with each other.*

* How do you organize your code?
	* *I like using the Module Pattern quite a bit. Whenever possible, I like to widgetize/pluginize my code.*

* What's the difference between host objects and native objects? 
	* *Native Objects are objects/methods that exist in the ECMAScript spec (Date, Math, String methods, etc.) Host Objects are created by the environment (window, history, getElementByID, etc.) or ones you create yourself.*

* Difference between: 
```javascript
function Person(){} var person = Person() var person = new Person()
```
	* *The first is undefined. The second is an object.*

* What's the difference between `.call` and `.apply`? 
	* *apply and call do the same thing, but apply() uses an array containing arguments for the target method as the second parameter.*

* explain `Function.prototype.bind`? 
* When do you optimize your code? 
* Can you explain how inheritance works in JavaScript?   
* When would you use `document.write()`?
	* Most generated ads still utilize `document.write()` although its use is frowned upon
* What's the difference between feature detection, feature inference, and using the UA string 
* Explain AJAX in as much detail as possible 
* Explain how JSONP works (and how it's not really AJAX) 
* Have you ever used JavaScript templating?
	* If so, what libraries have you used? (Mustache.js, Handlebars etc.) 
* Explain "hoisting".
* What is FOUC? How do you avoid FOUC?
* Describe event bubbling. 
* What's the difference between an "attribute" and a "property"? 
* Why is extending built in JavaScript objects not a good idea? 
* Why is extending built ins a good idea? 
* Difference between document load event and document ready event? 
* What is the difference between `==` and `===`? 
* Explain how you would get a query string parameter from the browser window's URL. 
* Explain the same-origin policy with regards to JavaScript. 
* Explain event delegation. 
* Describe inheritance patterns in JavaScript. 
* Make this work: 
```javascript
[1,2,3,4,5].duplicator(); // [1,2,3,4,5,1,2,3,4,5]
```
* Describe a strategy for memoization (avoiding calculation repetition) in JavaScript. 
* Why is it called a Ternary statement, what does the word "Ternary" indicate? 
* What is the arity of a function?  

## JS-Code Examples:

```javascript
~~3.14
```
Question: What value is returned from the above statement? 
**Answer: 3** 

```javascript
"i'm a lasagna hog".split("").reverse().join("");
```
Question: What value is returned from the above statement? 
**Answer: "goh angasal a m'i"** 

```javascript
( window.foo || ( window.foo = "bar" ) );
```
Question: What is the value of window.foo? 
**Answer: "bar"** 
only if window.foo was falsey otherwise it will retain its value.

```javascript
var foo = "Hello"; (function() { var bar = " World"; alert(foo + bar); })(); alert(foo + bar);
```
Question: What is the outcome of the two alerts above? 
**Answer: "Hello World" & ReferenceError: bar is not defined** 

```javascript
var foo = [];
foo.push(1);
foo.push(2);
```
Question: What is the value of foo.length? 
**Answer: `2`

```javascript
var foo = {};
foo.bar = 'hello';
```
Question: What is the value of foo.length? 
**Answer: `undefined`


## jQuery-Specific Questions:

* Explain "chaining". 
* Explain "deferreds".
* What are some jQuery specific optimizations you can implement?
* What does `.end()` do? 
* How, and why, would you namespace a bound event handler? 
* Name 4 different values you can pass to the jQuery method.
	* Selector (string), HTML (string), Callback (function), HTMLElement, object, array, element array, jQuery Object etc.
* What is the effects (or fx) queue? 
* What is the difference between `.get()`, `[]`, and `.eq()`? 
* What is the difference between `.bind()`, `.live()`, and `.delegate()`? 
* What is the difference between `$` and `$.fn`? Or just what is `$.fn`.
* Optimize this selector: 
```javascript
$(".foo div#bar:eq(0)")
```

## CSS-Specific Questions:

* Describe what a "reset" CSS file does and how it's useful. 
* Describe Floats and how they work. 
* What are the various clearing techniques and which is appropriate for what context? 
* Explain CSS sprites, and how you would implement them on a page or site. 
* What are your favourite image replacement techniques and which do you use when? 
* CSS property hacks, conditionally included .css files, or... something else? 
* How do you serve your pages for feature-constrained browsers? 
	* What techniques/processes do you use?  
* What are the different ways to visually hide content (and make it available only for screen readers)? 
* Have you ever used a grid system, and if so, what do you prefer? 
* Have you used or implemented media queries or mobile specific layouts/CSS? 
* Any familiarity with styling SVG? 
* How do you optimize your webpages for print? 
* What are some of the "gotchas" for writing efficient CSS? 
* Do you use CSS preprocessors? (SASS, Compass, Stylus, LESS) 
	* If so, describe what you like and dislike about the CSS preprocessors you have used. 
* How would you implement a web design comp that uses non-standard fonts? 
	* Webfonts (font services like: Google Webfonts, Typekit etc.)
* Explain how a browser determines what elements match a CSS selector?  

## Optional fun Questions:

* What's the coolest thing you've ever coded, what are you most proud of?
* Do you know the HTML5 gang sign? 
* Are you now, or have you ever been, on a boat. 
* What are your favorite parts about the developer tools you use?
* Do you have any pet projects? What kind? 
* Explain the significance of "cornify". 
* On a piece of paper, write down the letters A B C D E vertically. Now put these in descending order without writing one line of code. 
	* Wait and see if they turn the paper upside down
* Pirate or Ninja? 
	* Bonus if it's a combo and a good reason was given (+2 for zombie monkey pirate ninjas) 
* If not Web Development, what would you be doing? 
* Where in the world is Carmen Sandiego?
	* Hint: their answer is always wrong 
* What's your favorite feature of Internet Explorer?
* Complete this sentence: Brendan Eich and Doug Crockford are the __________ of javascript.
* jQuery: a great library or the greatest library? Discuss.
