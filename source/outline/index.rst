Web Application Security Outline
================================

**Thesis:** How to secure and protect web applications from hackers
utilizing preventative measures coded within the application.

* Explaining hacking (Will refer to [#f1]_)

    * What is hacking?
    * Why should we worry about hackers?
    * Black hat hackers
    * White hat hackers

* Common hacks and how to protect against them (Will refer to [#f4]_)

    * SQL injections (will have code samples)
    * Broken Authentication exploiting (will have code samples)
    * Important data accessible to client (will have code samples)
    * Remote file inclusion (will have code samples)

* Vulnerability scanners (Will refer to [#f3]_)

    * What is a vulnerability scanner
    * Why should we use Vulnerability scanners
    * How to use vulnerability scanners
    * What to do when a vulnerability is found.

* Client / Server Checks (Will refer to [#F1]_)

    * Never trust the client (will have image)
    * Restrict the power of the client
    * How to set up checks on the client and server (will include code)
    * Proper use cases of client/server interaction (will include code)

* User vulnerabilities (Will refer to [#F2]_)

    * User Data (Cookies) (will include images)
    * Cross-site scripting (XSS) (will include images)
    * Clickjacking  (will include images)
    * Uploaded data sanitation (data verification) (will include code)

* Other ways to protect your  (will refer to [#F2]_, [#F5]_, and [#F6]_)

    * Encoding Data
    * Firewall (image)
    * HTTPS
    * Two-Step verification (image)

Footnote Sources:

.. [#f1] Cross, M. (2007). "`Developer's guide to web application security
    <https://simpsoncollege.on.worldcat.org/oclc/85861133>`_". Syngress Pub.
    Retrieved February 8, 2021

.. [#f2] Reis, C., Barth, A., & Pizano, C. (2009). "`Browser Security: Lessons
    from Google Chrome: Google Chrome developers focused on three key problems
    to shield the browser from attacks
    <https://dl.acm.org/doi/pdf/10.1145/1551644.1556050>`_". Queue, 7(5), 3-8.
    Retrieved February 8, 2021

.. [#f3] Netsparker Security Team (2019, May 29). "`Getting started with web
    application security. <https://www.netsparker.com/blog/web-security/getting-started-web-application-security/>`_"
    Retrieved February 8, 2021

.. [#f4] NDC Conferences, Christian Wenz (2017, July 10). "`Web Application
    Security Risks: A Look at OWASP Top Ten 2017 - Christian Wenz
    <https://youtu.be/avFR_Af0KGk>`_". Retrieved February 8, 2021

.. [#f5] Ashri, R., Payne, T., Marvin, D., Surridge, M., & Taylor, S. (2004).
    "`Towards a semantic web security infrastructure
    <https://www.aaai.org/Papers/Symposia/Spring/2004/SS-04-06/SS04-06-012.pdf>`_."
    Retrieved February 8, 2021

.. [#f6] Uncle M. (2021) Personal Interview
