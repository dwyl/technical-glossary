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
the creation of variables.

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

**Hoisting** - Hoisting is JavaScript's default behaviour of moving `var`
declarations to the top of the current **scope**  when your code is run. What
this means is that whatever line your write a `var` declaration on e.g. `var x;`,
when your code is run it will automatically be lifted and read as if it were
written on the top lines of your current **scope** (to the top of the current
script or the current function).

This means that you can use `var`'s higher up in the code before the line you've
declared them on. So this example:
```
x = "hello";
console.log(x)     // logs 'hello'
var x;            //  declaring `x` which is hoisted as if it were written at the top on compilation
```

Is read by the computer like this:
```
var x;            //  declaring `x` which has been hoisted to the top line on compilation
x = "hello";
console.log(x)     // logs 'hello'
```

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

**Regression Testing** - the re-running of existing tests to ensure that new
changes/fixes have not broken any existing functionality.

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
```
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
a fuller definition see: https://github.com/dwyl/product-owner-guide#what-is-technical-debt
