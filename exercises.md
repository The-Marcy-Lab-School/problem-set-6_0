  # Unit 6 Lesson 0 Problem Set

0. Describe, in as much detail as you can, what happens when you open up Google Chrome, type "marcylabschool.org" into the address bar, and press enter.

    When trying to get to the marcylabschool.org website, our device/browser which is also our client sends a GET request to their respective servers for the files to preview the website.
    Once connected, the server will send back a response. In this case, that response is our entire marcylabschool website.
    
1. HTTP is a "stateless" protocol - what does this mean?

    Stateless protocols are protocals that returns a response to the client based on it's current state. Unlike a stateful protocal, it does not
    require the server to retain any information from previous requests to the server.

2. Given that HTTP is a stateless protocol, how do we build "stateful" web applications.
 
    

3. What is the difference between HTTP and HTTPS?
 
    HTTP stands for Hypertext Transfer Protocol, and the same for HTTPS though far more secure as the addition of the 's' tells us. They both connect to a port, typically port 80 for HTTP and port 443 for HTTPS.
    Esentially, with HTTP it allows for the communication between different systems and web servers. It’s most commonly used to transfer data from a web server to a browser in order to allow users to view web pages.
    Now where HTTPS come in is when users supply confidential information to the browser. What encrypts the information is an SSL certificate. This encrypts the information that users supply to the site so even if someone
    manages to steal or collect the data being sent back and forth between the server they would not be able to understand it due to this encryption.

4. Security is an important concept for web applications. What are two ways we can try to prevent a user's session from being highjacked?

5. What is the Same Origin Policy? What about CORS? How are they related?



6. Using Google Chrome, visit http://www.reddit.com/r/programming, then visit http://www.reddit.com/r/programming/.json. What differences do you notice between the response bodies of the requests? Why might this be important?

    The difference between the responses that I received is that I'll receive a formatted and styled web page that leads to the programming subreddit
    although when I request with JSON it sends back the html skeleton for all the objets within the page. This is important because This data
    could be fetched and used indepently of the site itself. Data could then eb collected and manipulated in various ways.

7. What are request and response headers? Why are they important?

Request and response headers contain all the information about the request that is being sent to a server. This is what determines what type of information
the server sends back to the client. 
<!--These headers tells the server what language to send the information in, or could accommodate for a disability-->
<!--that the user has.-->

<!--
use curl to test out HTTP requests and see it.
-->