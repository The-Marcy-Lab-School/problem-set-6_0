# Unit 6 Lesson 0 Problem Set

0. Describe, in as much detail as you can, what happens when you open up Google Chrome, type "marcylabschool.org" into the address bar, and press enter.
    + After typing the URL, the browsers checks its memory for the IP address corresponding to that domain name. If it can't find it, the operating system's memory is checked. If it doesn't exist there, a request for the IP is sent to a specified DNS server responsible for this task of matching domain names to IP addresses. After an IP address is identified, the browser sends a request to the server hosting the "marcylabschool.org" website following the HTTP(S) protocol. This request includes what we want to access, our IP address, and other relevant information about our system. This *GET* request and the other information that travels the internet is broken up into packets that each find the most efficient route to the target computer where they are reassembled once all the pieces arrive. The server to which we sent a request is usually programmed to respond by sending back information, in this case the markup, styling, and JavaScript files that allows our browser to display the "marcylabschool.org" website.

1. HTTP is a "stateless" protocol - what does this mean?
    + HTTP is stateless because each request (unit of communication) has all of the information needed to function properly. Thus, the server doesn't need to store information about the current state of a transaction, i.e, tracking the state.

2. Given that HTTP is a stateless protocol, how do we build "stateful" web applications?
    + Applications that give the illusion of 'statefulness' are possible with the use of cookies. Cookies allow web applications to store data client-side that enable a coherent experience across sessions.

3. What is the difference between HTTP and HTTPS?
    + HTTPS, or Secure HTTP, means that every request/response packet is encrypted. This prevents other users who intercept the packets as they travel from accessing sensitive information.

4. Security is an important concept for web applications. What are two ways we can try to prevent a user's session from being hijacked?
    + One way is to set a user's session (enabled by cookies) to expire after a certain amount of time. This limits the time someone could pretend to be the user. Another way is to reset the session before an important action, meaning the user has to re-authenticate their session.

5. What is the Same Origin Policy? What about CORS? How are they related?
    + The Same Origin Policy is one of the ways in which the web is kept secure. It restricts how a web application accesses information, limiting it to the same origin as itself, meaning the same server, port, and protocol. CORS, cross-origin resource sharing, allows us to use HTTP to give our web applications access to other specific origins.

6. Using cURL, make requests to http://www.reddit.com/r/programming and http://www.reddit.com/r/programming/.json from the command line. What differences do you notice between the two different response bodies? Why is this significant?
    + The link to the regular website is an HTML file meant to be rendered by our browsers. The response from the link that ends with `.json` is a JSON. This is an important distinction because when we want our applications to fetch data from the internet, a JSON file is meant to be manipulated and parsed while a HTML file is not.

7. What are request and response _headers_? Why are they important?
    + Request and response headers carry information about the request being sent. They are important because both the server and client can make decisions based on the information in the headers.


