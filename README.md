# Bookmarklets

Bookmarklets are bookmarks that have javascript code in them. In layman terms, they have scripts in them.

## How to use

This is an example of a bookmarklet. Copy and paste this into a bookmark.

```javascript
javascript:alert("This is a bookmarklet");
```
Below are more useful bookmarklets. Please check them out!
## Bookmarklet List
This one isn't that useful. It just gives a prompt for a url and opens that url. The url has to have "https://" at the beginning.
```javascript
javascript:var url1= prompt("Please enter a website address", "https://", "hello"); window.open(url1);
```
If for some random reason you want to edit a page, this bookmarklet lets you literally type anywhere on a website.
```javascript
javascript:if(confirm("Press ok to edit. Press cancel to stop editing.") == true){document.body.contentEditable = true; void 0;}else{document.body.contentEditable = 'false'; document.designMode='off'; void 0}
```
## Contributing
Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

Please make sure to update tests as appropriate.

## Other links
Please check out [Project Pog](https://sites.google.com/view/projectpog/), a game website. 
