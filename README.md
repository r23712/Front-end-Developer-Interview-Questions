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
 		* *[HTML5 Boilerplate](https://github.com/h5bp/html5-boilerplate/), [Modernizr](https://github.com/Modernizr/Modernizr/), [Video.js](https://github.com/zencoder/video-js) and lots more.*

* What blogs do you follow? 
	* *Lots (and also podcasts) including [HTML5Weekly](http://html5weekly.com), [JavaScript Weekly](http://javascriptweekly.com) / [JavaScript Show](http://javascriptshow.com/), [CSS Tricks](http://css-tricks.com/) / [Shoptalk](http://shoptalkshow.com/), [JavaScript Jabber](http://javascriptjabber.com/), [The Web Ahead](http://5by5.tv/webahead/) And I try to devour as much of what is on [Hacker News](http://news.ycombinator.com/) as possible.*

* What version control systems have you used (Git, SVN etc.)? 
	* *Git and SVN*

* What is your preferred development environment? (OS, Editor, Browsers, Tools etc.) 
	* *Mac, Sublime 2, Chrome Dev Tools, Firebug, Photoshop, lots of online resources*

* Can you describe your workflow when you create a web page? 
	* *Usually start with my [HTML5 Boilerplate fork](https://github.com/johnpolacek/html5project), then markup, then styling, then JavaScript. I try to tackle the most challenging stuff first.*

* Can you describe the difference between progressive enhancement and graceful degradation?
	* *Progressive enhancement is starting from a baseline and then building enhancements for new browser tech on top.*
	* *Graceful degradation is starting with designing the most optimal browser experience, then designing fallbacks for older browsers.*
	* *Some methods for doing this are media queries, javascript polyfills and javascript detection libraries like Modernizr*

* Explain what "Semantic HTML" means. 
	* *It means the opposite of using divs for everything. Taking advantage of new HTML5 elements like nav, article, header, footer, etc.*

* What browser do you primary develop in and what developer tools do you use?
	* *Chrome*

* How would you optimize a websites assets/resources?
	* *Use photoshop to compress image files, choosing the best format for the best compression, then use ysmush.it to get even more lossless compression.*
	* *Concatenate and minify JavaScript and CSS Files*
	* *Use sprite sheets and icon fonts*
	* *Use a cdn for jquery and hosting video*		
	* *Cache static files (in the past this would be typically done with a php header, but now you could use a HTML5 Cache Manifest)*

* Why is it better to serve site assets from multiple domains? 
	* *Parallel downloads speed up the page load. Also, serving static files from a CDN ([S3](http://aws.amazon.com/s3/) for example) takes some load off your server.*

* How many resources will a browser download from a given domain at a time?  
	* *Depends on the browser. The recommendation is to stick to 2-4 hostnames <small>[(source)](http://www.yuiblog.com/blog/2007/04/11/performance-research-part-4/)</small>*

* Name 3 ways to decrease page load. (perceived or actual load time) 
	* *The best way is usually to reduce your image sizes. Minify and concatenate JS/CSS. Have JS at the bottom of the page. Use a CDN.*

* If you jumped on a project and they used tabs and you used spaces, what would you do? 
	* *Conform to the conventions (stay consistant)*

* Write a simple slideshow page 
	* [Already did](http://johnpolacek.github.com/scrolldeck.js/)

* What tools do you use to test your code's performance?
	* *[Yahoo! YSlow](http://developer.yahoo.com/yslow/)*
 	* *[Google PageSpeed](https://developers.google.com/speed/pagespeed/)*
  	* *[Pingdom Tools](http://tools.pingdom.com/fpt/)*
   	* [JSPerf](http://jsperf.com/)
	* [Dromaeo](http://dromaeo.com/) 

* If you could master one technology this year, what would it be? 
	* *I put more importance on building cool things over any specific type of tech. People seem to be doing [neat stuff](http://www.instructables.com/id/Arduino-LCD-Twitter-display/) with [Node.js](http://nodejs.org/) + [Arduino](http://www.arduino.cc) lately*

* Explain the importance of standards and standards bodies.  
	* *Standards are the only thing holding this crazy chaotic thing we call the web together. They make it possible for us to code up web stuff that works cross-browser/platform/device/screen*

* What is FOUC? How do you avoid FOUC?
	* Some pages that uses CSS @import rule experience a curious display quirk in the Windows version of MS Internet Explorer: a momentary flash of unstyled page content.  We could avoid it by establishing the Link element to the basic HEAD element is probrably the most natural solution, why, because first of all every page can benefit from the addition of either an alternate stylesheet or a media-dependent stylesheet.

## HTML-Specific Questions:

* What's a `doctype` do, and how many can you name? 
	* *Defines the version of html the document is using. Let's just do html and call it a day. This ain't 2007.*

* What's the difference between standards mode and quirks mode? 
	* *Quirks mode is for old (really old!) browsers. It essentially gives them permission to continue to follow their own busted way of rendering a web page as opposed to standards mode where all the browsers have come to an agreement about how to handle styling and markup. This question feels dated.*

* What are the limitations when serving XHTML pages? 
	* Are there any problems with serving pages as `application/xhtml+xml`?  
	* *Yes. [Here's a nice article](http://www.webdevout.net/articles/beware-of-xhtml/) on this stuff. These questions are giving me a headache. Let's just do html5.*

* How do you serve a page with content in multiple languages? 
	* *You would generally use a CMS for this, which would be wired up with different content for each language, but still output the same structure and styling.*

* What kind of things must you be wary of when design or developing for multilingual sites?
	* *Spacing is a biggie. You want to make sure you have a fluid design that can accommodate different sized type. This can be particularly noticeable in navigation buttons that might overlap content or break in the middle of a word.*

* Can you use XHTML syntax in HTML5? 
	* *[Yes](http://adactio.com/journal/1595/)*

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

* Explain how 'this' works in JavaScript
	* 'this' in javascript is the current object, for example this is how you access your object in Javascript. For example:
	
	  ```
	  function HotDog() {
	    this.condiments = 'mustard, ketchup';
	    this.getCondiments = function() {
	      return this.condiments;
	    }
	  }
	  ```

* Explain how prototypal inheritance works
	* Every object in JavaScript has a prototype that is shared between all objects of the same type. Properties can be added to the prototype or an individual object.  Although not a great comparison you could say in this respect the prototype acts like a class in more "classical" object oriented programming.

* How do you go about testing your JavaScript?
	* 

* AMD vs. CommonJS?
	* CommonJS
	    * Is a server first approach
	    * Assumes Sync
	    * Clean slate, no global baggage
	    * forward looking
	* AMD
	    * Is a browser first approach
	    * prefers async
	    * non module resources (no File I/O)
	    * simplifies backward-compatibility 


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
	* *`.apply` and `.call` do the same thing, but `.apply` uses an array containing arguments for the target method as the second parameter.*

* explain `Function.prototype.bind`? 
	* *Use this to create functions that when called have a particular value for `this` and therefore binding it to the original value of the target object*

* When do you optimize your code? 
	* *All the time, from the beginning structure, to refactoring along the way, to re-evaluating at the end.*

* Can you explain how inheritance works in JavaScript?   
	* *JavaScript does not have classes - it uses prototypal inheritance. There continues to be [debate](http://stackoverflow.com/questions/6418674/improvement-over-john-resigs-javascript-class-framework) over what specific inheritance pattern works best. I like [John Resig’s approach](http://ejohn.org/blog/simple-javascript-inheritance/) as implemented in [$.Class by JavaScriptMVC](http://javascriptmvc.com/docs.html#!jQuery.Class) simply because it just makes the most sense to me.*

* When would you use `document.write()`?
	* *It is bad practice to use `document.write()`. Instead, use DOM manipulation methods like `innerHTML`. The one case where it is acceptable from what I understand is where you would want to add link to a stylesheet if JavaScript is enabled.*

* What's the difference between feature detection, feature inference, and using the UA string 
	* *Using feature detection over user agent detection is favored because devices and device features are constantly changing and therefore it is better to design behavior based on whether particular features are present or not. For example, by using [Modernizr](http://modernizr.com/) or [yepnope](http://yepnopejs.com).*

* Explain AJAX
	* *AJAX is used for asynchonously sending and receiving data without interfering with any processes occuring on the page. It is used for things like form submission, loading dynamic content assets and user interaction like chat rooms and multiplayer games. When data is returned from a server, a callback function is then executed that handles the data. AJAX stands for Asynchronous JavaScript and XML, which has become a bit outdated as most are using JSON these days. But, AJAJ just doesn’t have as nice a ring to it though.*

* Explain how JSONP works (and how it's not really AJAX) 
	* *JSONP stands for JSON with padding. The padding is a callback function that is used to wrap the data returned from the server. The reason for its existence is to get around browser's same-origin restriction against cross domain requests.*

* Have you ever used JavaScript templating? If so, what libraries have you used? (Mustache.js, Handlebars etc.)
	* *I've used jQuery Templates and more recently Mustache. Recently though, my favorite has been to use [ICanHaz.js](http://icanhazjs.com) with Mustache. *

* Explain "hoisting".
	* *Hoisting is a feature in JavaScript where var declarations are moved to the top of the function body. However, the initialization/assignment of the var is not. Therefore it is considered best practice to define and assign all var declarations at the top of a function.*

* What is FOUC? How do you avoid FOUC?
	* *FOUC = Flash Of Unstyled Content. The standard way is to do a .no-js hook on the document body that gets changed to .js by some script in the document head.*

* Describe event bubbling. 
	* *Events are dispatched first at the event target, then propagate up through the target element's parent and ancestors, 'bubbling' all the way up to the document root.*

* What's the difference between an "attribute" and a "property"? 
	* *An attribute carries information about an element in the form of a key value pair. A property is the key portion of that attribute.*

* Why is extending built in JavaScript objects not a good idea? 
	* *The main reason not to do it is to avoid conflicts - for example, if two different scripts are extending an object in an incompatible way. If every JS library out there started extending object prototypes, it would create a huge mess. It is best to leave the built-ins alone, as that way everyone knows their expected behavior and there are no surprises down the road.*

* Why is extending built ins a good idea? 
	* *The temptation is that by extending a native object, you can quickly bring useful functionality to JS prototypes, like Array or String. But that quick solution can lead to big headaches later on. Are there any good use cases? Some say a worthy use would be making polyfills for older browsers to bring them up to the latest EcmaScript standards, yet even that seems open to causing trouble. Best steer clear. There be dragons.*

* Difference between document load event and document ready event? 
	* *Document ready fires when the html load has completed and the DOM is 'ready'. The window load fires when images and other page content have all finished loading.*

* What is the difference between `==` and `===`? 
	* *`===` is strictly equal, while `==` allows for truthiness, where the objects being compared are equal after type coercion. For example, `1=="1"` is true, but `1==="1"` is false.*

* Explain how you would get a query string parameter from the browser window's URL. 
	* *I would look up how to do it on [stackoverflow](http://stackoverflow.com/questions/901115/get-query-string-values-in-javascript).*

* Explain the same-origin policy with regards to JavaScript. 
	* *A script can read only the properties of windows and documents that are loaded from the same host, through the same port, and by the same protocol as the script itself. <small>([source])(http://docstore.mik.ua/orelly/webprog/jscript/ch21_03.htm)</small>*

* Explain event delegation. 
	* *Event delegation is assigning event handlers further up the DOM tree to capture events as they bubble up from children. For example, adding a click event listener to a `<ul>` to capture any clicks upon its child `<li>` elements.*

* Describe inheritance patterns in JavaScript. 
	* *Didn't we do this one already?*

* Make this work: 
```javascript
[1,2,3,4,5].duplicator(); // [1,2,3,4,5,1,2,3,4,5]
```
	* *Ok, but this is going to extend the built in JS Array Object, which we already said was a bad idea.*

```javascript
Array.prototype.duplicator = function() {
    return this.concat(this);
}

// I'd prefer to do this:
function duplicateArray(array) {
	return array.concat(array);
}
var dup = duplicateArray([1,2,3,4,5])

// Or this:
function duplicateArray(array, numDups) {
    var dups = [];
    for (var i=0; i<numDups+1; i++) {
        dups = dups.concat(array);
    }
    return dups;
}
var dup = duplicateArray([1,2,3,4,5], 1);
```

* Describe a strategy for memoization (avoiding calculation repetition) in JavaScript. 
	* *The standard way to do it is to create a memoization function that creates a cache object for calculations. You then pass calculations into the function, which checks if it already exists in the cache. If it does, it returns the result without having to actually perform the calculation. If the calculation doesn't exist in the cache, it performs and returns the calculation, then also stores it in the cache object for next time.*

* Why is it called a Ternary statement, what does the word "Ternary" indicate? 
	* *Ternary indicates an inline if statement, comprised of 3 parts. The first is a boolean expression. The second is an expression that is returned if the boolean is true. The third is an expression returned if the boolean is false. “In computer science, a ternary operator is an operator that takes three arguments.” - http://en.wikipedia.org/wiki/Ternary_operation*

* What is the arity of a function?  
	* *The number of arguments expected by a function. <small>([source])(https://developer.mozilla.org/en-US/docs/JavaScript/Reference/Global_Objects/Function/arity)</small>*

* What is "use strict";? what are the advantages and disadvantages to using it?
	* Well strick mode improves Javascript code by enforcing better programming pratices and eliminating some of the languages insecure and ill-advised features.

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
	* *jQuery methods return an object, therefore making it possible to run sequential methods on the same jQuery object. This results in shorter, cleaner code that runs faster because it reduces interaction with the DOM.*

* Explain "deferreds".
	* *A jQuery Deferred Object is used to manage callbacks based on success and failure of other functions. It is primarily used for handling ajax requests that require flexible or complex state management. Multiple callbacks can be attached to a single deferred object in a chain, with methods like `deferred.then()` `deferred.done()` and `deferred.fail()`. Callbacks can even be bound after the event dispatch has occured.*

* What are some jQuery specific optimizations you can implement?
	* *Use chaining as much as possible. Optimize selectors (for example using `.find()` rather than context). Cache selectors that get run more than once. Use `.on()` assigned to a parent element, rather than binding lots of event listeners to child elements. Reduce the amount of DOM manipulation (for example, if you are building a list, instead of using multiple `.append()` calls to a `<ul>` element, instead build all the `<li>` elements as a string and use `.append()` just once).*

* What does `.end()` do? 
	* *You use `.end()` when chaining methods to revert back to a previous selected group of elements. For example, if you do a `.find()` and then `.end()`, it reverts the selector back to its state before the `.find()` was executed. It enables you to do less DOM lookups.*

* How, and why, would you namespace a bound event handler? 
	* *You would namespace an event handler if you want to refer to a specific event handler for triggering or removal (for example, you could have multiple click event handlers bound to an element, but only want to remove one of them).*

* Name 4 different values you can pass to the jQuery method.
	* Selector (string), HTML (string), Callback (function), HTMLElement, object, array, element array, jQuery Object etc.

* What is the effects (or fx) queue? 
	* *It is jQuery’s library for animation.*

* What is the difference between `.get()` and `.eq()`? 
	* *`eq()` returns a jQuery object and `get()` returns a DOM element.*

* What is the difference between `.bind()`, `.live()`, and `.delegate()`? 
	* *`.bind()` was the original method for attaching event listeners in jQuery, and is very straightforward way of putting an event listener onto an element. `.live()` is an improvement over `.bind()` in that it gets attached only once to a given selector, as opposed to `.bind()` which binds individual event listeners to each matched element. `.delegate()` is even better because you can attach the listener to a root element that will catch events that bubble up from the designated element delegates (resulting in better performance). It also works great for dynamic elements that get added to the page after the original event handler was attached.*

* What is the difference between `$` and `$.fn`? Or just what is `$.fn`.
* Optimize this selector: 
```javascript
$(".foo div#bar:eq(0)")
```
	* *`$('#bar')`*

## CSS-Specific Questions:

* Describe what a "reset" CSS file does and how it's useful. 
	* *A CSS reset is used to create a baseline set of styles that will display the same across browsers.*

* Describe Floats and how they work. 
	* *Elements can be floated left or right, elements after the float will then wrap around it (unless the clear property is applied to the element).*

* What are the various clearing techniques and which is appropriate for what context? 
	* *You could float a series of elements to achieve a gallery, then use clear both to force line breaks. You could make a flexible 2 or 3-column layout, then clear both on the footer. You would use clearfix technique to force a container’s height to adjust to fit floated elements.*

* Explain CSS sprites, and how you would implement them on a page or site. 
	* *First, create a spritesheet that contains all the commonly used graphic elements on your website. Then to use the sprites, use the spritesheet as a background image on a `<div>` set to the size of the sprite, then use `background-position` to display the appropriate sprite. A newer technique would be to use icon fonts, which have the added advantage of being vector-based and therefore look nicer on higher resolution (retina) screens. Some nice icon fonts are [Font Awesome](http://fortawesome.github.com/Font-Awesome/) and [Foundation Icons](http://www.zurb.com/playground/foundation-icons)*

* What are your favourite image replacement techniques and which do you use when? 
	* *Webfonts have replaced many of the use cases for image replacement. However, it still is necessary from time to time, especially for something like a company logo. I like the [HTML5 Boilerplate(H5BP)](http://html5boilerplate.com) approach of setting the font size to zero rather than use text-indent.*

* CSS property hacks, conditionally included .css files, or... something else? 
	* *Once again, I go with [H5BP](http://html5boilerplate.com) and their technique of conditional classes on `<html>`*

* How do you serve your pages for feature-constrained browsers? What techniques/processes do you use?  
	* *First, its important to take a look at any analytics you can to see what browsers and devices your users are using. Next of course, it depends on the content. I've used various approaches (graceful degradation, progressive enhancement, mobile first). I like the responsive web design approach of primarily using media queries. Also doing feature detection (usually with [Modernizr](http://modernizr.com/)) combined with polyfills.*

* What are the different ways to visually hide content (and make it available only for screen readers)? 
	* *Some people have used `text-indent` or absolute positioning to move the content off the page, but the favorable approach is to use `clip: rect(1px, 1px, 1px, 1px);` along with some other properties. Again, HTML5 Boilerplate is helpful here, as they have a nice `.visually-hidden` class for just this purpose.*

* Have you ever used a grid system, and if so, what do you prefer? 
	* *I used to use [960.gs](http://960.gs) (I think like everyone else). With fluid grids being all the rage these days (deservedly so) I've messed around with a few like [Golden Grid System](http://goldengridsystem.com) and [Skeleton](http://www.getskeleton.com) - Most of the time, I think I've been using [Twitter Bootstrap](http://twitter.github.com/bootstrap/) or rolling my own.*

* Have you used or implemented media queries or mobile specific layouts/CSS? 
	* *Only like all the time.*

* Any familiarity with styling SVG? 
	* *I have not, but I always say the key to being a good developer is to be good at [Google](http://lmgtfy.com/?q=css+svg) (and these days [StackOverflow](http://stackoverflow.com/questions/588718/jquery-svg-vs-raphael))*

* How do you optimize your webpages for print? 
	* *I would start with the H5BP print stylesheet as a base and then customize as needed.*

* What are some of the "gotchas" for writing efficient CSS? 
	* *One mistake I see commonly is using to many linked .css files. The old practice of trying to avoid 'class-itis' is outdated and no longer good practice (instead use semantic class names). The key is to not style 'pages', but rather style 'modules'. Optimize for change. Website maintainability is important.*

* Do you use CSS preprocessors? (SASS, Compass, Stylus, LESS) 
	* *I have not used them much other to try them out. If I worked with a team that used them, I would have no problem with doing so.*

* How would you implement a web design comp that uses non-standard fonts? 
	* *I would use webfonts via `@font-face`. I would be very relectant to use any other technique for any significant amount of text.*

* Explain how a browser determines what elements match a CSS selector?  
	* *Browsers read CSS from right to left. The less rules the browser has to evaluate, the faster the styling engine will perform.*

	* *To resolve conflicts between rules applying to the same element, browsers follow a set of rules to determine which selector is more specific (CSS Specificity). There is a weighted point system, where element selectors are 1 point, class selectors are 10 points and ID selectors are 100 points. In the case of 2 equally weighted selectors, the last rule is the one that gets followed.*

## Optional fun Questions:

* What's the coolest thing you've ever coded, what are you most proud of?
	* *Even though its a bit silly, my [Scrollorama](http://johnpolacek.github.com/scrollorama/) and [Superscrollorama](http://johnpolacek.github.com/superscrollorama/) plugins have gotten a lot of positive response and thats made me proud.*

* Do you know the HTML5 gang sign? 
	* *[Yes](http://html5homi.es)*

* Are you now, or have you ever been, on a boat. 
	* *I have ridden on boats of many sizes.*

* What are your favorite parts about the developer tools you use?
	* *Running JS in the console is purty dern cuhl.*

* Do you have any pet projects? What kind? 
	* *[Yes](http://areyouabrogrammer.com), [yes](http://johnpolacek.com/matchtheletter/) [yes](http://johnpolacek.github.com/scrolldeck.js/decks/responsive/).*

* Explain the significance of "cornify". 
	* *Bringing [rainbow happiness](http://www.cornify.com) to the dull corners of the web.*

* On a piece of paper, write down the letters A B C D E vertically. Now put these in descending order without writing one line of code. 
	* Wait and see if they turn the paper upside down

* Pirate or Ninja? 
	* *I think of myself more as [Winston Wolf](http://www.youtube.com/watch?v=ANPsHKpti48)*

* If not Web Development, what would you be doing? 
	* *I used to draw stuff, so maybe that.*

* Where in the world is Carmen Sandiego?
	* *Probably hanging out with Nora the Explorer*

* What's your favorite feature of Internet Explorer?
	* *The part where everybody makes funny jokes about it*

* Complete this sentence: Brendan Eich and Doug Crockford are the __________ of javascript.
	* *Eich and Crockford*

* jQuery: a great library or the greatest library? Discuss.
	* *Greatestest*
