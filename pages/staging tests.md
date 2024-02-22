---
title: staging tests
permalink: /permalink/
variant: tiptap
description: ""
---
<pre><code>Allowed script 

&lt;script src="//www.instagram.com/embed.js" async="true"&gt;&lt;/script&gt;

Disallowed in csp

&lt;script src="//www.evil.com/embed.js" async="true"&gt;&lt;/script&gt;

Allowed in csp but should also be controlled

&lt;script src="//www.blah.cloudfront.net/embed.js" async="true"&gt;&lt;/script&gt;


Attributes not allowed 

&lt;svg&gt;&lt;script src="/jquery/jquery.min.js" href="THISFILEWILLBELOADED"&gt;&lt;/script&gt;&lt;/svg&gt;
&lt;svg&gt;&lt;script src="/jquery/jquery.min.js" xlink:href="THISFILEWILLBELOADED"&gt;&lt;/script&gt;&lt;/svg&gt;
</code></pre>
<p></p>