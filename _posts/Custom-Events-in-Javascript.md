Events are actions that users are likely to take when they visit your page. Since every action requires a response, your web page needs to have some way of giving feedback or responding to a user when they perform a pre-defined action.
 
 Without this action and response cycle, your web app would more or less be like a fancy looking billboard that people just come in and glance at. Users cannot actually engage with it.

 Javascript together with modern browser APIs help breathe in life into your application by providing a set of events to which your app can recognize and respond to.
 For example, if you had a button on your web page, a likely event users will take is to click it. So, to instruct your app what to do when a user actually clicks, you may do something like:
 ```
 var btn = document.getElementById('submit-btn');
 btn.onclick = buttonClicked();
 function buttonClicked(){
     console.info("Yo, you clicked me!");
 }
```
Depending on your application, [there's a bunch of other events](https://developer.mozilla.org/en-US/docs/Web/Events) your web page can listen for. This is out of the scope of this article.

Haven done a recap of events in Javascript, let's talk about implementing custom events and use cases.

 ## Custom Events - What are they?
 Custom events simply help you create and define your own event