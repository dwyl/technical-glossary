<div align="center">

# Technical Glossary

This glossary is ever-evolving 
and relies on contributions <br />
from people like _you_ 
for improvements and new term suggestions ❤️. <br />
If you don't find the word or technical term you 
you are searching for, <br />
please create an issue: 
[github.com/dwyl/**technical-glossary/issues**](https://github.com/dwyl/technical-glossary/issues/new) 

[![contributions welcome](https://img.shields.io/badge/contributions-welcome-brightgreen.svg?style=flat-square)](https://github.com/dwyl/technical-glossary/issues)
[![HitCount](http://hits.dwyl.com/dwyl/technical-glossary.svg)](http://hits.dwyl.com/dwyl/technical-glossary)

</div>

## Why? 🤷‍♀️

Have you ever learnt something new 
without knowing what it's actually called? 
Or have you ever been reading about a concept 
only to get lost in the number of acronyms 
and other technical words 
used to describe what you're learning about? 🤔

This resource provides quick access, 
simple and easy to understand definitions 
to stop big words getting in the way of what could be
happy learning 😊

## What? 📝

A technical glossary for key words
you will encounter in your journey through learning creative technology.
These definitions are _deliberately_ succinct,
they aim to be easy to understand and bite-sized for quick access.
In some cases we include links where you can read more
on a given topic.

## How?

Scan down the alphabetically ordered list 
to learn about key words. 
If you don't find the word you're looking for,
or want to _expand_ on a definition,
please 
[open an issue](https://github.com/dwyl/technical-glossary/issues)
with your questions / suggestions.

### Adaptive Web Design

**Adaptive Web Design (AWD)** encourages the creation 
of several versions of a web page 
for a specified number of device dimensions. 
Which template to display
is determined in the HTTP GET request 
which recognises the screen size of the device. 
_Adaptive_ Web Design was introduced 
to deal with mobile browsing 
when most sites were optimised for desktop only. 
<!-- As devices now exist in many dimensions 
from different mobile brands through tablets to desktops,
**Responsive Web Design** 
has become a popular and more flexible alternative. -->

### Authentication

**Authentication** is the process of verifying 
that you are who you say you are
E.g. when you login to your email you use a password to authenticate your
identity. 
Other methods for authentication include using an ID card or
fingerprint/biometric method.

> **Note**: the authentication experience 
> can be a significant source 
> of frustration both as person _using_ 
> a digitial product and for the _engineers_ building it.
> We decided to build our own 
> **_Single_ Environment Variable**<sup>TM</sup> 
> drop-in solution to the problem:
> [dwyl/**auth**](https://github.com/dwyl/auth)

### Authorization

**Authorization** is checking that the person 
is authorised (has permission) 
to _access_ a given page/resource
or  to perform a certain action in an App.
e.g: a person with `admin` permissions 
is authorised to view logs in the App.

### Declarations

In `JavaScript` **declarations** 
are `var`, `const` and `let` 
for the creation of variables, constants 
and lexically scoped variables.

### Closure

The scope where a variable can be accessed. 
A function used within another function 
can access the parent function's variables 
since its scope extends to its parent.

In this example, the variable `color` 
is accessible to the function `displayColor()`.

```js
function showColor() {
    const color = 'red';
    function displayColor() {
        alert(color);
    }
    displayColor();
}
```

See:
https://developer.mozilla.org/en-US/docs/Web/JavaScript/Closures

### CSS Box Model

The concept that in HTML all elements are contained within
rectangles or boxes. Each box consists of: margins, borders, padding, and the
actual content.

See:
https://en.wikipedia.org/wiki/CSS_box_model <br />
also:


### Customer relationship management (CRM)

A CRM system allows organisations to
manage customer relationships 
and the data and information associated with them.
Typically a CRM is used for storing contact data 
and the log of communication between a business and its' cusotmers.
But increasingly CRMs are used for other functions in businesses
such as sales tracking, customer service and customer portals.

See: 
https://en.wikipedia.org/wiki/Customer_relationship_management


### Create, Read, Update, and Delete (CRUD)

CRUD refers to the 4 basic
operations you can perform 
in a database 
or application that process data. 
Create a new data entry, 
read or retrieve existing data from the database, 
update the value of an existing piece of data 
or delete an existing item of data.

See:
https://en.wikipedia.org/wiki/Create,_read,_update_and_delete


### Cross-Origin Resource Sharing (CORS)

**CORS** is a specification that allows
specified resources on a web page 
to be requested from another domain outside
the domain from which the first resource was served. 
E.g. uploading images using different domains using Amazon S3. 
For more about origin policies see
'Same-origin Policy'.
See:
https://en.wikipedia.org/wiki/Cross-origin_resource_sharing


### Destructuring Assignment

[**Destructuring Assignment**](https://en.wikipedia.org/wiki/JavaScript_syntax#Destructuring_assignment)
is the ability to unpack and assign variables 
when there are multiple parameters.

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

There is an extensive list of examples on this StackOverflow answer:
https://stackoverflow.com/questions/54605286/destructuring-assignment-uses 

### Domain Name

The characters/words used to identify a website 
after `https://` or `www.`. 
The domain name consists of two parts. 
Take this example:
`https://dwyl.com`, 
`dwyl` makes up the **second level domain (SLD)** 
which is then followed by `.com` 
which what is known as the **top level domain (TLD)** 
or **parent domain**. 
Other examples of top level domains are: 
`.org`, `.co.uk` or `.io`. 
Domain names are the more memorable 
and user-friendly representation of a website's **IP address**. 
Domain names are registered under the **Domain Name System (DNS)**.

### Domain Name System (DNS)

A distributed global directory 
of website domain names (and other internet resources). 
The directory stores already registered
domain names along with their corresponding IP addresses.

### Hexadecimal

**[Hexadecimal](https://en.wikipedia.org/wiki/Hexadecimal)**
Uses 16 different symbols: "0"-"9" and "A"-"F" 
to encode data.
It's common to use hexadecimals 
when working in CSS 
to assign colors to your elements.

The hexadecimal for dwyl's logo color is 
[`#4bc0a9`](https://color-hex.org/color/4bc0a9) 
(teal).

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

### Hoisting

**Hoisting** is JavaScript's default behaviour 
of moving `var` declarations 
to the top of the current **scope** 
when your code is run. 
What this means is that whatever line you write a `var` declaration on 
e.g. `var x;`,
when your code is run 
it will automatically be lifted 
and read as if it were written on the top lines of your current **scope** 
(to the top of the current
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

This is obviously confusing/undesireable code,
please don't do this!

### Higher-order Function

**[Higher-order Function](https://en.wikipedia.org/wiki/Higher-order_function)** 
are functions that take other functions as parameters 
and/or return a function. 
Some examples of these types of functions are the 
[`map`](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/map) and 
[`reduce`](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/Reduce) 
method used for arrays. 
They both accept a function to use on the elements in the given array.

```js
// perform an action twice
function twice (func, value) {
  return func(func(value));
}

// func can be any simple (preferably pure) function:
function func (value) {
  return value + 3;
}

console.log(twice(func, 1)); // 7
console.log(twice(func, 7)); // 13
```

Not to be confused with "pure" functions.
To undersand the difference,
please see:
[dwyl/learn-redux/issues/40](https://github.com/dwyl/learn-redux/issues/40#issuecomment-272489779) 


### Hypertext Transfer Protocol (HTTP)

**Hypertext Transfer Protocol (HTTP)** 
is the set of rules for transferring files
(text, graphic images, sound, video, and other multimedia files) 
on the World Wide Web. 
When you enter http:// in your address bar in front of the domain, 
it tells the browser to connect over HTTP.

### Initialisation

Defining a variable 
and providing it with an initial value:
e.g: 
```js
var x = 1;
```

### Internet Protocol (IP) Address

A unique series of numbers or hexadecimal
digits used to identify a website.

See:
https://en.wikipedia.org/wiki/IP_address

### Microservices

The practice of splitting the business logic of your App/business
into multiple distinct self-contained services 
and deploying them individually. 
It is a widely accepted/used application architecture. 
Lambda Functions are an example of a micro Node.js Server.

See:
https://en.wikipedia.org/wiki/Microservices

### Polymorphism

The ability for an object to take on many forms or types 
e.g:
when a parent class is used to refer to a child class object. 
**Operator overloading** is one form of polymorphism. 
It is not used in Javascript but is a
feature of C++, Scala, Ruby, Haskell and Rust.

See: 
https://en.wikipedia.org/wiki/Polymorphism_(computer_science)

### Progressive Web App (PWA)

PWAs are traditional websites that are enhanced
with modern web technologies, allowing them to provide a more app-like
experience. They offer functionality such as being saved as a tile on your
mobile home screen, working offline and push notifications. The “progressive”
part means they’re “progressively enhanced” with newer features, which means
they’ll also work in older browsers that don’t support the new features. Unlike
native apps, they don't have to be updated/listed in the app store although it
is possible to list them in the app store when this is desired.

### Regression Testing

**[Regression Testing](https://www.softwaretestingmaterial.com/regression-testing/)** -
the re-running of existing tests to ensure that new changes/fixes have not
broken any existing functionality. We should perform regression testing any time
we modify an application, automated testing is a convenient way to achieve this.

### REPL

**REPL (READ, EVAL, PRINT, LOOP)** 
is an interactive programming language shell. 
A simple, interactive computer programming environment 
that takes single user inputs (i.e. single expressions), 
evaluates them, and returns the result to the user. 
They are a handy tool for experimenting with
functionality outside of the context of a project.
_Most_ programming languages have them.
In `JavaScript` you can type `node` in your terminal
and then type any expression e.g:


```js
> console.log("Hello World!")
Hello World!
```

Similarly in `Elixir` we have `iex`:

```sh
iex
iex(1)> IO.inspect("hello world")
"hello world"
```

### Responsive Web Design

**Responsive Web Design (RWD)**
is the practice of designing one version 
of a web page which reorders and resizes content 
in response to the size of a browser **at any given point**, 
not just predetermined device sizes. 
This means the design of the site
is optimised for all screen sizes. 
See Adaptive Design for another approach to
designing.

### Same-origin Policy

The **security policy** implemented by web browsers,
whereby a document (i.e. like a web page) hosted on a server 
can only interact with other documents the _same_ server. 

### Search Engine Optimisation (SEO)

**Search Engine Optimisation (SEO)** 
is the process of improving the visibility
of a website or web page 
in unpaid/organic search engine results. 
There are many aspects to SEO 
and search engines change how it's calculated over time. 
It may include the use of key words on a page, 
how often you add/edit content on your site, 
to the way other sites link to you on the web.

### Semantic HTML

**Semantic HTML** is the use of HTML elements
that accurately describe 
what they contain/are being used for 
E.g: a `<p>` tag indicates that the text within it is a paragraph 
whereas a `<nav>` tag should contain navigation content 
and a `<footer>` should appear at the end of the page.

### Spike

A **spike** is a product development method 
that uses the **_simplest_ possible experiment** 
to explore potential solutions to a problem.
It can be just a basic design/interface test (wireframe)
or a technical exploration often called a **proof of concept** (POC).
See: https://en.wikipedia.org/wiki/Spike_(software_development)

> Remember a [problem well-stated is half solved](https://youtu.be/wO1WVguNQAM)
> so define the problem you're trying to solve with your spike
> _before_ attempting to solve it.
> e.g: by creating an issue to capture the requirements.

**`@dwyl`** our **spike** mini-projects 
are usually **time-boxed** 
anything from an hour to a day of effort.
The **objective** is to **capture the _learning_**
as much as it is to test the interface or technical implementation.
Therefore we always create a new GitHub repo to _capture_ the experiment.
Sometimes we will include the word "spike" in the repo,
e.g: 
[dwyl?q=**spike**](https://github.com/dwyl?q=spike)
Other times, we will _expand_ the repo into an **_example_ app**
that is more of a **tutorial** that _anyone_ can follow,
e.g: 
[dwyl/repositories?q=**example**](https://github.com/orgs/dwyl/repositories?q=example)
We have _plenty_ of recent examples of single-feature
spike experiments,
but we have been capturing our learning this way for a long time,
e.g: 
[dwyl/**meteor-search**](https://github.com/dwyl/meteor-search).

However much detail you include in your spike,
remember that the objective is to
**_communicate_ what you tried**
so that other people can **_replicate_ the experiment**.
It's not enough for _you_ to know that it worked (or failed),
you need to **share _everything_ you learned** along the way.
If you skip steps in your log of the spike
so other people 

### Syntactic Sugar

Syntactic sugar refers to syntax in a language that is
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

### Technical Debt

**[Technical Debt](https://en.wikipedia.org/wiki/Technical_debt)** is the time/cost of "re-working" a feature (or entire app) because corners
were cut the first time it was built. Think of Technical Debt like a "loan shark"
for your project, if you take "shortcuts" to implement a feature quickly (e.g:
by skipping tests) you will pay for it later and usually with "interest". For
more detail see: https://github.com/dwyl/product-owner-guide#what-is-technical-debt

### Transmission Control Protocol (TCP)

**[Transmission Control Protocol (TCP)](https://www.webopedia.com/TERM/T/TCP.html)**
is a protocol which exists to enable the establishment of a connection and
the exchange of streams of data (multiple
[data packets](https://www.techopedia.com/definition/6751/data-packet)) between
one or more computers. TCP guarantees the delivery of data and that packets will
be delivered in the same order in which they were sent.

A **[Transmission Control Protocol (TCP) handshake](https://www.techopedia.com/definition/10339/three-way-handshake)**
is the first part in a three part process
for TCP data transfer 
between a local host/client and a server. 
The handshake is a three-step method 
that requires both the client 
and server to exchange SYN 
and ACK (acknowledgment) packets 
to establish a connection before actual data
communication begins.
