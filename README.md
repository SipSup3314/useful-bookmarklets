# Bookmarklets

Bookmarklets are bookmarks that have javascript code in them. In layman terms, they have scripts in them.

## How to use

This is an example of a bookmarklet. Copy and paste this into a bookmark.

```javascript
javascript:alert("This is a bookmarklet");
```
Below are more useful bookmarklets. Please check them out!
## Bookmarklet List
### Google Search
This one isn't that useful. It just gives a prompt for a google search and doesn't have autocomplete.
```javascript
javascript:var url1= prompt("Search Google without getting distracted by autocomplete!"); if(url1){window.open("https://www.google.com/search?q=" + url1);} else {void(0);}
```
### Page Editor
If for some random reason you want to edit a page, this bookmarklet lets you literally type anywhere on a website.
```javascript
javascript:if(confirm("Press ok to edit. Press cancel to stop editing.") == true){document.body.contentEditable = true; void 0;}else{document.body.contentEditable = 'false'; document.designMode='off'; void 0}
```
### Crash Script
This bookmarklet crashes your computer. Who would need this?
```javascript
javascript:while(true){window.open("https://youtube.com", "", "width=2000,height=1000");}
```
### Script Prompt
This makes a popup appear asking you for javascript, then it executes that javascript.
```javascript
javascript:function JSexe(){ if(valJS!='null' && valJS!='undefined')strJS=valJS; strJS=prompt('Your Javascript code or variable:',strJS); if(strJS!=null && strJS!='' && strJS!='undefined'){  setTimeout('valJS=\'\'+eval(strJS);JSexe()',10); } else{valJS='';strJS='';}}valJS='';strJS='';JSexe();
```
### Mouse Pos
This one makes it so your mouse x and y positions appear in the url.
```javascript
javascript:document.addEventListener('mousemove',function(e)%7Blocation.hash=(window.scrollX+e.clientX)+','+(window.scrollY+e.clientY)%7D,true);
```
## Contributing
Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

Please make sure to update tests as appropriate.

## Other links
Please check out [Project Pog](https://sites.google.com/view/projectpog/), a game website. 
