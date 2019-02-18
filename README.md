<h1>Building a Realtime Chat App with Laravel 5.4 and VueJS</h1>
</header>
<section class="entry-content">
<p>With the announcement of <a href="https://laravel.com/docs/master/dusk">Laravel Dusk</a>, a browser automation and testing API tool, I noticed a cool chunk of demo code. It represents a realtime app that features user interacting using WebSockets:</p>
<p><script src="https://gist.github.com/jplhomer/a4d08754e7e1a9259c5d71c038a4d2da.js"></script></p>
<p>This inspired me to build an app for which I could use that same exact snippet of code. It ended up involving quite a few steps, but Laravel made it easy!</p>
<p><strong><a href="https://github.com/jplhomer/laravel-realtime-chat-demo">See the code for this tutorial on Github</a></strong></p>
<p><strong>Note</strong>: I&#8217;ve since updated the master branch of the code on Github which fixed some breaking changes to how Laravel Mix is compiled. They are <em>not</em> updated in the individual steps below.</p>
<h2 id="setup">Step 1: Setup</h2>
<p><iframe width="500" height="281" src="https://www.youtube.com/embed/rL-dJcxC8X8?feature=oembed" frameborder="0" allowfullscreen></iframe></p>
<p>In this video, I get the <code>dev</code> version of <a href="https://laravel.com/">Laravel</a> installed, get the new <a href="https://laravel.com/docs/master/mix">Laravel Mix</a> up and running, and render and example <a href="https://vuejs.org/">Vue</a> component.</p>
<ul>
<li><a href="https://github.com/jplhomer/laravel-realtime-chat-demo/tree/step1">Code for Step 1</a></li>
</ul>
<h2 id="vue">Step 2: Vue Components</h2>
<p><iframe width="500" height="281" src="https://www.youtube.com/embed/pTVCW5k4piU?feature=oembed" frameborder="0" allowfullscreen></iframe></p>
<p>Now I can start developing several Vue Components to create an interactive chat application. None of the data is persisted to the server yet, but it looks real!</p>
<ul>
<li><a href="https://github.com/jplhomer/laravel-realtime-chat-demo/tree/step2">Code for Step 2</a></li>
<li><a href="https://vuejs.org/v2/guide/components.html">VueJS component docs</a></li>
</ul>
<h2 id="backend">Step 3: Laravel Backend</h2>
<p><iframe width="500" height="281" src="https://www.youtube.com/embed/8aTfMHg3V1Q?feature=oembed" frameborder="0" allowfullscreen></iframe></p>
<p>Now I am POSTing chat messages to the server and start loading messages from the server. It&#8217;s basic Laravel models and routes in this video.</p>
<ul>
<li><a href="https://github.com/jplhomer/laravel-realtime-chat-demo/tree/step3">Code for Step 3</a></li>
</ul>
<h2 id="echo">Step 4: Laravel Echo</h2>
<p><iframe width="500" height="281" src="https://www.youtube.com/embed/iiBcOKYxd0Q?feature=oembed" frameborder="0" allowfullscreen></iframe></p>
<p>I have a functional chat app connected to the server, but I have to refresh to see new messages from other people. This step involves setting up Event Broadcasting within Laravel and implementing Laravel Echo on the front end using Pusher.</p>
<ul>
<li><a href="https://github.com/jplhomer/laravel-realtime-chat-demo/tree/step4">Code for Step 4</a></li>
<li><a href="https://laravel.com/docs/master/broadcasting">Event Broadcasting docs</a></li>
<li><a href="https://pusher.com/">Pusher</a></li>
</ul>
<h2 id="dusk">Step 5: Laravel Dusk</h2>
<p><iframe width="500" height="281" src="https://www.youtube.com/embed/wrF3cw0y95s?feature=oembed" frameborder="0" allowfullscreen></iframe></p>
<p>I&#8217;m finally to the point where I&#8217;m ready to test my realtime chat application. I install Laravel Dusk, write a couple example tests, and talk about the benefits of this sort of testing environment.</p>
<ul>
<li><a href="https://github.com/jplhomer/laravel-realtime-chat-demo/">Final Code</a></li>
<li><a href="https://laravel.com/docs/master/dusk">Laravel Dusk docs</a></li>
</ul>
<p>That&#8217;s all that I have! Let me know if you have had similar experiences with Laravel and what sort of things you&#8217;ve done with Laravel Dusk.</p>
<p><a class="twitter-follow-button" href="https://twitter.com/jplhomer"><br />
Follow @jplhomer</a></p>