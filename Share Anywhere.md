# Share Anywhere

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