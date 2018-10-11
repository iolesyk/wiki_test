<!-- TITLE: Nginx -->
<!-- SUBTITLE: A quick summary of Nginx -->

# NGINX
Popularity
According to Netcraft's November 2016 Web Server Survey,[13] Nginx was found to be the second most widely used web server across all "active" sites (18.22% of surveyed sites) and for the top million busiest sites (27.83% of surveyed sites). According to W3Techs, it was used by 37.7% of the top 1 million websites, 49.7% of the top 100,000 websites, and by 57.0% of the top 10,000 websites.[14] According to BuiltWith, it is used on 38.2% of the top 10,000 websites, and its growth within the top 10k, 100k and 1 million segments increased.[15] A 2018 survey of Docker usage found that Nginx was the most commonly deployed technology in Docker containers.[16] Wikipedia uses Nginx as its SSL termination proxy.[17] As of OpenBSD release 5.2 (1 November 2012), Nginx became part of the OpenBSD base system, providing an alternative to the system's fork of Apache 1.3, which it was intended to replace,[18] but it was later replaced by OpenBSD's own httpd(8).[19]

Features
Nginx can be deployed to serve dynamic HTTP content on the network using FastCGI, SCGI handlers for scripts, WSGI application servers or Phusion Passenger modules, and it can serve as a software load balancer.[20]

Nginx uses an asynchronous event-driven approach, rather than threads, to handle requests.[21] Nginx's modular event-driven architecture can provide more predictable performance under high loads.[22][23]

Nginx default configuration file is nginx.conf.[24]

HTTP proxy and Web server features
Ability to handle more than 10,000 simultaneous connections with a low memory footprint (~2.5 MB per 10k inactive HTTP keep-alive connections)
Handling of static files, index files and auto-indexing
Reverse proxy with caching
Load balancing with in-band health checks[25]
TLS/SSL with SNI and OCSP stapling support, via OpenSSL.
FastCGI, SCGI, uWSGI support with caching
Name- and IP address-based virtual servers
IPv6-compatible
WebSockets, HTTP/1.1 Upgrade (101 Switching Protocols)[26], HTTP/2 protocol support
URL rewriting and redirection[27][28]
Mail proxy features
TLS/SSL support
STARTTLS support
SMTP, POP3, and IMAP proxy
Authentication using an external HTTP server[29]
Other features include upgrading executable and configuration without client connections loss,[30] and a module-based architecture with both core[31] and third-party module support.[32]

The paid Plus product includes additional features such as advanced load balancing and access to an expanded suite of metrics for performance monitoring.[33][34]

Nginx vs Nginx Plus
There are two versions of Nginx, OSS Nginx and Nginx Plus. Nginx Plus offers additional features not included in OSS Nginx, such as Active health checks, session persistence based on cookies, DNS service discovery integration, Cache Purging API, AppDynamic, Datalog, Dynatrace New Relic plug-ins, Active-Active HA with config sync, Key-Value Store, on-the-fly with zero downtime updates upstream configurations and key‑value stores using Nginx Plus API[35] and Web application firewall (WAF) dynamic module.[36]

Performance vs Apache
Nginx was written with an explicit goal of outperforming the Apache web server.[37] Out of the box, serving static files, Nginx uses dramatically less memory than Apache, and can handle roughly four times more requests per second.[38] This performance boost comes at a cost of decreased flexibility, such as the ability to override systemwide access settings on a per-file basis (Apache accomplishes this with an .htaccess file, while Nginx has no such feature built in).[citation needed] Formerly, adding third party modules to nginx required recompiling the application from source with the modules statically linked. This was partially overcome in version 1.9.11 on February 2016, with the addition of dynamic module loading.[39] However, the modules still must be compiled at the same time as nginx, and not all modules are compatible with this system—some require the older static linking process.[40]

History
Nginx, Inc.
Type
Private
Industry	Technology
Founded	2011
Headquarters	San Francisco, California, U.S.[10]
Key people
Gus Robertson (CEO), Igor Sysoev (CTO)
Products	Nginx Web server, Nginx Amplify SaaS, Nginx Controller, Nginx Unix and Nginx Web Application Firewall
Website	nginx.com
Igor Sysoev began development of Nginx in 2002.[9] Originally, Nginx was developed to solve the C10k problem, and to fill the needs of websites including Rambler search engine and portal, for which it was serving 500 million requests per day by September 2008.[41]

A company of the same name was founded in July 2011 by Sysoev to provide commercial products and support for the software.[42]

The company's principal place of business is San Francisco, California, while legally incorporated in British Virgin Islands.[10]

In October 2011, Nginx raised $3 million from BV Capital, Runa Capital and MSD Capital, Michael Dell's venture fund.[43]

The company announced commercial support options for companies using Nginx in production. Nginx offered commercial support in February 2012,[44][45] and paid Nginx Plus subscription in August 2013.[46]

Support packages focus on installation, configuration, performance improvement, etc.[47] Support includes proactive notifications about major changes, security patches, updates and patches.

WordPress developer Automattic Inc. and content delivery network provider MaxCDN became funding partners for an update to Google's SPDY version 3.1, slated for early 2014.[48]

Nginx also offers consulting services to assist customers in custom configuration or adding additional features.[49]

In October 2013, Nginx raised a $10 million series B investment round led by New Enterprise Associates.[50] That round included previous investors, as well as Aaron Levie, CEO and founder of Box.com.[51][52] In December 2014, Nginx raised a $20 million series B1 round led by New Enterprise Associates, with participation from e.ventures (formerly BV Capital), Runa Capital, Index Ventures and Nginx's own CEO Gus Robertson.[53][54]

In October 2017 Nginx Inc. announced general available Nginx Amplify SaaS providing monitoring and analytics capabilities for Nginx.[55]

See also