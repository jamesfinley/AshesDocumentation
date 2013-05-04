# Share Anywhere

Share Anywhere allows you to add inter-app communication to Ashes. If an app, take Tumblr, supports openURL, we can easily create a URL to send info from Ashes to Tumblr. ``tumblr://x-callback-url/link?title=[[[title]]]&url=[[[url]]]&description=[[[textselection]]]&x-success=[[[callback]]]&x-cancel=[[[callback]]]`` will send you to Tumblr to create a new Link post with the item title, url, and current text selection, and when done will send you back to Ashes. See the list of variables below and learn how to add a Share Anywhere link to Ashes.

## Variables

**Text selection grabs the current text selection from the article or browser. If no selection is available, use item title.**  
``[[[textselection]]]``

**Title grabs either the item title or browser title**  
``[[[title]]]``

**Feed title isn't available in the Browser, clearly.**  
``[[[feedtitle]]]``

**If selection, “``[[[textselection]]]``” via ``[[[feedtitle]]]`` ``[[[url]]]``**  
**If no selection, ``[[[title]]] [[[url]]]``**  
``[[[post]]]``

**Current item or page (in browser) URL**  
``[[[url]]]``

**If the app supports x-callback, uses this to send back to Ashes.**  
``[[[callback]]]``

## Making a URL
**Each Share Anywhere link needs a title and the URL. The title identifies it in the share menu. Each of these need to be URL encoded.**  
**The format is:**  
``ashes://addOpenURL?title=&url=``

## Examples

**Share by Mail**  
ashes://addOpenURL?title=Share%20by%20Mail&url=mailto%3A%3Fsubject%3D%5B%5B%5Btitle%5D%5D%5D%26body%3D%5B%5B%5Bpost%5D%5D%5D

**Share by Sparrow Mail**  
ashes://addOpenURL?title=Share%20by%20Sparrow%20Mail&url=sparrow%3A%2F%2F%3Fsubject%3D%5B%5B%5Btitle%5D%5D%5D%26body%3D%5B%5B%5Bpost%5D%5D%5D

**Share with Pushpin**  
ashes://addOpenURL?title=Share%20with%20Pushpin&url=pushpin%3A%2F%2Fx-callback-url%2Fadd%3Furl%3D%5B%5B%5Burl%5D%5D%5D%26title%3D%5B%5B%5Btitle%5D%5D%5D

**Share Link with Tumblr**  
ashes://addOpenURL?title=Share%20Link%20with%20Tumblr&url=tumblr%3A%2F%2Fx-callback-url%2Flink%3Ftitle%3D%5B%5B%5Btitle%5D%5D%5D%26url%3D%5B%5B%5Burl%5D%5D%5D%26description%3D%5B%5B%5Btextselection%5D%5D%5D%26x-success%3D%5B%5B%5Bcallback%5D%5D%5D%26x-cancel%3D%5B%5B%5Bcallback%5D%5D%5D

**Share Quote with Tumblr**  
ashes://addOpenURL?title=Share%20Quote%20with%20Tumblr&url=tumblr%3A%2F%2Fx-callback-url%2Fquote%3Fquote%3D%5B%5B%5Btextselection%5D%5D%5D%26source%3D%5B%5B%5Btitle%5D%5D%5D%2520-%2520%5B%5B%5Burl%5D%5D%5D