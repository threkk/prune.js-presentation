---
theme: seriph
class: intro
background: /1-cover.jpg
highlighter: shiki
lineNumbers: true
---
# Dead Code Detection on Strict ECMAScript 6 Projects
## Alberto Martínez de Murga Ramírez
### Supervisor: Vadim Zaytsev

<!--
My name is Alberto Martinez de Murga Ramirez. My research has been based around
dead code detection in ECMAScript 6 projects. I started this research on 2017
as part time single student when I was working on a small startup here. 4 years
later, I am working at Booking.com in the experimentation department, I got
married, moved houses 2 times and lived in France briefly.

The problem of dead code in JavaScript is still relevant and I hope to make a
different about it today.
-->
---
layout: fact
---
# What is dead code?

<br />

> ## _Dead code is code which is never used or reachable. It is not harmful by itself since it does nothing but it is considered a “bad smell” in the code. A “bad smell” is a symptom of bad implementation or design that corresponds to a deeper problem in the system._

<!--
- Very common issue in all langauges.
- If affect around 30% of the codebase.
- Two main reasons: YAGNI and software evolution
- Web applications are one of the most common software program.
- They are constantly evolving and change very fast
- Lehman's classification type E
    - S - Specification, formally defined
    - P - Problem, may be formulated but approximated.
    - E - Embedded in the real world.
- Frontend can be only written in JavaScript. JavaScript evolves very fast.
- React has major versions since 2003.
- Fast evolution implies dead code.
- We aim to create a tool that detects this type of code.
-->
---
layout: two-cols
---

# Academy
- Not many initiatives in this area.
- Combination of static and dynamic analysis.
- Targets ECMAScript 5
- _JSNOSE, Lacuna_

::right::

# Industry
- Tools created for developers without academic research behind.
- Mostly static analysis.
- _ESLint_: Linter. Syntactic analysis, not semantic.
- _Rollup, webpack_: Transpilers. Three-shaking
<style>
ul { padding-top: 2.5em; li { font-size: 1.5em; } }
em { color: teal; }

</style>
<!--
- JavaScript is the language, ECMAScript is the specification of the language
- JNOSE: combination of metrics and thresholds.
- Lacuna: Combination of flow graphs and call graphs.
- Three-shaking: drops files and fragments of code during minification.
-->
---
layout: statement
---
# What is JavaScript

> ## Small glue language easy to use by designers and part-time programmers to assemble components like images.
## Curly-bracket syntax, dynamic, prototye based, first class functions.
## Multiparadigm

<style>
h2 { padding: 0.5em; }
blockquote { padding: 1.5em; }
</style>
<!--
- Like C, Java
- Dynamic types and everything in general.
- There have been implementations server side. Netscape introduced an implementation of the language into Netscape Enterprise server (1995) and Microsoft supported JSCript in ASP an .NET (1996). In 2009 Nodejs was released using the JavaScript engine V8 of Google Chrome browser.
- It is also used in databases (MongoDB, DynamoDB), videogames (UnityScript), operative systems (JavaScript for Autommation, WinJS) and phone programming (React Native, Cordova, KaiOS).
-->
---
layout: quote
---
# History of JavaScript: first versions
- **1995:** Created by Brendan Eich as part of the version 2.0 of Netscape.
- **1996:** Netscape submitted the JavaScript specification to the _European Computer Manufacturers Associations_ (ECMA).
- **1997:** Release of ECMAScript version 1.
- **1998:** ECMAScript version 2.
- **1999:** ECMAScript version 3.

<style>
ul { padding-top: 2.5em; li { font-size: 1.5em; } }
strong { background-color: teal; }
</style>

<!--
- Brendan Eich will become CEO of Mozilla and Brave
- Submitted with the intention that other browsers could implement the JavaScript language
- Only run on Netscape, but Microsoft reverse engineered its own scripting technologies for the browser Internet Explorer, named VBScript and JScript.
- Originally, Microsoft had no intention of implementing JavaScript on Internet Explorer.
- This was a big problem for developers trying to support all the browsers.
- _Best viwed in..._
-->
---
layout: quote
---
# History of JavaScript: the drama
- **2003:** ECMAScript 4 started to be developed, with participants very divided.
- **2008:** Both sides meet in Oslo and reach an agreement. ECMAScript 4 was never completed, but a subset of it was released as ECMAScript 3.1
- **2009:** ECMAScript 5 gets released. Common base for JavaScript.
- **2010:** ECMAScript 5.1 gets released to align with _ISO/IEC 16262_.
- **2015:** ECMAScript 6. Most improvements ever released.

<style>
ul { padding-top: 2.5em; li { font-size: 1.5em; } }
strong { background-color: teal; }
</style>

<!--
- There were two sides:  Adobe, Mozilla and Macromedia vs Microsoft, Yahoo and Google.
- Issues about how ambitious the changes should be and the possible backwards compatibility issues.
- They agreed on collaborating in the development of ECMAScript 5.
- ISO specification for JavaScript.
- Since then, one new version every year:  v7 (2016), v8 (2017)...
-->
---
layout: default
---
# JavaScript as a language
<!-- Picture of the holy trinity, tweet, protype chain graph -->

---
<!-- Limitations-->

<!-- Choices and challenges -->

---
<!-- What can we do -->

<!-- Approach summary -->

---
<!-- What does the tool do -->

<!-- Call graph code vs graph
Dead code explanation and picture of the forest. Big picture. -->

---
<!-- Results -->
<!-- Project analysed, results -->

---
<!-- Conclusions -->
