# Chat Application

<ul>
	<li><a href="#results">Final Results</a></li>
	<li><a href="#explain">Code Explanations and Notes</a></li>
	<li><a href="#howToRun">How to run?</a></li>
</ul>

<h3 id='explain'>Code Explanations and Notes</h3>

* defining the model for the messages:<br>
each message has 3 fields: 1) sender 2) message/body 3) type, which is an enum and is one of 3 types (chat, join, leave)
* STOMP:<br> These methods come from Spring frameworks STOMP implementation. STOMP stands for Simple Text Oriented Messaging Protocol. It is a messaging protocol that defines the format and rules for data exchange. Why do we need STOMP? Well, WebSocket is just a communication protocol. It doesn’t define things like - How to send a message only to users who are subscribed to a particular topic, or how to send a message to a particular user. We need STOMP for these functionalities.
* notes on main.js: <br> `getAvatarColor` uses the length of the users username to choose the avatar color so that we wouldn't have to hard code different colors or have a situation where all the users have the same avatar color 


<h3 id='results'>Final Results</h3>
<img src="result/1.png"><br>
<img src="result/2.png"><br>


<h3 id='howToRun'>How to run?</h3>
<code>
	mvn spring-boot:run
</code>

