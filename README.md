# Unit 6 Lesson 0 Problem Set

0. Describe, in as much detail as you can, what happens when you open up Google Chrome, type "marcylabschool.org" into the address bar, and press enter.

Our client (device) sends a GET request to our client's ISP which then passes that GET request to the server containing the marcylabschool.org HTML file, the server then sends a response back containing a an HTML file and its necessary resources, which our browser then proceeds to render.

1. HTTP is a "stateless" protocol - what does this mean?

This essentially means that the state of your page is not saved as a part of the protocol. For example if you log into Headlibrary.com, whom does not have cookies to save your data, then if you were to refresh your page, (sending another GET request) then the fact that you logged in is not saved as apart of the state of the page, so a fresh guest page is then rendered.

2. Given that HTTP is a stateless protocol, how do we build "stateful" web applications.

We build stateful web applications by by assigning things like cookies to clients so that for each of their GET requests, they can be recognized by the server and be sent a response with information assigned to that cookie ID

3. What is the difference between HTTP and HTTPS?

The difference is that unlike HTTP, HTTPS connections send encrypted data to one another. That way if any information is intercepted it would be encrypted rather than open.

4. Security is an important concept for web applications. What are two ways we can try to prevent a user's session from being highjacked?

One way is re-authentification before sensitive information is transmitted, this way if your session is hijacked then you can ensure it is actually the user sending/recieving the information. Another method is http header tracking. Essentially this method is when the server monitors the header and IP address, so that each time the header changes the server counts that against the user, and after a certain amount of changes, the connection is terminated. 

5. What is the Same Origin Policy? What about CORS? How are they related?

The same origin policy is the concept of one web application having access to data in another so long as they share the same origin (same web server). CORS stands for cross origin resource sharing, which means it's the exact opposite of the same origin policy, but it's restricted by browsers as it is a security hazard.

6. Using cURL, make requests to http://www.reddit.com/r/programming and http://www.reddit.com/r/programming/.json from the command line. What differences do you notice between the two different response bodies? Why is this be significant?

The first link shows me the HTML and scripts within it while the second link give me back a string in JSON which I can then parse and use. This is significant because it allows me to extract more information with the second link, whereas the first link is not very useful to my code at all.

7. What are request and response _headers_? Why are they important?

Request and response headers are used to send additional information along with the body of GET requests, which is useful for helping the receiver of the request or response to decide how to process it. It's important because it allows us to build stateful applications, as well as implement methods to secure client/server communications
