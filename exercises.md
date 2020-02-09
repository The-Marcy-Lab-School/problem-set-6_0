# Unit 6 Lesson 0 Problem Set

0. Describe, in as much detail as you can, what happens when you open up Google Chrome, type "marcylabschool.org" into the address bar, and press enter.
Answer: When I open Google Chrome and type "marcylabschool.org" into the address bar, and press enter, our device(client) is sending a GET request to the server that is hosting the marcylabschool html file. The server then sends back a response to our device containing the html file which our browser, then loads the page that we asked for.

1. HTTP is a "stateless" protocol - what does this mean?
Answer: Stateless protocol means the connection between the browser and server when you make a 'GET' request. When you send a request to a stateless server, it does not create any objects that track information regarding your requests. If you "open" something on the server, the server retains no information at all that you have something open.

2. Given that HTTP is a stateless protocol, how do we build "stateful" web applications.
Answer: HTTP can be made to act as if it were maintaining a stateful connection with the server, even though it's not. One way to accomplish this is by having the server send some form of a unique token to the client. Whenever a client makes a request to that server, the client appends this token as part of the request, allowing the server to identify clients. In web development, we call this unique token that gets passed back and forth the session identifier. We can also use cookies , cookies are a way for a server to store a little bit of information in your browser. 

3. What is the difference between HTTP and HTTPS?
Answer: HTTP stands for Hypertext Transfer Protocol which is used by a client and server which allows you to communicate with other websites. The data is sent in text format which is easy to read by anyone. HTTPS stands for Hypertext Transfer Protocol Secure. Generally sites running over HTTPS will have a redirect in place so even if you type in http:// it will redirect to deliver over a secured connection.

4. Security is an important concept for web applications. What are two ways we can try to prevent a user's session from being highjacked?
Answer: Two ways we can try to prevent a user's session from being highjacked are Content Security Policy (CSP) and Certificate Transfer (CT). CSP only allow CSS and Javascript from certain domains you choose to run on your website. Helps protect against cross-site-scripting attacks. Certificate Transparency is a system that can help find malicious SSL certificates issued for your site. This header gives the browser a URL to use to report bad certificates to you. 

5. What is the Same Origin Policy? What about CORS? How are they related?
Answer: The same origin policy is one way browsers protect you from malicious Javascript code. CORS stands for Cross Origin Resource Sharing. They are related because Cross-origin requests are not allowed by default because of the same origin policy.

6. Using cURL, make requests to http://www.reddit.com/r/programming and http://www.reddit.com/r/programming/.json from the command line. What differences do you notice between the two different response bodies? Why is this be significant?
Answer: The differences I notice between the two different response bodies are, the response I received when I made a request to http://www.reddit.com/r/programming was a raw HTTP response data of the page on Reddit. The response I received when I request http://www.reddit.com/r/programming/.json was a response data formatted by JSON. This is significant because if you've never seen raw HTTP response data before, this may be quite shocking. You can process and make some sense of it but you might not be able to paint a picture of what's going on. Ths JSON formatted data of the same page makes it easier to read and understand what you are actually requesting. 

7.What are request and response headers? Why are they important?
Answer: Request headers give more information about the client and the resource to be fetched. Response headers offer more information about the resource being sent back. They are important because for example we had a client that is requesting information but he is an English speaker when he makes the request if the server is located in an area where English is not the first language, it wouldn't be useful to send him data he cannot read or understand. By using headers when request data we send bits of information about us so when the server responds, it responds back to us in a way we can understand. This is important because it enables the client and server to communicate to each other in a better way.