## Notification !

Note! This Is a Horizon Remake Product (By Schmavery's Facebook-Chat-Api, The Author Is Not Responsible!), If There Is Any Error Please Try Using Another Product!

## Support For : 

+ Support English, VietNamese !,
+ All bot if using listenMqtt first.

# Api Cho ChatBot Messenger

Facebook Already Has And For Users To Create Api For Chatbots At Dey => [Here](https://developers.facebook.com/docs/messenger-platform).

### This Api Can Make You Payy Acc Like You Never Have, Please Pay Attention =))

Note ! If You Want To Use This Api Please See The Document At [Here](https://github.com/Schmavery/facebook-chat-api).

## Download 

If You Want To Use It, Download It By:
```bash
npm i fca-horizon-remake
```
or
```bash
npm install fca-horizon-remake
```

It Will Load Into node_modules (Your Lib) - Note Replit Won't Show Anywhere to Find 😪

### Download Latest Version Or Update

If You Want To Use The Latest Version Or Update Then Go To Terminal Or Command Prompt Enter :
```bash
npm install fca-horizon-remake@latest
```
Hoặc
```bash
npm i fca-horizon-remake@latest
```

## If You Want To Test Api 

Benefits For This You Will Not Spend Time Pay Acc And Have Acc 😪
Use it with a Demo Account=> [Facebook Whitehat Accounts](https://www.facebook.com/whitehat/accounts/).

## Using

```javascript
const login = require("fca-horizon-remake"); // get it from the lib 

// log in
login({email: "Gmail Account", password: "Your Facebook Password"}, (err, api) => {

    if(err) return console.error(err); // error case

    // create bots that automatically copy you:
    api.listenMqtt((err, message) => {
        api.sendMessage(message.body, message.threadID);
    });

});
```

As a result, it will copy you as shown below:
<img width="517" alt="screen shot 2016-11-04 at 14 36 00" src="https://cloud.githubusercontent.com/assets/4534692/20023545/f8c24130-a29d-11e6-9ef7-47568bdbc1f2.png">

If You Want Advanced Use Then Use Bot Types Listed Above !

## List

You Can Read Full Api At => [here](DOCS.md).

## Settings For Mirai: 

You Need to Go File Mirai.js,Then Find The Line
```js
    var login = require('tùy bot'); 
    /* Có thể là :
        var login = require('@maihuybao/fca-Unofficial');
        var login = require('fca-xuyen-get');
        var login = require('fca-unofficial-force');
    ...   
    */
```

And Replace It With:

```js
    var login = require('fca-horizon-remake')
```

Then Just Run As Normal  !

## Self-study

If You Want To Research Or Create Your Own Bot Then Go To This Read Its Function And How To Use It => [Link](https://github.com/Schmavery/facebook-chat-api#Unofficial%20Facebook%20Chat%20API)

------------------------------------

### Save Login Information.

To Save You Need 1 Style Apstate (Cookie, etc,..) To Save Or Use Login Code As Above To Login !

And This Mode Is Already Available In Some Vietnamese Bots So You Can Rest In Peace !

__Guide With Appstate__

```js
const fs = require("fs");
const login = require("fca-horizon-remake");

var credentials = {email: "FB_EMAIL", password: "FB_PASSWORD"}; // thông tin tk

login(credentials, (err, api) => {
    if(err) return console.error(err);
    // đăng nhập
    fs.writeFileSync('appstate.json', JSON.stringify(api.getAppState(), null,'\t')); //tạo appstate
});
```

Or Easier (Professional) You Can Use => [c3c-fbstate](https://github.com/c3cbot/c3c-fbstate) To Get Fbstate And Rename It To Apstate Is Also ! (appstate.json)

------------------------------------

## FAQS

FAQS => [Link](https://github.com/Schmavery/facebook-chat-api#FAQS)
