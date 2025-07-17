# what is the internet 
first lets take a quick look of what is the Internet and what is the difference between the internet and the WWW
https://youtu.be/eHp1l73ztB8?si=sCxrl6-aCvxdy9p5
* the internet is a big infrastructure which is a lot of cables(سلاك) connected with each other.
# who does the internet work in a abstract level.
now we new what is the internet and who does it work and what is the switch and what is the router and the is the modem 
and why do you need them and how does a computer find another computer.
https://developer.mozilla.org/en-US/docs/Learn_web_development/Howto/Web_mechanics/How_does_the_Internet_work
* all the world computer connected with other using a ISP's (in short this is the internet)   
# what is the internet and who does it work (تلخيص الفقرتين الفوق) 
![what is the internet and who does it work photo](images/Screenshot%20from%202025-06-09%2019-45-49.png) 
* in this photo we summarize the internet to be a cable and this cable is used to let the computers to speak to each other 
and to not get confuse to which computer to speak we give each computer a name (ip or a url) so now my computer (client) can speak with the aol or gmail (servers) using that cable 
* now why do my computer called client and the other two computer called servers? the reason for that because the  the servers can directly connected to the cable (the internet) but my computer uses something called isp to get access to the cable (in the future we will took more about the difference between them) //TODO check this chat with chatgpt https://chatgpt.com/share/68471c88-12e4-8006-96fd-cb6ca5e14cda
* what is the difference between the client computer and the server computer 
- the server gives data (response), the client ask for data (request).
- the main difference is that the server is directly connected to the internet which makes the road to it easy, so most of the time the main job for the server is to responds with data to the one's who ask for data, the one's who ask(clients) will find the road easy to get to the server  
- the servers also need to be working 24/7 because it may someone ask for data at any time also servers need to be secure against attacks 
- so why my computer is a client ?? because your computer is hard to access because of the Firewall for my computer and my network Firewall this does not let all the requests get to my computer and my computer can't work all the time and has a weak hardware  and most of the time my computer needs data so he will send the requests.
- but also i can make my computer a server using tools like (python http.server), and you need to configured in a way that let other computers access you (remove the things that protect you).
* the photo is from this video https://youtu.be/7_LPdttKXPc?si=pD11btJ1PHs88i8L.
# The difference between web page, website, web server, and search engine and who does the web work in deep
* what is the browser job?
- Retrieves documents (usually over the internet, using URLs like https://example.com).
- Parses and renders those documents to display them to the user.
- Supports many types of content, but is mainly designed to render HTML documents (web pages).
* what is a web page?
A web page is a document written mainly in HTML (HyperText Markup Language).
* then if the browser job is to get a documents and render them then the browser can get a web page and render them because the web page is a html document.
* what is website?
- a website is a collection of related web pages.
* what is the web server?
- the web server is the program that the browser get the documents from.
- so the web server main job is to handle a browser request, and to do so the server(at the end everything is a process and even the server is a process)needs to has the ability to listen for requests so the server need to be build using tools that give it the ability to listen for requests  
- you can use these tools to build a program with the ability to listen for a requests 
   - Apache HTTP Server, Nginx, Node.js with Express, Python’s Flask/Django.
* what now ?
- so now we have a server that can listen to requests and we have a browser that can make the the request what do you need else 
- first we need the internet that give us access to the cable.
- to make the connection and for that we will use the TCP/IP the TCP/IP will make the connection between the client and the server for us.  
- now the connection is done and now they can speak with each other but what to speak ?? that is the application layer job so if the application layer was a uses http protocol (browser) so they will use a http request and response and they will send and resive  html files
- recurses
    - https://developer.mozilla.org/en-US/docs/Learn_web_development/Getting_started/Web_standards/How_the_web_works#clients_and_servers
    - https://youtu.be/w5-0iBRCQvA?si=TUgeD47iHoIc9sJm
# packet
## ![two computers speak to each other](images/Screenshot%20from%202025-06-16%2013-01-51.png)
* now we knew that if we want to computers to take to each other we just need the to computers to be connected to each other via cable and now we can send the data through that cable and there is no need for a ip or even a packet idea 
## ![alot of computers speak to each other](images/Screenshot%20from%202025-06-16%2013-07-38.png)
* but now what if want alot of computers to take to each other lets say 5 computers now we need a (n * n - 1) cable to  connect all of them togather and this is a vary bad idea if i want to make the internet(alot of computers). 
## ![alot of computers speak to each other](images/Screenshot%20from%202025-06-16%2013-13-27.png)
* but what if there is a thing that his only job is to set between all the computers and made sure that a data from the sender computer is get to the target computer 
- but can the thing that between the computers to new which data for how ??? he can't know because all the computers connected to him he dont now where to go with the data sooo here comes the perfict solution of this problem and it is the packetttt
- now inested of just sending the row data now we want to send the data and send with it the name of the computer the i want to send the data to the now the computer that in the middle now can send the data to the right computer. 
- from now on we will use the packets to make the internet work and the packet is a data with meta data so the data can get to the target using this meta data.
- and there are a lot of things that can get added to the packet not just the name of the target computer(ip), to add the ip of a target computer to a packet we will use the ip protocol and a lot of other protocols that can be added to packet to make the internet better. 
- the tcp protocol can be used to add to the packet a meta data to the packet to tell the target computer about the idea of the connetion that i want to make with him
* now inested of using a lot of cables to make the internet work they decided to make the a lot of things that work betweeb the sender and the target and they are called (switches and routers). 
* to learn more about the ip which this playlist https://youtu.be/5WfiTHiU4x8?si=hBvTov0dVnmdx0nr 
- recurses
   - https://developer.mozilla.org/en-US/docs/Learn_web_development/Howto/Web_mechanics/How_does_the_Internet_work
   - this podcast start at (8:30) https://twit.tv/shows/security-now/episodes/25?autostart=false