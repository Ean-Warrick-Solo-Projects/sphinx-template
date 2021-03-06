Data Validation and Verification Page 1
=======================================

**Thesis:** Utilizing data validation and data verification within the
server-client model to protect against potentially harmful client input.

    * Introduction: The client-server model

The client-server model is the basis in which a server communicates to many
clients [#F1]_. When using technology devices on the internet, usually the
device plays the role of the client. As example, gamers use this when playing
online multiplayer games. Online gamers, who are the client, send information of
their inputs to the server which the server sends back information back to all
of the clients, such as opponent player location and the game state.

    * Why to use the client-server model

There are many reasons why we use the client-server model. One of the reasons
is reducing the amount of data redundancy. Rather than have all the data stored
on all of the clients, it is much more efficient to share data from one source
(in this case the server) between all the clients. It also costs less to
maintain a server-client model than other models.

.. image:: internetserver.jpg
   :width: 500

Image from W3Schools [#f3]_

    * How the client accesses the server

In order for clients to connect to servers, clients must request a connection.
The server may accept or reject the connection, whatever is appropriate in the
circumstance. How the connection is handled is determined by the protocols.
Protocols refers to the method and execution of data transmission through a
connection. Different protocols provide different levels, areas of security
and speed of transfer. The most commonly used protocols are UDP, HTTP, and FTP.
Through connections with servers, clients can send requests in which servers
respond by sending information back to the client. Clients can also use
connections to send data to servers, which servers can utilize. As an example,
when uploading a profile picture to a social media, that photo is sent as data
to a server, which receives the image and stores it on the server.


    * How the server talks to clients

Servers respond to client requests through their connections.
When a server receives a request from a client, such as a request of a page
on the internet, the server will first look at what the client is wanting to
request. The server looks through its resources in order to see if it has what
the client is requesting. If the resource is found, the server will send a copy
back to the client through its established connection.


    * Never trust the client

Servers should never trust data that is received from clients. Client users are
usually good hearted and are just looking to upload or input data. However,
there are individuals that will take this neat feature and use it to their
advantage, and while also making it a disadvantage to others. Clients can
manipulate data they send to the server, which could possibly break the function
of servers not expecting the type of input. Even worse, manipulated data can
contain malicious code which could have adverse effects on servers, or even
other clients.

Here is an example of HTML a malicious user could inject into the code of a
website:

.. code-block:: html

    <H1> Vulnerability test </H1>
    <META HTTP-EQUIV="refresh" CONTENT="1;url=http://www.test.com">

Example code retrieved from CodeProject [#F2]_

This code would make it so that clients would be sent to a page of the malicious
users choosing whenever clients refresh the page. In the example,
the HTTP-EQUIV="refresh"
represents the action of refreshing the web page, followed by
CONTENT="1;url=http://www.test.com"
which is the page that is returned when the page is refreshed. This may not be
bad if it only affects the malicious user, but if there is no data sanitation
done on the server, it could be uploaded to the server and affect every user. To
protect against this, data validation and data verification can be implemented
in the server-client model.

----

* Data validation (Will include images representing
  validation process)

    * What is data validation
    * Why we validate data
    * How we validate data


* Data validation in practice (will include code
  representing possible validation examples)

    * Server-side validation
    * Server-side validation examples
    * Client-side validation
    * Client-side validation examples
    * Reasons for using both server and client validation
    * Data validation isn not enough alone


* Data verification (will include images)

    * What is data verification
    * Why we verify data
    * How we verify data


* Data verification in practice (will include code)

    * Client-side verification
    * Client-side verification examples
    * Server side verification
    * Server side verification examples
    * Pros and cons to verification methods
    * Why data verification and data validation should work together


* Conclusion (will include citations)

    * The Client-server model is prevalent today
    * The client-server model has vulnerabilities
    * Data verification and data validation can help mitigate these
      vulnerabilities

Footnote Sources:

.. [#f1] Christensson, Per. "`Client-Server Model Definition
    <https://techterms.com/definition/client-server_model>`_".
    TechTerms. Sharpened Productions, 17 June 2016. Web. 16 March 2021.

.. [#f2] Skynet_Code. "`HTML and JavaScript Injection
    <http://www.codeproject.com/Articles/134024/HTML-and-JavaScript-Injection>`_".
    CodeProject, 7 Dec. 2010.

.. [#f3] W3schools.
    "`What Is Client-Server Architecture? W3schools Online Programming Tutorials.
    <http://www.w3schools.in/what-is-client-server-architecture>`_".

.. [#f4] Inspire EU. "`Best practices - validation <https://www.youtube.com/watch?v=_RTHDVVGaKU>`_"
   Uploaded 29 November 2018. Retrieved 13 March 2021.

.. [#f5] Enriquez, Rene. "`RESTful Java Web Services Security
   <http://search.ebscohost.com/login.aspx?direct=true&db=nlebk&AN=817631&site=ehost-live&scope=site>`_".
   Packt Publishing, 2014. EBSCOhost. Retrieved 13 March 2021

.. [#f6] Deepa, G., and P. Santhi Thilagam.
   "Securing web applications from injection and logic vulnerabilities:
   Approaches and challenges." Information and Software Technology
   74 (2016): 160-180.

