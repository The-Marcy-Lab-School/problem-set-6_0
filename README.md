# Unit 6 Lesson 0 Problem Set

0. Describe, in as much detail as you can, what happens when you open up Google Chrome, type "marcylabschool.org" into the address bar, and press enter.
    When you open up "marcylabschool.org" into the browser, a request is sent to the devices network interface. This request goes over to the Internet and the searches for the url which is a human-readable IP address, within a remote server. The server then accepts the request and sends a response over to the Internet, is sent to the network interface, and makes it back to the network interface. In the end the browser displays the response in what can be see as a web page.

1. HTTP is a "stateless" protocol - what does this mean?
    This means that HTTP is  designed in a way in which each request and response pair is entirely independent of the previous one.

2. Given that HTTP is a stateless protocol, how do we build "stateful" web applications.
    "Stateful" web applications are made possible through techniques such as sessions, cookies, and Asynchronous JS to simulate a stateful experience.

3. What is the difference between HTTP and HTTPS?
    HTTPS is a secure form of HTTP. Evey request and response is encrypted before being transported on the network.

4. Security is an important concept for web applications. What are two ways we can try to prevent a user's session from being highjacked?
    In order to prevent session highjacking, having session expirations would reduce the time for an attacker to pose as a user. Also resetting session, would have an authenticating system which would require a successful login to render an old session id invalid and create a new sessions id.

5. What is the Same Origin Policy? What about CORS? How are they related?
    Same Origin Policy is a concept that permits unrestricted interaction between resources that come from the same origin. SOP is an important gaurd against session hacking however it creates restrictins for programmers who have a need to make restricted forms of cross-origin requests. CORS deals with this issue and allows for normally restricted cross-origin interactions to take place.

6. Using cURL, make requests to https://www.reddit.com/r/programming and https://www.reddit.com/r/programming/.json from the command line. What differences do you notice between the two different response bodies? Why is this be significant?
    The URL without the .json is formatted as string and is visually more complicated to read. JSON allows for a string to be not only formatted in a more organized manner but also parses the string into usable objects, arrays, and string which allows for programmers to easily access certain aspects of data.

7. What are request and response _headers_? Why are they important?
    Request and response _headers_ allow for the client and server to send additional information during the request and responese HTTP cycle.
