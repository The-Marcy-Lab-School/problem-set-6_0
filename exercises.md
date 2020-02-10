# Unit 6 Lesson 0 Problem Set

0. Describe, in as much detail as you can, what happens when you open up Google Chrome, type "marcylabschool.org" into the address bar, and press enter.
    
    After typing the URL, the browsers  first checks its memory for the IP address that is linked to that domain name. 
    Failing that, the operating system's memory is checked. Failing even that, a request for the IP is sent to a specified DNS server made to match domain names to IP addresses. 
    If and when an IP address is identified, the browser sends a request to the server hosting the "marcylabschool.org" website following the HTTP(S) protocol. This request is bundles with what the person wants to view, IP  and machine information. 
    This GET request is split into packets to facilitate a quicker transfer of data and send to the host server.
    The server will then serve the response with packets containing the information to render the website which is the interpretted by the browser.

1. HTTP is a "stateless" protocol - what does this mean?
    
    HTTP is stateless because each request is bundled with the information needed to function properly. 
    Thus, the server doesn't need to store information about the current state of a transaction.

2. Given that HTTP is a stateless protocol, how do we build "stateful" web applications.
    
    Applications can achieve a sense of 'statefulness' with the use of cookies.
    Cookies allow web applications to store data client-side that enable a better user experience across platforms when used ethically.

3. What is the difference between HTTP and HTTPS?
    
    HTTPS, or Secure HTTP, means that every request/response packet is encrypted.
    This prevents other users who intercept the packets as they travel from accessing sensitive information.

4. Security is an important concept for web applications. What are two ways we can try to prevent a user's session from being highjacked?
    
    One way is to have a users session expire after a certain amount of time.
    This limits the time someone could pretend to be the user. Another way is to reset the session before an important action, 
    meaning the user has to re-authenticate their session.

5. What is the Same Origin Policy? What about CORS? How are they related?
    
    The Same Origin Policy restricts how a web application accesses information, limiting it to the same origin/location as itself, 
    meaning the same server, port, and protocol. CORS, cross-origin resource sharing,
    allows us to use HTTP to give our web applications access to other specific origins.

6. Using Google Chrome, visit http://www.reddit.com/r/programming, then visit http://www.reddit.com/r/programming/.json. What differences do you notice between the response bodies of the requests? Why might this be important?
    
    The link to starts as an HTML file meant to be rendered by our browsers. 
    The response from the link that ends with .json is a JSON. This is important because the JSON has data that can be parsed and interpretted depending on the use case. 
    The JSON object acts as a storage space for key points of data in any given time.