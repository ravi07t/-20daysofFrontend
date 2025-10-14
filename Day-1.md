Day-1 Focus:

1.	What is the difference between HTML and HTML5?
HTML5 is the latest version of HTML that supports audio, video, local storage, semantic tags, and APIs (like Geolocation).
<!-- HTML4 -->
<div id="header"></div>

<!-- HTML5 -->
<header></header>

2.	What are semantic elements in HTML5? Give examples.
Semantic elements describe the meaning of content (improves readability & SEO).
Examples: <header>, <footer>, <section>, <article>, <nav>.
<article>
  <h2>Frontend Developer</h2>
  <p>Building interactive UI using ReactJS.</p>
</article>

3.	What’s the purpose of the <!DOCTYPE html> declaration?
Declares the latest HTML version to the browser.
<!DOCTYPE html>

4.	Difference between <div> and <span> tags?
<div> → block-level element
<span> → inline element

5.	What are meta tags used for?
Define metadata (SEO, viewport, charset, CTR, SERP, etc.)
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">

6.	What are the different types of CSS selectors?
element, class, id, universal, attribute, pseudo-class
h1 { color: red; }
.title { color: blue; }
#main { color: green; }
* { color: yellow; }
[type=radio]{ color: blue; }

7.	What’s the difference between inline, internal, and external CSS?
•	Inline CSS: Applied directly within an HTML open tag with style attribute, affecting only that specific element.
        <!-- Inline -->
<h1 style="color: red;">Hello</h1>
•	Internal CSS: Defined within a <style> tag in the <head> section of an HTML document.
        <!-- Internal -->
<style>h1 { color: blue; }</style>
•	External CSS: Contained in separate .css file linked to the HTML document there we can use styles.
        <!-- External -->
<link rel="stylesheet" href="style.css">

8.	Explain the concept of specificity in CSS.
Inline > id > class > element

9.	What are pseudo-classes and pseudo-elements?
Pseudo-classes: Single colon (:) followed by name(:hover, :link, :active, :focus, :first-child, etc.)
/* Pseudo-class */
button:hover { background: blue; }
Pseudo-elements: Double colon (::) followed by name(::before, ::after, ::first-letter, ::first-line, ::selection, etc.)
/* Pseudo-element */
p::first-letter { font-size: 24px; }

10.	What’s the difference between static, relative, absolute, fixed, and sticky positioning?
•	Position: static - Document flows static in default ‘top, bottom, left, right’ - These properties have no effect. 
•	Position: relative - Document flows following the normal flow ‘top, bottom, left, right’ - These properties are used to move the element from its original position. 
•	Position: absolute - absolute removes the element from the flow to position it relative to a positioned ancestor (Relative to the nearest positioned ancestor) ‘top, bottom, left, right’ - Used to set the final position relative to its containing element. 
•	Position: fixed - fixed removes it from the flow to position, making it stay in place during scrolling
