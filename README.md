<div align="center">

## Changing content on the fly using JavaScript


</div>

### Description

Using JavaScript and DHTML, content on your page can be changed dynamically and on-the-fly. Learn how to in this tutorial! You're learn three different techniques, one for IE5, NS4, and NS6.
 
### More Info
 


<span>             |<span>
---                |---
**Submitted On**   |
**By**             |[David Gardner](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByAuthor/david-gardner.md)
**Level**          |Intermediate
**User Rating**    |3.8 (15 globes from 4 users)
**Compatibility**  |
**Category**       |[Miscellaneous](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByCategory/miscellaneous__2-57.md)
**World**          |[Java](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByWorld/java.md)
**Archive File**   |[](https://github.com/Planet-Source-Code/david-gardner-changing-content-on-the-fly-using-javascript__2-2345/archive/master.zip)





### Source Code

<html>
<head>
<title>Changing content on the fly using DHTML</title>
</head>
<body>
<p><b><font size="4"><u>Changing content on the fly using </u></font></b><b><font size="4"><u>JavaScript/DHTML</u></font></b></p>
<p><font size="3">One of my favorite uses of JavaScript, and I guess more
specifically, DHTML, is to change content on the fly. Using just a few lines of
scripting, I can do away with the slow downloading Java and Flash, and change
text even after the page has loaded.</font></p>
<p><font size="3">I write this tutorial based on the assumption that you have at
least some working knowledge of JavaScript.</font></p>
<p>Changing text requires 3 different techniques, depending on the browser. If you're
like me, you favor Internet Explorer 5, but the point is that there are always
people using other browsers, so we must address them all.</p>
<p>Let me first introduce a simple text which I will base my explanations on
changing text using:</p>
<p><font size="4" face="Courier" color="#008000">&lt;div
ID=&quot;testing&quot;&gt;Planet Source Code&lt;/div&gt;</font></p>
<p>In Internet Explorer 4 or above, the script to change the above text is:</p>
<p><font size="3" face="Courier" color="#008000">document.all.testing.innerHTML=&quot;A
very cool site!&quot;</font></p>
<p>I access the text's ID, which tells the script which text I wish to change.
Then I use the property .innerHTML, which allows me to change this text to
another.</p>
<p>In Netscape 6, the idea to alter a text is very similar, except in the
precise syntax:</p>
<p><font size="3" face="Courier" color="#008000">document.getElementById(&quot;testing&quot;).innerHTML=&quot;A
very cool site!&quot;</font></p>
<p>Interesting to note is that Internet Explorer 5 also supports this method of
changing text. If you don't care about IE4, this one line is sufficient to cover
both IE5 and NS6.</p>
<p>Finally, we have the dreaded Netscape 4, which surprising is still more
popular than NS6. To change text in this browser, I must actually embed the text
using a different set of tags (from the DIV). The tags required is:</p>
<p><font size="3" face="Courier" color="#008000">&lt;ilayer
name=&quot;testing&quot;&gt;&lt;layer name=&quot;testing2&quot;&gt;Planet Soure
Code&lt;/layer&gt;&lt;/ilayer&gt;</font></p>
<p>Once the proper tags are setup, I can change its text in Netscape 4 using:</p>
<p><font size="3" face="Courier" color="#008000">document.</font><font size="3" face="Courier" color="#008000">testing.document.test2.document.write(&quot;A
very cool site!&quot;)<br>
</font><font size="3" face="Courier" color="#008000">document.</font><font size="3" face="Courier" color="#008000">testing.document.test2.document.close()</font></p>
<p>Awk! Yes, it's quite messy, but that's the only route to NS4's heart!</p>
<p>Many interesting and useful applications can be created by dynamically
altering text. I can create a message scroller that changes messages every few
seconds, a text that changes when I move my mouse over it, or even an image
slide show with a corresponding description beneath it. </p>
<p>If you're looking for working examples of changing text on the fly, a good
place to start is <a href="http://www.dynamicdrive.com/" target="new">Dynamic Drive</a>.</p>
<p>Well, that's it for now. <a href="mailto:davidgardner7@yahoo.com">Email me</a>
if you have any suggestions for new tutorials I can contribute.</p>
</body>
</html>

