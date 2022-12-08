## Port 80

###### Might be a rabit hole

![[Pasted image 20221128101644.png]]

#### Dir Enumeraiton

- common.txt (html, txt):
``` 
301        2l       10w      150c http://10.10.10.213/Images
200      211l      718w     9386c http://10.10.10.213/About.html
200      347l     1094w    14879c http://10.10.10.213/Index.html
200      147l      412w     5528c http://10.10.10.213/News.html
200      155l      468w     6326c http://10.10.10.213/Support.html
200      211l      718w     9386c http://10.10.10.213/about.html
200      243l      870w    10592c http://10.10.10.213/Services.html
200      274l      958w    12146c http://10.10.10.213/clients.html
301        2l       10w      147c http://10.10.10.213/css
301        2l       10w      149c http://10.10.10.213/fonts
301        2l       10w      150c http://10.10.10.213/images
200      347l     1094w    14879c http://10.10.10.213/index.html
301        2l       10w      146c http://10.10.10.213/js
200      147l      412w     5528c http://10.10.10.213/news.html
301        2l       10w      153c http://10.10.10.213/fonts/css
301        2l       10w      155c http://10.10.10.213/fonts/fonts
200      243l      870w    10592c http://10.10.10.213/services.html
200      155l      468w     6326c http://10.10.10.213/support.html
```
	Does not seem like there is something intersting. Could be a rabbit hole more enumeratin is needed maybe.


- directory-list-2.3-medium.txt (html, txt):
```
301        2l       10w      150c http://10.10.10.213/images
200      155l      468w     6326c http://10.10.10.213/support.html
200      147l      412w     5528c http://10.10.10.213/news.html
200      243l      870w    10592c http://10.10.10.213/services.html
200      211l      718w     9386c http://10.10.10.213/about.html
200      347l     1094w    14879c http://10.10.10.213/index.html
301        2l       10w      150c http://10.10.10.213/Images
200      147l      412w     5528c http://10.10.10.213/News.html
301        2l       10w      147c http://10.10.10.213/css
200      211l      718w     9386c http://10.10.10.213/About.html
200      347l     1094w    14879c http://10.10.10.213/Index.html
200      274l      958w    12146c http://10.10.10.213/clients.html
301        2l       10w      146c http://10.10.10.213/js
200      155l      468w     6326c http://10.10.10.213/Support.html
200      243l      870w    10592c http://10.10.10.213/Services.html
200      147l      412w     5528c http://10.10.10.213/NEWS.html
301        2l       10w      149c http://10.10.10.213/fonts
301        2l       10w      153c http://10.10.10.213/fonts/css
301        2l       10w      150c http://10.10.10.213/IMAGES
200      347l     1094w    14879c http://10.10.10.213/INDEX.html
301        2l       10w      155c http://10.10.10.213/fonts/fonts
301        2l       10w      149c http://10.10.10.213/Fonts
301        2l       10w      153c http://10.10.10.213/Fonts/css
200      274l      958w    12146c http://10.10.10.213/Clients.html
301        2l       10w      155c http://10.10.10.213/Fonts/fonts
301        2l       10w      155c http://10.10.10.213/fonts/Fonts
301        2l       10w      147c http://10.10.10.213/CSS
301        2l       10w      146c http://10.10.10.213/JS
301        2l       10w      155c http://10.10.10.213/Fonts/Fonts
301        2l       10w      153c http://10.10.10.213/fonts/CSS
301        2l       10w      153c http://10.10.10.213/Fonts/CSS
200      155l      468w     6326c http://10.10.10.213/SUPPORT.html
200      243l      870w    10592c http://10.10.10.213/SERVICES.html
200      211l      718w     9386c http://10.10.10.213/ABOUT.html
```

