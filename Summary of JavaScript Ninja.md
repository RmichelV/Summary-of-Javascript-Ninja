
# Javascript is everywhere

<div style="text-align: justify">

***This chapter cover***

* The core language features of Javascript
* The core items of Javascript engine
* Three best practices in JavaScript development 

Let´s start this summary talking about Bob who is a software development, who graduated in 2000's after learn how create desktop application. As the web pages had just hit stride he learned PHP so he could create dynamic web pages sprinkled with JavaScript to achieve complex functionalities like form validations. When the smartphones arrived, they opened a new market and bob didnâ€™t want keep back and learned Objective-C and Java to develop mobile apps that run on IOS and Android. Now lets talk about Ann who graduated with a degree in software development. She made websites based on the modern Model-View-Controller, also made mobile applications that running on IOS and Android, she got to make desktop applications that runs on Windows, Linux and OS X, she has started to building a server less version of that applications entirely based in the cloud. Everything written in JavaScript. That was extraordinary because what took Bob 10 years and 5 languages to do, Ann has achieved in 2 years and in just one language. What started as a humble 10-day project back in 1995 is now one of the most widely used programming languages in the world, now JavaScript is getting long overdue upgrades to be more suitable for modern application development.

**1.1 Understanding the JavaScript language**

Using a vast number of elements in the languages is not enough to take beyond fundamental levels because JavaScript often using a C-like syntax because it  has a resemblance to others C-like languages such C# and Java. People often think if they know C# or Java they know JavaScript but the reality is other and they check it after writing JavaScript as if it were Java and the results are other that they expected. 

These differences include the following:

* *Functions are fist class objects* - Function can coexist and be treated like any other JavaScript objet. They can be created through literals, referenced by variables, passed around as function arguments an event return as function return values.

* *Function clouser* - Function is a closure when it actively maintains the external variables used in its body.

* *Scopes* - JavaScript didn’t have block levels variables as other C-like languages and we had to rely on global variables and function level variables. 

* *Prototype-base object orientation* - JavaScript instead use class-based object orientation like C#, Java and Ruby, uses prototypes. Many developers that come from class-based languages such Java try to use Java using the syntax of JavaScript and they have  a big impression because the results are differ than they expected. 

JavaScript consist of a close relationship between objects and prototypes and prototypes, and functions and closures, understanding those concepts you will have a strong foundation for any type of application development, regardless of whether your JavaScript code will be executed in a desktop application, web page, mobile app or on the server. 

Also exist other features of JavaScript can help you to write more elegant and efficient code in particular we will focus on the following: 

*Generators* - are function that can generate multiple values on a per-request and can suspend their execution between request. 

*Promises* - give us better control over asynchronous code 

*Proxies* -  allow us to control access to certain objects 

*Advanced array methods* - make array-handling code much more elegant 

*Maps* - we can use to create dictionary collections and sets which allow us to deal with collections of unique items. 

*Regular expression* - let us simplify what would otherwise be complicated pieces of code 

*Modules* - we can use to break code into smaller, relatively self-contained pieces that make projects more manageable 

Having a deep understanding of the fundaments and learning how to use the advanced language features to their best advantages can elevate your code to higher levels 

**1.1.1 How will JavaScript evolve**

The ECSMASccript committee in charge of standardizing the language has just finished the ES7/2016 version, a small upgrade to JavaScript compared with ES6, because the committee's goal going forward is to focus on smaller 

Yearly exist updates for the languages but it doesn’t mean that developers will have access to those new features that have been released so we keep waiting for new JavaScript engines that have the new features. Unfortunately there’s always a chances that you’ll run into features that you want to use but that are yet to be supported. 

**1.1.2 Transpiliers give us access to tomorrow’s JavaScript today** 

With the rapid release cycles of browsers we don’t have to wait long for a JavaScript features to be supported but the user of our web application may still using older browsers? One answer could be use transpilers *(transformation + compiling)* are tools that take the cutting edge of JavaScript code and transform it into equivalent (or similar) code that works properly in most current browsers and one of the most popular in transpilier is Traceur. 

**1.2 Understanding the browser**

These days, JavaScript applications can be executed in many environments, but the environments from which all other environment have taken ideas, and the environment on which we’ll focus us the browser. The browser provides various concepts and APIs to thoroughly explore see figure 1.1 

![figure 1.1](images/figure1.jpg)

##### **Figure 1.1 Client-side web application rely on the infraestructure provided by the browser. We'll particularly focus on the DOM, events, tumers, and browser APIs**.

We’ll concentrate on the following:

*The Document Object Model (DOM)* – The DOM is a structured representation of the UI of a client-side web application that is built from the HTML code of a web application to develop great applications you need to not only have a deep understanding of the core JavaScript mechanics. 

*Events* –  Many JavaScript application are event-driven applications, it means the most code executed is in response of a particular event. Examples of events include network events, timers and user-generate events such as clicks, mouse moves, keyboard presses and so on. 

*Browser API* – The browsers offers an API that allow us to access information about devices, store data locally or communicate with remote servers  

The browsers has improved but they still have some bugs, missing APIs and some browsers-specific quirks that we nee to deal with. We need to develop strategies to deal with those issues and becoming familiar with their differences and quirks. 

When we write browser application or JavaScript libraries to be used in them we need choose admit them because the reality is that no all the browsers admit all the libraries or applications. 

**1.3 Using current best practices**

Mastery of the JavaScript language and a strong understanding of coding issues are important parts of becoming an expert web application developer. You need to exhibit the traits that scores of previous developers have proven. Thess traits are known as *best practices* they include such elements as

* Debbugging skills
* Testing
* Performance analysis

Those are important to adhere to theses practices when coding.

**1.3.1 Debugging**

Debugging JavaScript used to mean using alert to verify the value of variables, Fortunately the ability to debug JavaScript code has improve a lot. Because similar tools like Firebug have been developed for the major browsers:

* *Firebug* – The popular developer extension for Firefox that got the ball rolling.
* *Chrome DevTools* – Developed by the Chrome team and used in Chrome and Opera.
* *Firefox Developer* Tools – A tool included in Firefox, built by the Firefox team
* *F12 developer tools* – Included in Internet Explorer and Microsoft Edge
* *Webkit Inspector* – Used by Safari

Every major browsers offers us developer tools to debug  our web applications. All of theses tools are based on similar ideas, they offer similar functionality, exploring the DOM, debugging JavaScript, editing CSS styles, tracking network events and any of them will do a fine job 

**1.3.2 Testing**

 Throughout this book, we’ll apply testing techniques to ensure that the examples operates as intended and serve as examples of how to test code in general. The primary tool we’ll use for testing is an *assert* function, who purpose is to assert that a premise is true or false. And we can prove whether the code is behaving as expected. The general form of this function is as follows:

```
assert(condition, message); 
```

The first parameter is a condition that should be true, and the second is a message that will be displayed if it’s not. Consider this for example:
```
assert(a===1, “Disaster! A is not 1!”) 
```
If the value of variable *a* isn't equal to 1, the assertion fails, and the somewhat overly dramatic message is dsplayed. 

>**Note** The assert function isn't a standard feature of the language, so we'll implement if ourselves in appendix B.

**1.3.3 Performance analysis**

JavaScript engines have made astounding strides in the performance of JavaScript, but that’s no excuse writing sloppy and inefficient code. We’ll use code such as the following later int his book to collect performance information: 

```JavaScript 
console.time(“My operation”); Starts the timer

for(var n = 0; n < maxCount: n++){
/*perform the operation to be measured*/
}

console.timeEnd(“My operation”);
``` 
we bracket the execution of the code to be measured with two calls to the time and time time end methods of the built-in console object.  

Before the operation begins executing, the call to *console.time* starts a timer wiith a name (in this case, My operation), Then we run the code in the *for* loop a certain number of times (in this case, *maxCount* times). Because a single operation of the code happens much to quickly to measure reliably, we need to perform the code many times to get a measurable value. Frequently, this count can be in the tens of thousands or even millions, depending on the nature of the code being measured. A little trial an error lets us choose a reasonable value. When the operation  ends we call the *console.timeEnd* with the same name. The causes the browser to output the time that elapsed since the timer was started. 

**1.4 Boosting skill transferability**

Each browser had its own way to interpreted the scripts and UI styles making that many developers grind their teeth for the frustration but it ends when arrive HTML CSS DOM and JavaScript all being standardized and the developers focus turning toward effective cross-browser JavaScript application. Treat the websites like applications generated many ideas, tools and techniques crossing over from desktop applications to websites applications web development have also permeated other application domains. Have the knowledge about the fundamentals of JavaScript principles and the core of APIs, it makes you a more versatile developer. By using the browser and Node.JS you can developer any type of application imaginable: 

* *Desktop applications* , by using of NW.JS or Electron we can build a desktop Uis with standard HTML, CSS and JavaScript with additional support that makes it possible interact with the file system.

* *Mobile apps with frameworks* the frameworks for mobile apps use a wrapped browser but additional platform specific APIs that let us interact with the mobile platform.

* *Server-side applications an applications for embedded devices with Node.Js* an environment derived from browser that uses many of the same underlying principles as the browser.

Desktop applications, mobile applications, server-side applications, all these types of applications share  some of the same underlying principles of standard client-side web applications. Understanding how the core mechanics of JavaScript work or the core APIs provided by browsers you’ll become in a versatile developer and gain knowledge and understanding to tackle variety of problems. You’ll be able to build your own server less applications   based in the cloud by using JavaScript APIs for services such as AWS Lambada to deploy, maintain, and control your application’s cloud components. 

</div>

