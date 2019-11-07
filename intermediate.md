---
title: "What to Do Next: Intermediate"
subtitle: "Learning about the difference between font end and back end code and more advanced front end code."
layout: default
prevpage: novice.html
prevtitle: "What to Do Next: Beginners"
nextpage: advanced.html
nexttitle: "What to Do Next: Advanced"
---

<h2 class="anchor" id="intermediate">Intermediate Difficulty</h2>

<p>This is where things start to get more difficult, but you don't need to be a professional web developer yet. You'll need to be rather familiar with HTML, CSS, and JaveScript.</p>

<p>From this point on, everything will be discussed in terms of of two categories: <strong>front end</strong> and <strong>back end</strong>. Here's what these terms mean:</p>

<ul>
    <li><strong>Front End</strong> &mdash; also called "client side" &mdash; means that you are programming the user's browser. This includes HTML, CSS, DOM, and client-side (browser side) JavaScript. It also includes things like jQuery, Bootstrap, Processing.js, and any other library that works in the browser. So far everything you've done has been front end.</li>
    <li><strong>Back End</strong> &mdash; also called "server side" &mdash; refers to programming the web server. Code that runs on the web server can <em>render</em> HTML (which means a computer program generates the HTML instead of just sending an HTML file) or implement <em>web services</em> that allow client side JavaScript code to connect to databases to retrieve data or store it in a more permanent manner. In general, code that runs on the server can gain access to things that live on servers like databases, and can serve as a hub for communication between users such as chat rooms and message forums.</li>
</ul>

<p>Any time you hear about something new, like Express.js, you should ask yourself "is this front end or back end stuff?" If something falls into the back end category then you need a server that will support it. Express.js is a back end framework that runs on node.js (which is effectively a web server). Some things are frameworks with both front and back end parts to them, but it is more common to find frameworks for one or the other.</p>

<p>Not all hosting services support back end development. KISSr, for example, doesn't support any back end development at all. All it will do is send your files to the browser and any code will have to run in the browser. Other web hosting services may only support PHP and the MySQL database, but not node.js. Yet others might support almost anything if you know what you're doing.</p>


<h3>More Advanced Web Tutorials</h3>

<p>Before moving on, check out <a href="https://www.freecodecamp.com/">FreeCodeCamp</a>. You could almost just go to this site and forget about the rest of this page. They have almost everything you need to know including:</p>
<ul>
    <li><strong>Front End Development Certification:</strong> HTML5, CSS, JavaScript, Bootstrap, jQuery, Object Oriented and Functional Programming, JSON/Ajax, Algorithms</li>
    <li><strong>Data Visualization Certification:</strong> Sass, React, D3</li>
    <li><strong>Back End Development Certification:</strong> Testing/Debugging, Git, Node.js/Express.js, MongoDB</li>
    <li><strong>Full Stack Development Certification:</strong> Requires using what you learned above to complete real working projects for non-profit groups.</li>
</ul>
<p>But in case that seems like too much to bite off at the moment, I've provided some other suggestions below.</p>


<h3>Learn Bootstrap</h3>

<p><a href="http://getbootstrap.com/">Bootstrap</a> is a HTML, CSS, and JavaScript <a href="https://en.wikipedia.org/wiki/Front-end_web_development">front-end</a> <a href="https://en.wikipedia.org/wiki/CSS_frameworks">UI framework</a> that improves layout across devices with different screen sizes (responsive design) and provides a large number of HTML/CSS components for you to use. This may sound complicated, but it makes it easy to create some very professional looking web pages. In fact, this page was created using Bootstrap 4.</p>

<p>One of the biggest advantages of using Bootstrap is <a href="https://en.wikipedia.org/wiki/Responsive_web_design">responsive design</a> which means that anything created with it almost automatically looks good on everything from a mobile phone screen to a desktop web browser.</p>

<p>Bootstrap tutorials are available at <a href="http://www.w3schools.com/bootstrap/default.asp">w3schools.com</a>, <a href="http://www.tutorialspoint.com/bootstrap/">tutorialspoint</a>, and <a href="https://www.tutorialrepublic.com/twitter-bootstrap-tutorial/">TutorialRepublic</a>.</p>


<h3>Learn Vue</h3>

<p>You may be able to create dynamic web pages with DOM methods or jQuery, but there's a better way! These days there are a nuber of frameworks for <em>reactive</em> HTML that will automatically update your page for you whenever you change a property in JavaScript. The top three frameworks that do this for you, among other things, are Angular, React, and Vue.</p>

<p>But I recommend learning <strong><a href="https://vuejs.org/">Vue</a></strong> because it is simple, works well, and is easy to learn. There are also good learning materials for it online.</p>

<p>Here's an excellent video about how it works:</p>

<p><div class="embed-responsive embed-responsive-16by9">
    <iframe class="embed-responsive-item" src="https://player.vimeo.com/video/247494684" allowfullscreen></iframe>
</div></p>

<p>If you're already hooked on the whole idea after watching that, then <a href="https://www.vuemastery.com/courses/intro-to-vue-js/vue-instance">Watch the Intro Course Videos</a> and after you've done that move on to the <a href="https://vuejs.org/v2/guide/">Official Vue Guide</a>.</p>


<h3>Learn SQL</h3>

<p>If you haven't already, learn SQL with the <a href="https://www.khanacademy.org/computing/computer-programming/sql">Intro to SQL: Querying and managing data</a> lessons on Khan Academy or something similar.</p>

<p>After learning SQL, you might want to install some free SQL relational database software on your own computer. The two most popular free and open source SQL relational databases are MySQL and PostgreSQL. Both of these come with installers and excellent GUI management tools.</p>
<ul>
    <li><a href="http://mysql.com">MySQL</a> - This one has a very good GUI management client with database schema design diagramming built in.</li>
    <li><a href="http://www.postgresql.org/">PostgreSQL</a></li>
</ul>
<p><a href="http://sqlfiddle.com/">SQLFiddle</a> can be used for sharing code you're having trouble with or testing things out without having to install database software.</p>


<h3>More Advanced Code Testing Sandboxes and Playgrounds</h3>

<p>Here are some sites where you can play around with JavaScript, Bootstrap, other front-end frameworks, and in some cases even experiment with server-side scripting using Node.js and Express.js:</p>
<ul>
    <li><a href="https://glitch.com/">Glitch</a> supports <a href="https://nodejs.org/">Node.JS</a> and <a href="http://expressjs.com/">Express.js</a> for server side scripting! (Recommended)</li>
    <li><a href="http://c9.io">Cloud9</a> is the king of online development tools. You can get a free account with a full in-browser IDE that allows you to create workspaces (containers) where you can do almost anything and use almost any language, even C++. This is a great place to practice if you want to learn something other than Node.js, PHP, or SQL.</li>
    <li><a href="http://codepen.io/pen/">Codepen</a> is client-side only but supports a number of JS libraries.</li>
    <li><a href="http://jsbin.com">JSBin</a> is similar to Codepen in capability.</li>
    <li><a href="https://jsfiddle.net/">JSFiddle</a> is similar to the previous two but has Processing.js as a library option. You can still use Processing.js with the others, there's just no shortcut for adding the script link for it.</li>
    <li><a href="http://sqlfiddle.com/">SQLFiddle</a> for runnig SQL and sharing SQL that you need help with.</li>
</ul>
