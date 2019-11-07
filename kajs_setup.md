---
title: "Khan Academy Javascript Setup"
subtitle: "Instructions for using Khan Academy's Processing.js on your own web site."
layout: default
nextpage: novice.html
nexttitle: "What to Do Next: Beginners"
prevpage: site_setup.html
prevtitle: "Site Setup"
---


<h2 class="anchor" id="ka-processingjs">Running Processing.js Programs from Khan Academy on Your Site</h2>

<p>This part is optional. It only applies if you have created your own programs using JavaScript+Processing.js on Khan Academy and want to embed them in your site's pages.</p>

<h3>Khan Academy Processing.js Template</h3>

<p>You can use your programs from Khan Academy on your own web site, but you will need to add a little extra code to them to make them work. The main thing you need is the <a href="https://www.khanacademy.org/computer-programming/processingjs-inside-webpages-template/5157014494511104">Processing.js Template</a> from the Khan Academy web site. Here is a stripped-down version of it with the important parts:</p>
<pre class="code">
&lt;body&gt;
&lt;!--Place the canvas element where you want the canvas to appear --&gt;
&lt;canvas id="mycanvas"&gt;&lt;/canvas&gt;

&lt;!-- This causes the browser to load the Processing.js library --&gt;
&lt;script src="https://cdn.jsdelivr.net/processing.js/1.4.8/processing.min.js"&gt;&lt;/script&gt;
&lt;script&gt;
    var sketchProc = function(processingInstance) {
        with (processingInstance) {
            size(400, 400);
            frameRate(30);

            // YOUR CODE STARTS HERE

            /***** Replace this line with your code from KA. *****/

            // YOUR CODE ENDS HERE
        }};
    var canvas = document.getElementById("mycanvas");
    var processingInstance = new Processing(canvas, sketchProc);
&lt;/script&gt;
&lt;/body&gt;
</pre>

<p>Just copy the needed parts of this snippet to your HTML file and replace the indicated comment line with your code.</p>

<p>Put the <code>&lt;canvas&gt;</code> tag wherever you want the program's canvas to appear. There is an example program below so you can see what it will look like. If it helps any, you can also use the <strong>View Page Source</strong> function in your browser to view the HTML of this page to see how it is coded.</p>

<div class="canvas">
    <!--This draws the ProcessigJS Canvas on the web page -->
    <canvas id="mycanvas"></canvas><br>This is <a href="https://www.khanacademy.org/computer-programming/spin-off-of-project-paint-splatter/5316498611372032">Paint Splatter</a> from Khan Academy.
</div>

<p>You can CSS style the <code>&lt;canvas&gt;</code> element to control things like the placement and margin of the canvas. If you want a different canvas size or frame rate, change the numbers in this part of the code:</p>
<pre class="code">
...
with (processingInstance) {
    size(400, 400);
    frameRate(30);
...
</pre>

<h3>Differences Between Khan Academy's Processing.js and the Standard Version</h3>

<p>There are some differences between the Processing.js library used by Khan Academy and the standard one that you will be using on your own web pages.</p>

<p><strong>The good news:</strong> You can now use some Processing.js functions and JavaScript features that don't work on Khan Academy! See the following documentation for all the cool stuff you can do now:</p>
<ul>
    <li><a href="http://processingjs.org/reference/">Processing.js Reference</a> for the full list of Processing.js functions.</li>
    <li><a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript">JavaScript Reference</a> (ECMAScript 5.1)</li>
</ul>

<p><strong>The bad news:</strong> You might need to make some minor code changes to get your code working outside of KA. Fortunately, this usually only means adding a line or two of code. <a href="https://khanacademy.zendesk.com/hc/en-us/articles/202260404-What-parts-of-ProcessingJS-does-Khan-Academy-support-">See here</a> for some differences between KA and the standard Processing.js library.</p>
