---
title: "Site Setup"
layout: default
subtitle: "Instructions to help Khan Academy students and others create a working public web site using what they've learned about HTML, CSS, and JavaScript."
nextpage: kajs_setup.html
nexttitle: "Khan Academy JS Setup"
prevpage: index.html
prevtitle: "Home"
---

<h2 class="anchor" id="setup">Site Setup for HTML/CSS/JS</h2>
<p>Below are the instructions for setting up your static web site. A static web site is the simplest type of web site. There are no scripts or SQL databases running on the server, but it is sufficient for <a href="https://en.wikipedia.org/wiki/Front-end_web_development">front-end web development</a>. This means that <strong>SQL is not supported</strong> on this type of site. (<a href="https://glitch.com/">Glitch</a> actually does support a node.js backend including different databases. But this is a bit more complex to use.)</p>

<p>Anything you have learned about HTML, CSS, and JavaScript will work in this environment. You can write JavaScript that will work in the browser of anyone visiting your site.</p>

<div class="alert alert-danger" role="alert"><strong>Alert:</strong> If you are under 18 (or considered a minor according to the laws in your locale) please talk to your parents or legal guardian about setting up your web site before proceeding!</div>


<div class="container step-reset">

<h3 class="step">Create a Dropbox Account</h3>
<p>First, you will need a Dropbox account. This will provide network storage space for your web site, and you can use it for storing other files too. If you already have a Dropbox account, you can skip this part since you can use your existing Dropbox account with KISSt.</p>
<ol>
    <li>Create an account on <a href="https://db.tt/JBhh3niM">Dropbox.com</a> - Please use <a href="https://db.tt/JBhh3niM">this link</a> to help the author of this guide. That way he will get referral credit which increases the storage limit on his own Dropbox account. (Thank you in advance for your help!)</li>
    <li>Install the <a href="https://db.tt/JBhh3niM">Dropbox Software</a> on your computer. The Dropbox software automatically syncs the Dropbox folder on your computer to your Dropbox account. This means you won't have to manually upload files.</li>
</ol>
<p>Here is a video about how to install Dropbox if you need help, but it is not very difficult.</p>

<div class="embed-responsive embed-responsive-16by9">
    <iframe class="embed-responsive-item" src="https://www.youtube.com/embed/zAsye_RDnAg" allowfullscreen></iframe>
</div>

<h3 class="step">Log in to KISSr</h3>
<p>First make sure you are already logged in to your <a href="https://db.tt/JBhh3niM">DropBox account</a>. Then, after logging in to dropbox via dropbox.com, go to <a href="https://www.kissr.com/">KISSr</a> and authorize it to link to your dropbox account. This will not disclose your Dropbox password to KISSr.</p>

<p>Create your subdomain of the form: <code>yoursitename.kissr.com</code> where <code>yoursitename</code> is replaced with a name you choose. Pick something good because you can't easily change it once you tell people about it.</p>

<h3 class="step">Download and Install a Code Editor</h3>
<p>To edit the code for your site, you will need a text editor. Using a <strong>code editor</strong>, a type of text editor that is designed with HTML and other code editing in mind, is essential for making it easier to write code. Here are some options which range from easiest to more difficult. All of these are free.</p>
<ul>
        <li><a href="http://brackets.io/">Brackets</a> is the easiest choice. It comes with many good features, such as a color picker, and good default settings for HTML, CSS, and JavaScript.</li>
        <li><a href="https://code.visualstudio.com/">VS Code</a> is similar, but it is somewhat more advanced and oriented toward programming in general.</li>
</ul>
<p>You can use any text editor, even Windows Notepad or OS X TextEdit, but the rest of this tutorial will assume you are using one of the code editors listed above. Your editor doesn't need any special file upload features because you're just going to edit your files locally and Dropbox Sync will automatically upload your changes to your Dropbox storage. Once uploaded to Dropbox, your files automatically become available to the web server.</p>

<p>Here is a beginner's level video about Brackets that introduces you to its features.</p>

<div class="embed-responsive embed-responsive-16by9">
    <iframe class="embed-responsive-item" src="https://www.youtube.com/embed/GN0txxeT46A" allowfullscreen></iframe>
</div>

<h3 class="step">Launch the Editor and Open Your Site Folder</h3>
<p>Launch your editor, use the <strong>File-&gt;Open Folder</strong> menu option, then navigate to the <code>Dropbox\Apps\KISSr</code> folder on your local hard drive. Select the folder inside that has the same name as your web site and click the <strong>Open</strong> button.</p>

<h3 class="step">Edit Your index.html File</h3>
<p>The <code>index.html</code> file is the main page on your site. In your editor in the sidebar on the left, you will see the <code>index.html</code> file. Click on it to start editing. You can put other html files in the same directory, or create them from within the editor and save them in your site directory, and they will show up here.</p>

<p>KISSr automatically creates an <code>index.html</code> file for you as a template, but you can delete the entire contents of the file and start over if you want. There is nothing special about the code in the file, and no reason to keep any of it if you do not want it.</p>

<p>Changes you make to the file, or any other files, will not be available on your web site until:</p>
<ol>
    <li>You save the file, and</li>
    <li>Dropbox Sync has a few seconds to upload the file.</li>
</ol>
<p>Small files like text files sync very quickly so it will probably happen too fast for you to notice. If you have any problems, check the Dropbox status icon to see if there are any warnings or error messages.</p>

<h3 class="step">Verify Operation</h3>

<p>Now that you've made some sort of change to your <code>index.html</code> file, load your new site in your browser to see if it's working. By now you have probably figured out that the URL will be <code>http://yoursitename.kissr.com/</code> where <code>yoursitename</code> is the subdomain name you used.</p>

<p>You don't need to put a filename at the end of the URL. This is because <code>index.html</code> is a special filename that the server knows to look for when a specific filename is not in the URL. Any other files in the same directory will need to have their filename specified in the URL.</p>

<p>If you create a subdirectory in your site folder then you can put an <code>index.html</code> file in the subdirectory, and it will return that file if someone uses the URL <code>http://yoursiename.kissr.com/subdir/</code> where "subdir" is the name of the directory. Practically every single web server works ths way, so you can assume this works on any web server.</p>

<p>Notice that when you make changes to an HTML file you will need to use the page reload button on your web browser before they become visible.</p>

<p><strong>TIP:</strong> You can also just double-click on an html file from a file browser window on your desktop and this will load the file into your browser from the local hard drive. This is a good way of checking your code more quickly when you are editing it. The code editors mentioned above also have functions or extensions that will do this for you automatically every time you save a file. Brackets has a live preview feature that will update your browser as you type so you don't even have to save the file to see the preview.</p>

<h3 class="step optional">Upload Images for Your Site</h3>
<p>To upload images, open a file browser window (File Explorer in Windows or Finder in OS X) on your desktop, go to the <code>Dropbox\Apps\KISSr\yoursitename.kissr.com</code> folder and just copy your images in there.</p>

<p>It is strongly recommended that you create a subdirectory called <code>img</code> in your site folder and place all images in there. That will help prevent your site folder from getting too messy.</p>

<p>Once your image or images have been uploaded, you can use them with a an image element like <code>&lt;img src="img/myimage.jpg"&gt;</code>.</p>

<h3 class="step">Create Your Site Content</h3>

<p>You are now done with the initial setup of your new web site! Now all you have to do is keep creating your site content using your HTML, CSS, and possibly JavaScript skills. Don't forget to tell tell everyone about it.</p>

<h3 class="step optional">Register a Domain Name</h3>

<p>This is completely optional and it's the only thing here that costs money, but some domains are extremely cheap (less than US$1/year).</p>

<p>If you don't like the domain name <code>kissr.com</code> (most people wouldn't blame you) you can register your own domain name. <a href="https://www.namecheap.com/domains.aspx">NameCheap</a> will register some domains for less than US$1 per year, but the catch with them is that the price goes way up after a year. Fortunately most domains can be transferred to a different registrar.</p>

<p>The best thing to do is check out <a href="http://www.registrarowl.com/report_registrar_price_comparison.php">Registrar Owl</a> for a massive price comparison list. Don't forget to take <a href="http://www.registrarowl.com/report_registrar_free_whois_privacy.php">Whois Privacy</a> into account because many registrars charge money to keep your name and address out of the whois database. (Thanks to <a href="http://ejohn.org/blog/low-cost-com-domains-with-whois-privacy/">John Resig</a> for pointing this out on his blog.)</p>

<p>Once you have registered a domain name, you will need to point a DNS record to the web server. Instructions on how to do that are <a href="https://www.kissr.com/pages/documentation">available here</a>. You can also use a URL redirect if necessary.</p>

<p>Domain names are useful not just because you can pick your own name, but also because they allow you to move your site to a different server without changing the URL. So if you later decide to move your site to a web server with more features, all you will need to do is update the DNS record for the domain to point to the new server. Nobody will even notice that you moved your site to a different service because the URL for your site will stay the same.</p>


<h2>Oh Noes! Where is Oh Noes! the Error Buddy?</h2>

<p>He needs some rest and is sitting this one out. Actually, there is no "Oh noes! the error buddy" in a standard web browser environment!</p>

<p>The training wheels are off now, but the good news is you are in the same browser environment as professional web developers. To see errors, look for the <strong>JavaScript Console</strong> in your browser menus. On Firefox it is under <strong>Tools-&gt;Web Developer-&gt;Web Console.</strong> For this option to appear in the menus you may need to enable developer or debugging options in your browser configuration depending on which browser you are using.</p>

<p>You can also learn more about how to access the web developer tools in your browser at <a href="https://www.wickedlysmart.com/hfjsconsole/">this web site</a> or <a href="http://webmasters.stackexchange.com/questions/8525/how-to-open-the-javascript-console-in-different-browsers">this one</a>.</p>

<p>The code editors mentioned above also have syntax checking features that can warn you of some types of errors as soon as you type them. Read the manual for your code editor to find out more about these. You may need to download and install extension packages to get some of these features.</p>

<p>And if you don't like Oh Noes! on Khan Academy and want to get rid of him, <a href="https://khanacademy.zendesk.com/hc/en-us/community/posts/218698787-Oh-Yes-A-UserScript-to-get-rid-of-Oh-Noes-the-Error-Buddy">see here for instructions</a> on how to do that.</p>
