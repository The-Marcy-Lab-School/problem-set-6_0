# Unit 6 Lesson 0 Problem Set

0. Describe, in as much detail as you can, what happens when you open up Google Chrome, type "marcylabschool.org" into the address bar, and press enter.
- When this happens, we are typing the URL of a page using the client program, in this case, Google Chrome.
- Your computer is the client sending a HTTP request to a web sever and waits for a response.
- Because the HTTP is a conectionless protocol, the client will diconnect from the web serveer while waiting for a reponse
- The sever will process the request, prepare the response, will establish the connection again, and will send back a response in the form of an HTTP message 
- The marcylabschool website will appear in the browser and the connection between the server and client will diconnect.


1. HTTP is a "stateless" protocol - what does this mean?
- This means that the client and the server know about eachother only during the current request.
- If the request closes and the computers want to connect again they need to provide information to eachother again and they can connect like the first request. 


2. Given that HTTP is a stateless protocol, how do we build "stateful" web applications.
- We can create "statefulness" using sessions and cookies
- One way to do this is with a session id. 
    - Whenever a client sends a request to the server, the client appends a session id to the request, which helps servers identify clients. 
- Another way to maintain statefulness is with the use of cookies or HTTP cookies. 
    - Cookies are small files stored in the browser and contain the session information.
    - By default most browsers have cookies.
    - When you send a request to access a website for the first time, the server sends a session id and sets it in your browser cookie stored in your local computer. 
    - This session data is stored on the server and every time you visit the page again your session will be recognized because of the cookie. 
    


3. What is the difference between HTTP and HTTPS?

- In HTTPS, there are encrypted connections. It allows secure transactions by encrypting the entire communication with a combination of SSL/TLS protocol and HTTP. 
- HTTP also allows you to create a secure encrypted connection between the server and the browser.There is no data encryption implemented.


4. Security is an important concept for web applications. What are two ways we can try to prevent a user's session from being highjacked?



5. What is the Same Origin Policy? What about CORS? How are they related?



6. Using cURL, make requests to http://www.reddit.com/r/programming and http://www.reddit.com/r/programming/.json from the command line. What differences do you notice between the two different response bodies? Why is this be significant?



7. What are request and response _headers_? Why are they important?
