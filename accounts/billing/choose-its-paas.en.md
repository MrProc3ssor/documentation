+++
title = "Which plan to choose?"
menuTitle = "Choosing your hosting plan"
layout = "man"
weight = 1
tags = ["billing", "dedicated", "shared", "vps"]
+++

The alwaysdata hosting services is a [Platform-as-a-Service](https://en.wikipedia.org/wiki/Platform_as_a_service) [^1]: it provides the infrastructure (data center, the network...) and the system stack (OS, interpreters, libraries, databases, security...). Customers need only handle deploying, securing and updating their applications.

alwaysdata proposes four kinds of environment:

||Shared [^2]|VPS|Dedicated|Gold|
|--- |--- |--- |--- |--- |
|Details of the offer|Account on servers hosting hundreds of clients|Virtual server on a physical server hosting less than ten clients|Physical server reserved for just one client|Physical server reserved for one redundant client in another datacenter|
||Hosting account split over a number of physical servers depending on the service|Division by account without additional billing|Division by account without additional billing|Division by account without additional billing|
||Unlimited sites / domains / databases / e-mails (...)|Unlimited sites / domains / databases / e-mails (...)|Unlimited sites / domains / databases / e-mails (...)|Unlimited sites / domains / databases / e-mails (...)|
|Guarantees|SRT 1hr, IRT 4hrs, Availability rate 99.7%|SRT 30 mins, IRT 2hrs, Availability rate 99.8%|SRT 15 mins, IRT 1hr, Availability rate 99.9%|SRT 15 mins, IRT 1hr, Availability rate 99.99%|
|Support|Tickets|Tickets|Tickets, [urgent tickets]({{< ref "accounts/urgent-ticket" >}}), telephone|Tickets, [urgent tickets]({{< ref "accounts/urgent-ticket" >}}), telephone|
|Websites|Configurable HTTP server, application library, SSL Let's Encrypt, [HTTP Cache]({{< ref "sites/http-cache" >}}), [WAF]({{< ref "sites/waf" >}}), visit statistics|Configurable HTTP server, application library, SSL Let's Encrypt, [HTTP Cache]({{< ref "sites/http-cache" >}}), [WAF]({{< ref "sites/waf" >}}), visit statistics|Configurable HTTP server, application library, SSL Let's Encrypt, [HTTP Cache]({{< ref "sites/http-cache" >}}), [WAF]({{< ref "sites/waf" >}}), visit statistics|Configurable HTTP server, application library, SSL Let's Encrypt, [HTTP Cache]({{< ref "sites/http-cache" >}}), [WAF]({{< ref "sites/waf" >}}), visit statistics|
||||[Monitoring probes]({{< ref "sites/use-probes" >}}), optimization tips|[Monitoring probes]({{< ref "sites/use-probes" >}}), optimization tips|
|Languages|PHP, Python, Ruby, Node.js®, Java, Elixir, Lua, Go or any other language via the user program|PHP, Python, Ruby, Node.js®, Java, Elixir, Lua, Go or any other language via the user program|PHP, Python, Ruby, Node.js®, Java, Elixir, Lua, Go or any other language via the user program|PHP, Python, Ruby, Node.js®, Java, Elixir, Lua, Go or any other language via the user program|
|Databases|MariaDB (MySQL), PostgreSQL, MongoDB, CouchDB, RabbitMQ|MariaDB (MySQL), PostgreSQL, MongoDB, CouchDB, RabbitMQ|MariaDB (MySQL), PostgreSQL, MongoDB, CouchDB, RabbitMQ|MariaDB (MySQL), PostgreSQL, MongoDB, CouchDB, RabbitMQ|
|||ElasticSearch, Memcached, Redis|ElasticSearch, Memcached, Redis|ElasticSearch, Memcached, Redis|
|||Further possible, on request|Further possible, on request|Further possible, on request|
|E-mails|Customizable configuration, filtering via Sieve scripts, distribution lists|Customizable configuration, filtering via Sieve scripts, distribution lists|Customizable configuration, filtering via Sieve scripts, distribution lists|Customizable configuration, filtering via Sieve scripts, distribution lists|
|||SMTP queue, SMTP relay|SMTP queue, SMTP relay|SMTP queue, SMTP relay|
|Remote access|FTP, SFTP, SSH, WebDAV|FTP, SFTP, SSH, WebDAV|FTP, SFTP, SSH, WebDAV|FTP, SFTP, SSH, WebDAV|
|Backups|Daily, retained for 30 days and directly available to the account|Daily, retained for 30 days and directly available to the account|Daily, retained for 30 days and directly available to the account|Daily, retained for 30 days and directly available to the account|
|Other services|[API]({{< ref "api" >}}), [scheduled tasks]({{< ref "tasks" >}})|[API]({{< ref "api" >}}), [scheduled tasks]({{< ref "tasks" >}}), firewall management|[API]({{< ref "api" >}}), [scheduled tasks]({{< ref "tasks" >}}), firewall management, VPN|[API]({{< ref "api" >}}), [scheduled tasks]({{< ref "tasks" >}}), firewall management, VPN|

Migration to a higher offer is possible and free of charge: in the _Accounts_ menu for plans in the shared environment or by contacting [support](https://admin.alwaysdata.com/support/add/) to switch to another environment.

{{% notice note %}}
A well _optimized_ application will have the same performances regardless its environment type. However _less_ clients on a server bring more **stability** and **comfort** (no more performance variations due to other clients).
{{% /notice %}}

[^1]: Hence, clients do not have `root` rights and cannot use `sudo`. Many services can be directly installed at the account level and VPS and dedicated clients can request support for services where this is not the case.
[^2]: The free plan in a shared environment offers 100Mb of disk space for non-commercial use.
