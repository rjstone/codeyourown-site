---
title: "What to Do Next: Advanced"
subtitle: "Learning both front and back end development plus some devops like command line interfaces and virtual servers."
layout: default
prevpage: intermediate.html
prevtitle: "What to Do Next: Intermediate"
nextpage: dm-frameworks.html
nexttitle: "Native Desktop and Mobile Apps"
---

<h2 class="anchor" id="advanced">Advanced Difficulty Level</h2>

<p><strong>This section is very advanced, so be prepared to learn a lot of stuff if you want to do any of this.</strong></p>

<p>Before continuing, you should learn how to use <strong>command line interfaces</strong> (CLIs), also called shells. Which one you use will depend on which operating systems you are using. Web servers most frequently use Linux, so you will need to learn that no matter what. Fortunately for Mac users, OS X uses essentially the same command line interface as Linux with a few minor differences. Windows is a little different since PowerShell is now the preferred CLI, but you can install <span class="code">bash</span> or another Unix/Linux style shell in Windows if you want.</p>

<p>Here are some resources that will help:</p>
<ul>
    <li><a href="https://www.codecademy.com/learn/learn-the-command-line">Learn to use the shell command line</a> on CodeAcademy. This tutorial is interactive and will teach you to use Unix/Linux style command line shells, such as 'bash', even if you know nothing yet.</li>
    <li>If you installed <a href="https://git-for-windows.github.io/">Git for Windows</a>, you already have a Linux-like shell called "Git Bash" that you can launch from the start menu. Just type "git bash" into the search box of the start menu. You don't have to be using Git to use the 'bash' shell. You can do anything with it, and it comes already configured for running git shell commands too. It recognizes the same sort of commands as 'bash' on Linux, but it doesn't allow you to run Linux software.</li>
    <li><a href="https://blog.udemy.com/powershell-tutorial/">A Beginner’s Introduction to Windows PowerShell</a> for those using Windows.</li>
    <li>If you have Windows 10 and have installed the Anniversary Update, you can actualy <a href="http://www.howtogeek.com/249966/how-to-install-and-use-the-linux-bash-shell-on-windows-10/">install Microsoft's Linux command line environment on Windows</a>. This will not only give you a Linux shell, but you can also run actual Linux command line software. It is a Linux emulator, but it doesn't use a virtual machine and doesn't come with support for graphical applications unless you use <code>apt-get</code> to install it.</li>
</ul>


<h3>Install Node.js and a Database Server on Your Desktop or Laptop</h3>

<p>You can install <a href="https://nodejs.org/">Node.js</a> on your Windows, Mac, or Linux computer, run applications from the command line, and use your browser to view them. This is useful for developing and testing your code offline until you're ready to deploy (upload) it.</p>

<p>It is also possible to install Apache, PHP, python, ruby, and other languages with web application frameworks on your local computer for purposes of learning and testing.</p>

<p>If you haven't already then you may want to install a database such as MySQL or PostgreSQL on your local computer. See above for links to some free database software.</p>


<h3>Get a Free Containerized Cloud Hosting Account at Heroku</h3>

<p>Now that you know the CLI and know some things about both server-side scripting and databases, you might want to try out containerized <a href="https://en.wikipedia.org/wiki/Cloud_computing#Service_models">cloud computing</a> services. There is one that allows you to use Node.js and PostgreSQL for free called <a href="http://www.heroku.com/">Heroku</a> and what they give you for free is pretty impressive.</p>

<p>You will need to know how to use the CLI on your local computer because it's pretty much impossible to use Heroku without the CLI, but they have excellent step-by-step tutorials on how to deploy and manage applications on their service. You will also need to <a href="https://www.codecademy.com/learn/learn-git">learn to use Git from the command line</a>.</p>

<p>Heroku is a <strong>PaaS</strong> (Platform as a Service) type service which doesn't offer you true virtual machines like an <strong>IaaS</strong> (Infrastructure as a Service) type service. So don't expect to be able to upload your own virtual machine images.</p>


<h3>Experiment With Local Virtual Servers</h3>

<p>You can simulate an IaaS cloud hosting server on your local computer using free virtual machine software. This is helpful because it gets you used to using a virtual server the same way you would using a virtual server hosting service.</p>

<p>Download <a href="https://www.virtualbox.org/wiki/Downloads">VirtualBox</a> (Virtual Machine hypervisor) and run a <a href="https://bitnami.com/stack/mean/virtual-machine">virtual machine image</a> installed with <a href="http://meanjs.org/">MEAN.JS</a> for example. There are a lot of other <a href="https://bitnami.com/stacks">virtual machine images</a> that you can experiment with including LAMP images.</p>

<p>Once you have a virtual machine running, you will want to treat it like it's running on an unknown rack mount server in some unknown location where you will never see it, because this is the situation with actual virtual machine hosting services. In other words, you want to treat your VM like a "headless" machine (one with no monitor or keyboard).</p>

<p>To access and control your VM, you will <a href="http://www.makeuseof.com/tag/beginners-guide-setting-ssh-linux-testing-setup/">need to use ssh</a> which is a way to get a command line on remote computers and upload files. Hopefully your VM image has git installed on it already because the best practice for uploading changes to a site is to use git.</p>


<h3>Virtual Web Server Hosting</h3>

<p>These days most people are actually happy with CaaS (Container as a Service) and PaaS type services because they do almost everything one could want but are less trouble to deal with than full virtual machines. But, once you're familiar with virtual machine servers, you might want to create your own web site based on one and possibly run other types of servers on it such as game servers.</p>

<p><strong>This is very advanced, so you will need to learn a lot about system administration and web devlopment before you can make good use of an environment like this. Get comfortable with running a virtual server on your own computer first.</strong> Here are some recommendations.</p>

<p>A <a href="https://www.digitalocean.com/products/one-click-apps/lamp/">virtual server hosting account</a> running a <a href="https://en.wikipedia.org/wiki/LAMP_(software_bundle)">LAMP</a> (Linux, Apache, MySQL, PHP) installation will do pretty much anything that one could want, but it isn't much different than the free LAMP-based web hosting accounts mentioned above. The main advantage is that you will have command line access and can do whatever you want with the virtual server.</p>

<p>A <a href="https://www.digitalocean.com/products/one-click-apps/mean/">virtual server hosting account</a> running <a href="http://meanjs.org/">MEAN.JS</a> provides an environment with <a href="http://docs.mongodb.org/manual/">MongoDB</a> and <a href="http://expressjs.com/">Express.js</a> plus <a href="https://nodejs.org/">Node.JS</a> for server-side scripting. This is a little more sophisticated than the previous option but it entirely uses JavaScript so learning PHP isn't necessary. Learning the JavaScript frameworks (Express.js, Node.js, and Angular.js) is necessary though, and you can learn more about some of those on <a href="https://www.codecademy.com/learn">CodeAcademy</a>. You can experiment with Node.js and Express.js at <a href="https://hyperdev.com/">HyperDev</a>.</p>