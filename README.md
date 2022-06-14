# GoBadian

**Main Link - `javascript:(function(){document.body.appendChild(document.createElement('script')).src='https://testingherokuapp.github.io/GoBadian/GoBadian.min.js'})()`**

Contact - *[j4jeffrey2424@outlook.com](mailto:j4jeffrey2424@outlook.com)* | *M4MASON#0697*

**Join [TitaniumNetwork](https://discord.gg/unblock)!**

A favelet which can be used to unblock websites that are blocked with GoGuardian.
Drag this to your Bookmarks bar, click on it and it will prompt you to enter a URL:
`javascript:(function(){document.body.appendChild(document.createElement('script')).src='https://testingherokuapp.github.io/GoBadian/GoBadian.min.js%27%7D)()`

## IMPORTANT
For first time set up remove ALL text already there and replace it with https://9e2d20ff-aa91-4ab5-b621-79905727ede6.id.repl.co/. If its blocked then hit the back arrow untill its unblocked (bug) then type in google.com into the search bar and hit enter. Now it will work, you can refresh the page and hit enter without removing the text now and it will work properly.

## NOTE!
Lyft requires loading quickly. I do NOT recommend you host this on a server, as it is most likely to fail for taking too long to request for the JS. Instead, run the favelet completely locally: `javascript:window.addEventListener('beforeunload', function (e) {e.preventDefault();return "h";});`

### What is this?
GoBadian is a tool designed to unblock websites, specifically tailored to GoGuardian.

### Who is developing it?
Mason now. The original creator is luphoria but his code is outdated so I improved it and made it working in 2022

### How do I install it?
GoGaurdian is a favelet, or a bookmarklet. To use it, all you have to do is:
 - host GoBadian.js on your own webpage (e.g. a github pages website)
 - drag this "favelet" to your Bookmarks bar: `javascript:s=document.body.appendChild(document.createElement ('script'));s.id='fs';s.language='javascript';void (s.src='//path/to/GoBadian.js');`
 - *Many websites using the default setting do not work. This can be resolved by visiting that website FIRST, stopping the page from fully loading, and then loading GoBadian. If the page STILL doesn't work, contact me and ill help you.
 
### How do I use it?
Simply click on the favelet and it will load a menu. It should be fairly self-explanatory.
 - The proxy used is called "Corrosion" by sexyduceduce. Slight modifications have been made so that it can be run within GoBadian. It is planned to have more proxies in the future.

### So, how TF does it work??
GoGuardian blocks pages by checking your URL, and if the URL is blocked, redirecting your page. This works fine, however there are two major flaws with this system:
 - GoGuardian has to actually load to block the page (and BEFORE any code from the original page can be executed)
 - This does **not** account for elements like `iframe`, in which a page is embedded within a totally separate page -- with a **different URL**.
By combining onbeforeunload, iframes, and adding a proxy as well, you can unblock essentially any website,

### What's the "FakeWin" stuff?
Ignore for now -- heavy in testing stuff. But feel free to check out what it's based on -- [luphoria/FakeWindow](https://github.com/luphoria/FakeWindow)

## End Goal
Any and all websites unblockable and functional.
*Any website will work via Lyft, however its speed-spam-clicky nature makes this less than preferable.*
## CREDITS
  - Code: luphoria and improved by Mason
  - "Corrosion" web proxy: @Carcal-js
