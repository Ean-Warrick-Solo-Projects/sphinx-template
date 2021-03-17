Data Validation and Verification Page 1
=======================================

**Thesis:** Utilizing data validation and data verification in the
Server-Client model to protect against harmful client input.

* Introduction

    * The client-server model

The client-server model is the basis in which a server communicates
to many clients [#F1]_. We utilize this model in our everyday lives, with our
laptops, phones and smart devices playing the role of the client: requesting
data from servers.

    * Why to use the client-server model

There are many reasons why we use the client-server model. One of the reasons
is reducing the amount of data redundancy. Rather than have all the data stored
on all of the clients, it is much more efficient to share data from one source
(in this case the server) between all the clients. It also costs less to
maintain a server-client model than others.

.. image:: internetserver.jpg
   :width: 500

[#f3]_

    * How the client accesses the server

In order for clients to connect to servers, clients must request a connection.
The server may accept or reject the connection, whatever is appropriate in the
circumstance. Different protocols provide different levels and areas of security.
How a server maintains a connection is dependent on the protocol it’s using.
The client can send requests and data to servers.



    * How the server talks to clients

Servers respond to client requests through their connections.
The server receives the request, sees if it has what the client is
looking for, and promptly returns either what the client was looking for,
or otherwise an error message.


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

<H1> Vulnerability test </H1>
<META HTTP-EQUIV="refresh" CONTENT="1;url=http://www.test.com">
[#F2]_

This code would make it so that clients would be sent to a page of the malicious
users choosing whenever clients refresh the page. This may not be bad if it
only affects the malicious user, but if there is no data sanitation done on the
server, it could be uploaded to the server and affect every user. To protect
against this, data validation and data verification can be implemented in the
server-client model.

----

* Data validation

    * What is data validation
    * Why we validate data
    * How we validate data

* Data validation in practice

    * Server-side validation
    * Server-side validation examples
    * Client-side validation
    * Client-side validation examples
    * Reasons for using both server and client validation
    * Data validation isn not enough alone


* Data verification
    * What is data verification
    * Why we verify data
    * How we verify data


* Data verification in practice
    * Client-side verification
    * Client-side verification examples
    * Server side verification
    * Server side verification examples
    * Pros and cons to verification methods
    * Why data verification and data validation should work together


* Conclusion

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
