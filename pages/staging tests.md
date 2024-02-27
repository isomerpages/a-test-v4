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
&lt;svg&gt;&lt;script src="/jquery/jquery.min.js" xlink:href="THISFILEWILLBELOADED"&gt;&lt;/script&gt;&lt;/svg&gt;</code></pre>
<p>Allowed script</p>
<p>&lt;script src="//<a href="http://www.instagram.com/embed.js" rel="noopener noreferrer nofollow" target="_blank">www.instagram.com/embed.js</a>"
async="true"&gt;&lt;/script&gt;</p>
<p>Disallowed in csp</p>
<p>&lt;script src="//<a href="http://www.evil.com/embed.js" rel="noopener noreferrer nofollow" target="_blank">www.evil.com/embed.js</a>" async="true"&gt;&lt;/script&gt;</p>
<p>Allowed in csp but should also be controlled</p>
<p>&lt;script src="//<a href="http://www.blah.cloudfront.net/embed.js" rel="noopener noreferrer nofollow" target="_blank">www.blah.cloudfront.net/embed.js</a>"
async="true"&gt;&lt;/script&gt;</p>
<p>Attributes not allowed</p>
<p>&lt;svg&gt;&lt;script src="/jquery/jquery.min.js" href="THISFILEWILLBELOADED"&gt;&lt;/script&gt;&lt;/svg&gt;</p>
<p>&lt;svg&gt;&lt;script src="/jquery/jquery.min.js" xlink:href="THISFILEWILLBELOADED"&gt;&lt;/script&gt;&lt;/svg&gt;</p>
<p></p>