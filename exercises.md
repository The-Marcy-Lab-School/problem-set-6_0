# Unit 6 Lesson 0 Problem Set

0. Describe, in as much detail as you can, what happens when you open up Google Chrome, type "marcylabschool.org" into the address bar, and press enter.

- You open up the web browser, which is the platform that will manage sending requests and getting responses from the servers that hold the webpage you're trying to access. When you type in "marcylabschool.org", you're typing a user-friendly version of the DNS (Domain Name System). When you press enter, which the web browser is perhaps listening for, the DNS gets translated into the webpage's IP address, which is a unique label that each computer who accesses the internet has, as well as every webpage in the internet. The request gets sent out to a server, where some of the webpages are stored. If that server doesn't have the webpage you're looking for, it sends the request out to another server, and it keeps going until it does find the webpage. The server sends back the resources and files from that webpage, such as HTML and CSS files, along with things like images and any other resources. Your web browser recieves this response and all of the resources, and parses the information into a jumble of whatever information is on it. Then, it takes that information and displays it on your screen.

1. HTTP is a "stateless" protocol - what does this mean?

- Every page on the internet is independent - if you were to log into an account and taken to another page, technically your data would not be transferred over to the next page because the website remembers nothing that you've inputted. There is nothing that connects your inputted data to other sites - the web browser simply keeps track of requests and responses.

2. Given that HTTP is a stateless protocol, how do we build "stateful" web applications.

- The only way to track any user information, and make it seem like there is some state in the pages you're viewing, is by keeping track of cookies, using your computer's ID and rendering some sort of state on the backend of their site, or any other method that they use to remember your data. When the data is stored, they can reference this data by identifying who is making the request, and given their info, and how their data should be represented when they get the response.

3. What is the difference between HTTP and HTTPS?

- For one thing, the default ports are different. For HTTP, it's 80, while for HTTPS, it's 443. The primary difference between them, however, is that HTTPS has encryption when a request is made to a server. When a request is recieved, an encryption is selected, and it keeps the information private and makes it so that only the server and the client have access to the information being transferred.

4. Security is an important concept for web applications. What are two ways we can try to prevent a user's session from being highjacked?

- One way to prevent a session from being highjacked is by having an engine that keeps track of all requests for a session, or in other words, keeps track of the HTTP headers. Whenever the header changes, a penalty point is given to the session, and when enough points have been reached, the session terminates entirely. The best way to prevent a highjacking is based on the client side, however. By having an anti-virus set up, which has real-time protection (which I assume is constantly scanning for any logged viruses that appear on the web), and by keeping their software up to date (which should also do the same thing), they can take preventive measures to keep their information safe. Even having a VPN can make their information secure.

5. What is the Same Origin Policy? What about CORS? How are they related?

- The Same Origin Policy is a protocol that restricts the way the webpage origin is loaded when accessing another webpage. Changing the pathways to this new page is acceptable, but making any other changes or essentially rerouting the origin will terminate the request and fail. Cross-Origin Resource Sharing (CORS) is giving a web application access to selected sources from a different origin, and the running application initiates the requests in its own to give back to the client. They're related in the fact that they both have restrictions in how the client gets their data. Both require the source to be from where the request was made, and no outside source or change can be made to the initial pathway, otherwise the request will not be accepted.

6. Using Google Chrome, visit http://www.reddit.com/r/programming, then visit http://www.reddit.com/r/programming/.json. What differences do you notice between the response bodies of the requests? Why might this be important?

- Not sure if this makes a difference, but on the first link, using curl, I recieve a large body of the html file for reddit. On the second link, using Google Chrome, it looks a lot cleaner, more organized and you can actually see the way the API is structured. It could be important because you want to quickly search for what you're looking for, rather than spending precious time reading through a massive body of code that's put together in one big mess.