Author: Andre k Lorenci
Contact: avlorenci@gmail.com

I will create this repository because I don't know if this is a knowed vulnerability so just to make sure, that's the poc.

Hello, this vulnerability consists in a function called showAlert() in the administration panel of bludit,that when accessed in DOM, allows users define the text to be popped up in the message box. But this function dont have any sanatization and the user can inject any javascript code or even HTML in the page

![XSS in admin page](https://github.com/gh0st56/bludit-DOM-xss/blob/master/xss-bludit.jpg)

the payload used was:
showAlert("<script>alert(1)</script>");

The versions that i tested was the Bludit 3.x. I'll check the old ones for a more in deep report

Thank you.
