# Technical Glossary

This glossary is ever-evolving and relies on the contributions of people like
you for new word suggestions :heart:. If you've got a word you'd like a definition
please create an issue: [github.com/dwyl/technical-glossary/issues/](https://github.com/dwyl/technical-glossary/issues/new)

### Why?
Have you ever learnt something cool in coding without knowing what it's actually
called? Or have you ever been reading about a concept only to get lost in the
number of acronyms and other technical words used to describe what you're
learning about? 🤔

This resource has been created to provide quick access, simple and easy to
understand definitions to stop big words getting in the way of what could be
happy learning :blush: :muscle:

### What?

A technical glossary for key words
you will encounter in your journey through learning creative technology.
These definitions are deliberately succinct,
they aim to be easy to understand and bite-sized for quick access.

### How?

Scan down the alphabetically ordered list to learn about key words or open an
issue with more key word suggestions.

**Adaptive Web Design (AWD)** - encourages the creation of several versions of a
web page for a specified number of device dimensions. Which template to display
is determined in the HTTP GET request which recognises the screen size of the
device. Adaptive Web Design was introduced to deal with mobile browsing when
most sites were optimised for desktop only. As devices now exist in many sizes
and dimensions from different mobile brands through tablets to desktops,
**Responsive Web Design** has become a popular and more flexible alternative.

**Authentication** - the process of verifying that you are who you say you are
E.g. when you login to your email you use a password to authenticate your
identity. Other methods for authentication include using an ID card or
fingerprint/biometric method.

**Authorization** - check that you are authorised (have permission) to perform a
certain action or to see a given page. E.g. admin users are authorised to create
new users on the website.

**Declarations** - in JavaScript declarations are `var`, `const` and `let` for
the creation of variables, constants and lexically scoped variables.

**Closure** - the scope where a variable can be accessed. A function used within another function can access the parent function's variables since its scope extends to its parent.

In this example, the variable `color` is accessible to the function `displayColor()`.

```js
function color() {
    var color = 'red';
    function displayColor() {
        alert(color);
    }
    displayColor();
}
```

**CSS Box Model** - the concept that in HTML all elements are contained within
rectangles or boxes. Each box consists of: margins, borders, padding, and the
actual content.

**Customer relationship management (CRM)** - a CRM system allows businesses to
manage business relationships and the data and information associated with them.
E.g. using CRM to track holiday bookings for a holiday bookings site. The CRM
would have information on the customer and the trip they’re planning/ have
booked and any staff members or actions that may need taking to progress or
confirm their booking.

**Create, Read, Update, and Delete (CRUD)** - CRUD refers to the 4 basic
operations you can perform on data in a relational database application. Create
a new data entry, read or retrieve existing data from the database, update the
value of an existing piece of data or delete an existing piece of data.

**Cross-Origin Resource Sharing (CORS)** - is a specification that allows
specified resources on a web page to be requested from another domain outside
the domain from which the first resource was served. E.g. uploading images using
different domains using Amazon S3. For more about origin policies see
'Same-origin Policy'.

**[Destructuring Assignment](https://en.wikipedia.org/wiki/JavaScript_syntax#Destructuring_assignment)** - 
the ability to unpack and assign variables when there are multiple parameters.

A way to simply assign the variables and then swap their values.
```js
let x, y;
[x, y] = [5, 6];
// x = 5, y = 6
[y, x] = [x, y];
// x = 6, y = 5
```
To assign values from an object.
```js
let obj = { 'a': 1, 'b': {'b1': '1.1'}}
let {a, b, b:{b1}} = obj
// a = 1, b = {'b1': '1.1'}, b1 = 1.1
```
There is an extensive list found [here](https://stackoverflow.com/questions/54605286/what-is-destructuring-assignment-and-its-uses) for more examples.

**Domain Name** - the characters/words used to identify a website after `http://` or
`www.`. The domain name consists of two parts. Take this example:
`https://dwyl.com`, `dwyl` makes up the **second level domain (SLD)** which is
then followed by `.com` which what is known as the **top level domain (TLD)** or
**parent domain**. Other examples of top level domains are: `.org`, `.co.uk`
`.io`. Domain names are the more memorable and user-friendly representation of a
website's **IP address**. Domain names are registered under the **Domain Name
System (DNS)**.

**Domain Name System (DNS)** - a distributed global directory of website domain
names (and other internet resources). The directory stores already registered
domain names along with their corresponding IP addresses.

**[Hexadecimal](https://en.wikipedia.org/wiki/Hexadecimal)** - Uses 16 different symbols. "0"-"9" to represent the values 0 to 9 and "A"-"F" ("a"-"f" is acceptable too) to represent the values 10 to 15. It's common to use
hexadecimals when working in CSS to assign colors to your elements.

The hexadecimal for dwyl's logo color is #4bc0a9 (teal).
To convert the hexadecimal into RGB values, do the following:
```
R = 4b
G = c0
B = a9

Convert the letters to their numerical value.
b = 11
c = 12
a = 10

Red: 4 * (16^1) + 11 * (16^0) = 75
Green: 12 * (16^1) + 0 * (16^0) = 192
Blue: 10 * (16^1) + 9 * (16^0) = 169
```
Hex: #4bc0a9 is RGB: 75, 192, 169.


**Hoisting** - Hoisting is JavaScript's default behaviour of moving `var`
declarations to the top of the current **scope**  when your code is run. What
this means is that whatever line your write a `var` declaration on e.g. `var x;`,
when your code is run it will automatically be lifted and read as if it were
written on the top lines of your current **scope** (to the top of the current
script or the current function).

This means that you can use `var`'s higher up in the code before the line you've
declared them on. So this example:
```js
x = "hello";
console.log(x)     // logs 'hello'
var x;            //  declaring `x` which is hoisted as if it were written at the top on compilation
```

Is read by the computer like this:
```js
var x;            //  declaring `x` which has been hoisted to the top line on compilation
x = "hello";
console.log(x)     // logs 'hello'
```

**[Higher-order Function](https://en.wikipedia.org/wiki/Higher-order_function)** - Functions that can take other functions as parameters or return them in the process. Some examples of these types of functions are the `map` and `reduce` method used for arrays.

**Hypertext Transfer Protocol (HTTP)** - the set of rules for transferring files
(text, graphic images, sound, video, and other multimedia files) on the World
Wide Web. When you enter http:// in your address bar in front of the domain, it
tells the browser to connect over HTTP.

**Initialisation** - defining a variable and providing it with an initial value:
e.g. `var x = 1;`.

**Internet Protocol (IP) Address** - a unique series of numbers or hexadecimal
digits used to identify a website.

**Microservices** - the practice of running multiple web/application servers
simultaneously. It is a widely accepted/used application architecture used in
most companies. Lambda Functions are an example of a micro Node.js Server.   

**Polymorphism** - the ability for an object to take on many forms or types e.g.
when a parent class is used to refer to a child class object. **Operator
overloading** is one form of polymorphism. It is not used in Javascript but is a
feature of C++, Scala, Ruby, Haskell and Rust.

**Progressive Web App (PWA)** - PWAs are traditional websites that are enhanced
with modern web technologies, allowing them to provide a more app-like
experience. They offer functionality such as being saved as a tile on your
mobile home screen, working offline and push notifications. The “progressive”
part means they’re “progressively enhanced” with newer features, which means
they’ll also work in older browsers that don’t support the new features. Unlike
native apps, they don't have to be updated/listed in the app store although it
is possible to list them in the app store when this is desired.

**[Regression Testing](https://www.softwaretestingmaterial.com/regression-testing/)** -
the re-running of existing tests to ensure that new changes/fixes have not
broken any existing functionality. We should perform regression testing any time
we modify an application, automated testing is a convenient way to achieve this.

**REPL (READ, EVAL, PRINT, LOOP)** - a REPL is an interactive toplevel or
language shell. A simple, interactive computer programming environment that
takes single user inputs (i.e. single expressions), evaluates them, and returns
the result to the user. They are a handy tool for experimenting with
functionality outside of the context of a project.

**Responsive Web Design (RWD)** - is designing one version of a web page which
reorders and resizes content in response to the size of a browser **at any given
point**, not just predetermined device sizes. This means the design of the site
is optimised for all screen sizes. See Adaptive Design for another approach to
designing.

**Same-origin Policy** - Under this security policy implemented by web browsers,
a document (i.e. like a web page) hosted on server A can only interact with
other documents that are also on server A. In short, the same-origin policy
enforces that documents that interact with each other have the same origin.

**Search Engine Optimisation (SEO)** - is the process of improving the visibility
of a website or web page in unpaid/organic search engine results. There are many
aspects to SEO and search engines change how it's calculated over time. It may
include the use of key words on a page, how often you add/edit content on your
site, to the way other sites link to you on the web.

**Semantic HTML** - semantic HTML is the use of HTML elements that accurately
describe what they contain/are being used for E.g. a `<p>` tag indicates that the
text within it is a paragraph whereas a `<nav>` tag should contain navigation
content and a `<footer>` should appear at the end of the page.

**Syntactic Sugar** - syntactic sugar refers to syntax in a language that is
designed to make things easier to read. The syntax makes the language "sweeter"
to use as things can be expressed more clearly or concisely. Something can be
considered "syntactic sugar" if it could be removed from the language without
removing any functionality on what the language can do. For example ternary
operators in Javascript: `x ? a : b` doesn't require the ternary operator syntax
it could also be expressed with an `if/else` statement:
```js
if(x)
 { a }
else
 { b }
```

**[Technical Debt](https://en.wikipedia.org/wiki/Technical_debt)** - Technical
debt is the time/cost of "re-working" a feature (or entire app) because corners
were cut the first time it was built. Think of Technical Debt like a "loan shark"
for your project, if you take "shortcuts" to implement a feature quickly (e.g:
by skipping tests) you will pay for it later and usually with "interest". For
more detail see: https://github.com/dwyl/product-owner-guide#what-is-technical-debt

**[Transmission Control Protocol (TCP)](https://www.webopedia.com/TERM/T/TCP.html)** -
TCP is a protocol which exists to enable the establishment of a connection and
the exchange of streams of data (multiple
[data packets](https://www.techopedia.com/definition/6751/data-packet)) between
one or more computers. TCP guarantees the delivery of data and that packets will
be delivered in the same order in which they were sent.

**[Transmission Control Protocol (TCP) handshake](https://www.techopedia.com/definition/10339/three-way-handshake)** -
A TCP handshake or three-way handshake is the first part in a three part process
for TCP data transfer between a local host/client and a server. The handshake is
a three-step method that requires both the client and server to exchange SYN and
ACK (acknowledgment) packets to establish a connection before actual data
communication begins.
