# EmailScrapperBotTest

### Overview

Simple scrapper bot that once run in the console on a webpage scans for all emails on the page. It then scans for links that are on the page that link to other pages on the same domain as current page.

One it has gathered those links it fires off an XMLHttp Request asynchronously for each one grabing just the DOM HTML representation. Upon returning it scans those documents for email addresses. Lastly once all requests are back in we eliminate all non-unique email addresses and output found email addresses to console.

### Syntax Style

I decided to write this as close to functional ES6 as possible. Favoring working with returned arrays over large number of holder variables.
I tend to think in terms of Funtional Programming with lambda expressions '=>' to derive meaning over being overly verbose.