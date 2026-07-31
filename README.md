# Web-Security

> Master web security: OWASP Top 10, XSS, SQLi, CSRF, and secure coding practices. Includes labs, tools, and examples for secure web development.


## Contact With Me:

<div align="left">
  <a href="https://www.youtube.com/@awjunaid/featured" target="_blank">
    <img src="https://img.shields.io/static/v1?message=Youtube&logo=youtube&label=&color=FF0000&logoColor=white&labelColor=&style=for-the-badge" height="27" alt="youtube logo"  />
  </a>
  <a href="https://www.instagram.com/awjunaid_" target="_blank">
    <img src="https://img.shields.io/static/v1?message=Instagram&logo=instagram&label=&color=E4405F&logoColor=white&labelColor=&style=for-the-badge" height="27" alt="instagram logo"  />
  </a>
  <a href="https://www.twitch.tv/awjunaid" target="_blank">
    <img src="https://img.shields.io/static/v1?message=Twitch&logo=twitch&label=&color=9146FF&logoColor=white&labelColor=&style=for-the-badge" height="27" alt="twitch logo"  />
  </a>
  <a href="mailto:awjunaid@proton.me" target="_blank">
    <img src="https://img.shields.io/static/v1?message=Proton%20Mail&logo=protonmail&label=&color=7341FF&logoColor=white&labelColor=&style=for-the-badge" height="27" alt="proton mail logo"  />
  </a>
  <a href="https://www.linkedin.com/in/aw-junaid" target="_blank">
    <img src="https://img.shields.io/static/v1?message=LinkedIn&logo=linkedin&label=&color=0077B5&logoColor=white&labelColor=&style=for-the-badge" height="27" alt="linkedin logo"  />
  </a>
  <a href="https://twitter.com/awjunaid_" target="_blank">
    <img src="https://img.shields.io/static/v1?message=Twitter&logo=twitter&label=&color=1DA1F2&logoColor=white&labelColor=&style=for-the-badge" height="27" alt="twitter logo"  />
  </a>
  <a href="https://discord.gg/Neddn8gPqY" target="_blank">
    <img src="https://img.shields.io/static/v1?message=Discord&logo=discord&label=&color=7289DA&logoColor=white&labelColor=&style=for-the-badge" height="27" alt="discord logo"  />
  </a>
</div>



Needless to say, most websites suffer from various types of bugs which may eventually lead to vulnerabilities. Why would this happen so often? There can be many factors involved including misconfiguration, shortage of engineers' security skills, etc. To combat this, here is a curated list of Web Security materials and resources for learning cutting edge penetration techniques, and I highly encourage you to read this article "[So you want to be a web security researcher?](https://portswigger.net/blog/so-you-want-to-be-a-web-security-researcher)" first.


---

## Table of Contents

- [Digests & News](#digests--news)
- [Forums & Communities](#forums--communities)
- [Vulnerability Classes](#vulnerability-classes)
  - [XSS — Cross-Site Scripting](#xss--cross-site-scripting)
  - [Prototype Pollution](#prototype-pollution)
  - [CSV Injection](#csv-injection)
  - [SQL Injection](#sql-injection)
  - [NoSQL Injection](#nosql-injection)
  - [Command Injection](#command-injection)
  - [ORM Injection](#orm-injection)
  - [Template Injection (SSTI/CSTI)](#template-injection-ssticsti)
  - [XXE — XML External Entity](#xxe--xml-external-entity)
  - [CSRF — Cross-Site Request Forgery](#csrf--cross-site-request-forgery)
  - [Clickjacking](#clickjacking)
  - [SSRF — Server-Side Request Forgery](#ssrf--server-side-request-forgery)
  - [Web Cache Poisoning / Deception](#web-cache-poisoning--deception)
  - [Request Smuggling](#request-smuggling)
  - [Relative Path Overwrite](#relative-path-overwrite)
  - [Open Redirect](#open-redirect)
  - [Insecure Deserialization](#insecure-deserialization)
  - [File Upload Vulnerabilities](#file-upload-vulnerabilities)
  - [IDOR & Access Control](#idor--access-control)
  - [Race Conditions](#race-conditions)
  - [GraphQL Security](#graphql-security)
  - [API Security (REST/gRPC)](#api-security-restgrpc)
- [Identity, Auth & Standards](#identity-auth--standards)
  - [OAuth / OpenID Connect](#oauth--openid-connect)
  - [JWT — JSON Web Tokens](#jwt--json-web-tokens)
  - [SAML](#saml)
  - [SSL/TLS](#ssltls)
- [Framework & Platform Specific](#framework--platform-specific)
  - [Rails](#rails)
  - [AngularJS / Angular](#angularjs--angular)
  - [React](#react)
  - [WordPress & CMS](#wordpress--cms)
  - [Webmail](#webmail)
- [Infrastructure & Cloud](#infrastructure--cloud)
  - [AWS](#aws)
  - [Azure](#azure)
  - [GCP](#gcp)
  - [NFS](#nfs)
  - [DNS Rebinding](#dns-rebinding)
- [Reconnaissance](#reconnaissance)
  - [Fingerprinting](#fingerprinting)
  - [Sub-Domain Enumeration](#sub-domain-enumeration)
  - [OSINT](#osint)
- [Cryptography](#cryptography)
- [Web Shells & Post-Exploitation](#web-shells--post-exploitation)
- [Browser Exploitation](#browser-exploitation)
  - [Frontend / Logic-Level](#frontend--logic-level)
  - [Engine / Native-Level](#engine--native-level)
- [Evasion Techniques](#evasion-techniques)
  - [XXE Evasion](#xxe-evasion)
  - [CSP Bypasses](#csp-bypasses)
  - [WAF Evasion](#waf-evasion)
  - [JS Framework Sandboxes](#js-framework-sandboxes)
  - [Authentication Bypass](#authentication-bypass)
- [Notable Write-ups & Case Studies](#notable-write-ups--case-studies)
- [Proof-of-Concept Databases](#proof-of-concept-databases)
- [Cheat Sheets](#cheat-sheets)
- [Tools](#tools)
  - [All-in-One Platforms](#all-in-one-platforms)
  - [Auditing](#auditing)
  - [Command Injection](#tools-command-injection)
  - [Reconnaissance Tools](#reconnaissance-tools)
  - [Fuzzing](#fuzzing)
  - [Scanning](#scanning)
  - [Penetration Testing Frameworks](#penetration-testing-frameworks)
  - [Secrets & Repo Leaking](#secrets--repo-leaking)
  - [Offensive — By Vulnerability](#offensive--by-vulnerability)
  - [Detection](#detection)
  - [Prevention](#prevention)
  - [Proxies](#proxies)
  - [Web Shells](#web-shells)
  - [Disassemblers & Decompilers](#disassemblers--decompilers)
  - [DNS Rebinding Tools](#dns-rebinding-tools)
  - [Misc Tools](#misc-tools)
- [Social Engineering](#social-engineering)
- [Blogs](#blogs)
- [Practice Platforms & CTFs](#practice-platforms--ctfs)
  - [General Web Application](#general-web-application)
  - [XSS Challenges](#xss-challenges)
  - [Cloud (AWS/Azure/GCP)](#cloud-awsazuregcp)
  - [ModSecurity / WAF Tuning](#modsecurity--waf-tuning)
- [Bug Bounty Methodology](#bug-bounty-methodology)
- [Community](#community)
- [Miscellaneous](#miscellaneous)
- [License](#license)

---

## Digests & News

- [Hacker101](https://www.hacker101.com/) — Free video classes and CTFs for web hackers, run by HackerOne.
- [The Daily Swig](https://portswigger.net/daily-swig) — Web security news digest from PortSwigger.
- [tl;dr sec](https://tldrsec.com/) — Weekly newsletter summarizing top security tools, posts, and research.
- [PayloadsAllTheThings](https://github.com/swisskyrepo/PayloadsAllTheThings/) — Massive living repository of payloads and bypass techniques for almost every vulnerability class.
- [CTF Field Guide](https://trailofbits.github.io/ctf/) — Reference material for CTF-style exploitation.
- [Infosec Newbie](https://www.sneakymonkey.net/2017/04/23/infosec-newbie/) — Entry points into the infosec field.
- [The Magic of Learning](https://bitvijays.github.io/) — Structured notes on offensive security learning paths.
- [HackTricks](https://book.hacktricks.wiki/) — Enormous, continuously updated wiki covering web, cloud, and pentesting techniques.
- [Awesome Hacking](https://github.com/Hack-with-Github/Awesome-Hacking) — Curated list of hacking tutorials, tools, and resources.
- [OWASP Cheat Sheet Series](https://cheatsheetseries.owasp.org/) — Authoritative, actively maintained defensive cheat sheets for nearly every vulnerability class.
- [SANS Internet Storm Center](https://isc.sans.edu/) — Daily security news and threat handler diaries.

## Forums & Communities

- [Phrack Magazine](http://www.phrack.org/) — Long-running e-zine written by and for hackers.
- [The Hacker News](https://thehackernews.com/) — Security news aggregator.
- [Security Weekly](https://securityweekly.com/) — Security podcast network.
- [The Register – Security](https://www.theregister.com/security/) — Tech/security news.
- [Dark Reading](https://www.darkreading.com/) — Information security community news.
- [r/netsec](https://www.reddit.com/r/netsec/) — Technical security news and write-ups.
- [InfoSec Exchange](https://infosec.exchange/) — Mastodon instance popular with the security community.

---

## Vulnerability Classes

### XSS — Cross-Site Scripting

- [Cross-Site Scripting – Application Security – Google](https://www.google.com/intl/sw/about/appsecurity/learning/xss/)
- [H5SC](https://github.com/cure53/H5SC) — HTML5 Security Cheatsheet.
- [AwesomeXSS](https://github.com/s0md3v/AwesomeXSS)
- [Excess XSS](https://excess-xss.com/) — A beginner's guide to cross-site scripting.
- [THE BIG BAD WOLF - XSS AND MAINTAINING ACCESS](https://www.paulosyibelo.com/2018/06/the-big-bad-wolf-xss-and-maintaining.html)
- [payloadbox/xss-payload-list](https://github.com/payloadbox/xss-payload-list)
- [PayloadsAllTheThings - XSS Injection](https://github.com/swisskyrepo/PayloadsAllTheThings/tree/master/XSS%20Injection)
- [PortSwigger — Cross-site scripting](https://portswigger.net/web-security/cross-site-scripting) — Full theory + interactive labs.
- [DOM Clobbering — the Underrated Vulnerability Class](https://portswigger.net/research/dom-clobbering-strikes-back) — Modern DOM-based attack vector.
- [OWASP XSS Filter Evasion Cheat Sheet](https://owasp.org/www-community/xss-filter-evasion-cheatsheet)

### Prototype Pollution

- [Prototype pollution attack in NodeJS application (paper)](https://github.com/HoLyVieR/prototype-pollution-nsec18/blob/master/paper/JavaScript_prototype_pollution_attack_in_NodeJS.pdf)
- [Exploiting prototype pollution – RCE in Kibana (CVE-2019-7609)](https://research.securitum.com/prototype-pollution-rce-kibana-cve-2019-7609/)
- [Real-world JS - 1](https://blog.p6.is/Real-World-JS-1/)
- [Server-Side Prototype Pollution](https://portswigger.net/research/server-side-prototype-pollution) — PortSwigger research on detecting it via gadget probing.
- [PP2RCE — Client-Side Prototype Pollution](https://github.com/BlackFan/client-side-prototype-pollution) — Scanner + gadget database for client-side PP-to-XSS.

### CSV Injection

- [CSV Injection -> Meterpreter on Pornhub](https://news.webamooz.com/wp-content/uploads/bot/offsecmag/147.pdf)
- [The Absurdly Underestimated Dangers of CSV Injection](http://georgemauer.net/2017/10/07/csv-injection.html)
- [PayloadsAllTheThings - CSV Injection](https://github.com/swisskyrepo/PayloadsAllTheThings/tree/master/CSV%20Injection)

### SQL Injection

- [SQL Injection Cheat Sheet](https://www.invicti.com/blog/web-security/sql-injection-cheat-sheet/)
- [SQL Injection Wiki](https://sqlwiki.netspi.com/)
- [SQL Injection Pocket Reference](https://websec.ca/kb/sql_injection)
- [payloadbox/sql-injection-payload-list](https://github.com/payloadbox/sql-injection-payload-list)
- [PayloadsAllTheThings - SQL Injection](https://github.com/swisskyrepo/PayloadsAllTheThings/tree/master/SQL%20Injection)
- [PortSwigger — SQL injection](https://portswigger.net/web-security/sql-injection) — Interactive labs covering blind, error-based, and out-of-band SQLi.
- [sqlmap usage handbook](https://github.com/sqlmapproject/sqlmap/wiki/Usage)

### NoSQL Injection

- [GraphQL NoSQL Injection Through JSON Types](http://www.petecorey.com/blog/2017/06/12/graphql-nosql-injection-through-json-types/)
- [PayloadsAllTheThings - NoSQL Injection](https://github.com/swisskyrepo/PayloadsAllTheThings/tree/master/NoSQL%20Injection)
- [A NoSQL Injection Primer (MongoDB)](https://www.netsparker.com/blog/web-security/what-is-nosql-injection/)

### Command Injection

- [Potential command injection in resolv.rb](https://github.com/ruby/ruby/pull/1777)
- [payloadbox/command-injection-payload-list](https://github.com/payloadbox/command-injection-payload-list)
- [PayloadsAllTheThings - Command Injection](https://github.com/swisskyrepo/PayloadsAllTheThings/tree/master/Command%20Injection)
- [PortSwigger — OS command injection](https://portswigger.net/web-security/os-command-injection)

### ORM Injection

- [HQL for pentesters](http://blog.h3xstream.com/2014/02/hql-for-pentesters.html)
- [HQL : Hyperinsane Query Language](https://www.synacktiv.com/ressources/hql2sql_sstic_2015_en.pdf)
- [ORM2Pwn: Exploiting injections in Hibernate ORM](https://www.slideshare.net/0ang3el/orm2pwn-exploiting-injections-in-hibernate-orm)
- [ORM Injection (slides)](https://www.slideshare.net/simone.onofri/orm-injection)

### Template Injection (SSTI/CSTI)

- [PayloadsAllTheThings - Server Side Template Injection](https://github.com/swisskyrepo/PayloadsAllTheThings/tree/master/Server%20Side%20Template%20Injection)
- [Server-Side Template Injection: RCE for the Modern Web App](https://portswigger.net/research/server-side-template-injection) — James Kettle's original SSTI research and detection methodology.
- [XSS without HTML: Client-Side Template Injection with AngularJS](http://blog.portswigger.net/2016/01/xss-without-html-client-side-template.html)

### XXE — XML External Entity

- [XXE](https://phonexicum.github.io/infosec/xxe.html)
- [XML external entity (XXE) injection](https://portswigger.net/web-security/xxe)
- [XML Schema, DTD, and Entity Attacks](https://www.vsecurity.com/download/publications/XMLDTDEntityAttacks.pdf)
- [payloadbox/xxe-injection-payload-list](https://github.com/payloadbox/xxe-injection-payload-list)
- [PayloadsAllTheThings - XXE Injection](https://github.com/swisskyrepo/PayloadsAllTheThings/tree/master/XXE%20Injection)

### CSRF — Cross-Site Request Forgery

- [Wiping Out CSRF](https://medium.com/@jrozner/wiping-out-csrf-ded97ae7e83f)
- [PayloadsAllTheThings - CSRF Injection](https://github.com/swisskyrepo/PayloadsAllTheThings/tree/master/CSRF%20Injection)
- [PortSwigger — CSRF](https://portswigger.net/web-security/csrf)
- [OWASP CSRF Prevention Cheat Sheet](https://cheatsheetseries.owasp.org/cheatsheets/Cross-Site_Request_Forgery_Prevention_Cheat_Sheet.html)

### Clickjacking

- [Clickjacking](https://www.imperva.com/learn/application-security/clickjacking/)
- [X-Frame-Options: All about Clickjacking?](https://github.com/cure53/Publications/blob/master/xfo-clickjacking.pdf?raw=true)
- [PortSwigger — Clickjacking](https://portswigger.net/web-security/clickjacking)

### SSRF — Server-Side Request Forgery

- [SSRF bible. Cheatsheet](https://docs.google.com/document/d/1v1TkWZtrhzRLy0bYXBcdLUedXGb9njTNIJXa3u9akHM/edit)
- [PayloadsAllTheThings - Server-Side Request Forgery](https://github.com/swisskyrepo/PayloadsAllTheThings/tree/master/Server%20Side%20Request%20Forgery)
- [PortSwigger — SSRF](https://portswigger.net/web-security/ssrf)
- [A New Era of SSRF - Exploiting URL Parser in Trending Programming Languages!](https://www.blackhat.com/docs/us-17/thursday/us-17-Tsai-A-New-Era-Of-SSRF-Exploiting-URL-Parser-In-Trending-Programming-Languages.pdf)

### Web Cache Poisoning / Deception

- [Practical Web Cache Poisoning](https://portswigger.net/research/practical-web-cache-poisoning)
- [PayloadsAllTheThings - Web Cache Deception](https://github.com/swisskyrepo/PayloadsAllTheThings/tree/master/Web%20Cache%20Deception)
- [Bypassing Web Cache Poisoning Countermeasures](https://portswigger.net/research/bypassing-web-cache-poisoning-countermeasures)
- [PortSwigger — Web cache poisoning](https://portswigger.net/web-security/web-cache-poisoning)

### Request Smuggling

- [HTTP Desync Attacks: Request Smuggling Reborn](https://portswigger.net/research/http-desync-attacks-request-smuggling-reborn) — James Kettle's foundational modern research.
- [PortSwigger — HTTP request smuggling](https://portswigger.net/web-security/request-smuggling)
- [PayloadsAllTheThings - HTTP Request Smuggling](https://github.com/swisskyrepo/PayloadsAllTheThings/tree/master/HTTP%20Request%20Smuggling)
- [Browser-Powered Desync Attacks](https://portswigger.net/research/browser-powered-desync-attacks) — Client-side variant.

### Relative Path Overwrite

- [Large-scale analysis of style injection by relative path overwrite](https://blog.acolyer.org/2018/05/28/large-scale-analysis-of-style-injection-by-relative-path-overwrite/)
- [MBSD Technical Whitepaper - A few RPO exploitation techniques](https://www.mbsd.jp/Whitepaper/rpo.pdf)

### Open Redirect

- [Open Redirect Vulnerability](https://s0cket7.com/open-redirect-vulnerability/)
- [payloadbox/open-redirect-payload-list](https://github.com/payloadbox/open-redirect-payload-list)
- [PayloadsAllTheThings - Open Redirect](https://github.com/swisskyrepo/PayloadsAllTheThings/tree/master/Open%20Redirect)

### Insecure Deserialization

- [What Do WebLogic, WebSphere, JBoss, Jenkins, OpenNMS, and Your Application Have in Common?](https://foxglovesecurity.com/2015/11/06/what-do-weblogic-websphere-jboss-jenkins-opennms-and-your-application-have-in-common-this-vulnerability/)
- [Attacking .NET deserialization](https://www.youtube.com/watch?v=eDfGpu3iE4Q)
- [.NET Roulette: Exploiting Insecure Deserialization in Telerik UI](https://www.youtube.com/watch?v=--6PiuvBGAU)
- [How to exploit the DotNetNuke Cookie Deserialization](https://pentest-tools.com/blog/exploit-dotnetnuke-cookie-deserialization/)
- [HOW TO EXPLOIT LIFERAY CVE-2020-7961](https://www.synacktiv.com/en/publications/how-to-exploit-liferay-cve-2020-7961-quick-journey-to-poc.html)
- [PayloadsAllTheThings - Insecure Deserialization](https://github.com/swisskyrepo/PayloadsAllTheThings/tree/master/Insecure%20Deserialization)
- [ysoserial](https://github.com/frohoff/ysoserial) — Tool for generating Java deserialization exploit payloads.
- [ysoserial.net](https://github.com/pwntester/ysoserial.net) — .NET equivalent.

### File Upload Vulnerabilities

- [File Upload Restrictions Bypass](https://www.exploit-db.com/docs/english/45074-file-upload-restrictions-bypass.pdf)
- [PayloadsAllTheThings - Upload Insecure Files](https://github.com/swisskyrepo/PayloadsAllTheThings/tree/master/Upload%20Insecure%20Files)
- [PortSwigger — File upload vulnerabilities](https://portswigger.net/web-security/file-upload)

### IDOR & Access Control

- [PayloadsAllTheThings - Insecure Direct Object References](https://github.com/swisskyrepo/PayloadsAllTheThings/tree/master/Insecure%20Direct%20Object%20References)
- [PortSwigger — Access control vulnerabilities](https://portswigger.net/web-security/access-control)
- [IDOR leads to account takeover](https://s0cket7.com/idor-leads-to-account-takeover/)
- [Autorize (Burp extension)](https://github.com/Quitten/Autorize) — Automates detection of authorization/IDOR flaws.

### Race Conditions

- [Smashing the state machine: the true potential of web race conditions](https://portswigger.net/research/smashing-the-state-machine) — James Kettle's deep dive on race condition exploitation.
- [PortSwigger — Race conditions](https://portswigger.net/web-security/race-conditions)
- [Turbo Intruder](https://github.com/PortSwigger/turbo-intruder) — Burp extension for high-throughput race condition testing.

### GraphQL Security

- [PayloadsAllTheThings - GraphQL](https://github.com/swisskyrepo/PayloadsAllTheThings/tree/master/GraphQL%20Injection)
- [OWASP GraphQL Cheat Sheet](https://cheatsheetseries.owasp.org/cheatsheets/GraphQL_Cheat_Sheet.html)
- [InQL](https://github.com/doyensec/inql) — Burp extension for GraphQL introspection and testing.
- [GraphQL NoSQL Injection Through JSON Types](http://www.petecorey.com/blog/2017/06/12/graphql-nosql-injection-through-json-types/)

### API Security (REST/gRPC)

- [OWASP API Security Top 10](https://owasp.org/www-project-api-security/)
- [Astra](https://github.com/flipkart-incubator/astra) — Automated security testing for REST APIs.
- [PayloadsAllTheThings - API](https://github.com/swisskyrepo/PayloadsAllTheThings/tree/master/API%20&%20Mobile%20Application)

---

## Identity, Auth & Standards

### OAuth / OpenID Connect

- [Introduction to OAuth 2.0 and OpenID Connect](https://pragmaticwebsecurity.com/courses/introduction-oauth-oidc.html)
- [What is going on with OAuth 2.0?](https://medium.com/securing/what-is-going-on-with-oauth-2-0-and-why-you-should-not-use-it-for-authentication-5f47597b2611)
- [Facebook OAuth Framework Vulnerability](https://www.amolbaikar.com/facebook-oauth-framework-vulnerability/)
- [PayloadsAllTheThings - OAuth Misconfiguration](https://github.com/swisskyrepo/PayloadsAllTheThings/tree/master/OAuth%20Misconfiguration)
- [The EvilRedirect / OAuth account takeover series](https://portswigger.net/daily-swig/oauth) — Ongoing coverage of OAuth-related bugs on The Daily Swig.

### JWT — JSON Web Tokens

- [Hardcoded secrets, unverified tokens, and other common JWT mistakes](https://r2c.dev/blog/2020/hardcoded-secrets-unverified-tokens-and-other-common-jwt-mistakes/)
- [PayloadsAllTheThings - JSON Web Token](https://github.com/swisskyrepo/PayloadsAllTheThings/tree/master/JSON%20Web%20Token)
- [jwt_tool](https://github.com/ticarpi/jwt_tool) — Toolkit for validating, forging, and cracking JWTs.
- [jwt.io](https://jwt.io/) — Debugger/decoder reference.

### SAML

- [How to Hunt Bugs in SAML; a Methodology - Part I](https://epi052.gitlab.io/notes-to-self/blog/2019-03-07-how-to-test-saml-a-methodology/)
- [How to Hunt Bugs in SAML; a Methodology - Part II](https://epi052.gitlab.io/notes-to-self/blog/2019-03-13-how-to-test-saml-a-methodology-part-two/)
- [How to Hunt Bugs in SAML; a Methodology - Part III](https://epi052.gitlab.io/notes-to-self/blog/2019-03-16-how-to-test-saml-a-methodology-part-three/)
- [PayloadsAllTheThings - SAML Injection](https://github.com/swisskyrepo/PayloadsAllTheThings/tree/master/SAML%20Injection)
- [SAMLExtractor](https://github.com/fadyosman/SAMLExtractor) — Extract SAML endpoints for testing.

### SSL/TLS

- [SSL & TLS Penetration Testing](https://www.aptive.co.uk/blog/tls-ssl-security-testing/)
- [Practical introduction to SSL/TLS](https://github.com/Hakky54/mutual-tls-ssl)
- [testssl.sh](https://github.com/drwetter/testssl.sh) — Command-line TLS/SSL configuration scanner.
- [SSL Labs Server Test](https://www.ssllabs.com/ssltest/) — Deep online analysis of any public TLS server.

---

## Framework & Platform Specific

### Rails

- [Rails Security - First part](https://hackmd.io/s/SkuTVw5O-)
- [Zen Rails Security Checklist](https://github.com/brunofacca/zen-rails-security-checklist)
- [Rails SQL Injection](https://rails-sqli.org)
- [Official Rails Security Guide](https://guides.rubyonrails.org/security.html)

### AngularJS / Angular

- [XSS without HTML: Client-Side Template Injection with AngularJS](http://blog.portswigger.net/2016/01/xss-without-html-client-side-template.html)
- [DOM based Angular sandbox escapes](http://blog.portswigger.net/2017/05/dom-based-angularjs-sandbox-escapes.html)
- [Angular Security Guide](https://angular.io/guide/security) — Official framework documentation on XSS/sanitization.

### React

- [XSS via a spoofed React element](http://danlec.com/blog/xss-via-a-spoofed-react-element)
- [dangerouslySetInnerHTML and common React XSS pitfalls](https://cheatsheetseries.owasp.org/cheatsheets/DOM_based_XSS_Prevention_Cheat_Sheet.html)

### WordPress & CMS

- [wpscan](https://github.com/wpscanteam/wpscan) — Black-box WordPress vulnerability scanner.
- [WPVulnDB / WPScan Vulnerability Database](https://wpscan.com/vulnerability-database) — Searchable WordPress CVE database.
- [JoomlaScan](https://github.com/drego85/JoomlaScan) — Component enumeration for Joomla.

### Webmail

- [Why mail() is dangerous in PHP](https://blog.ripstech.com/2017/why-mail-is-dangerous-in-php/)

---

## Infrastructure & Cloud

### AWS

- [PENETRATION TESTING AWS STORAGE: KICKING THE S3 BUCKET](https://rhinosecuritylabs.com/penetration-testing/penetration-testing-aws-storage/)
- [AWS PENETRATION TESTING PART 1. S3 BUCKETS](https://www.virtuesecurity.com/aws-penetration-testing-part-1-s3-buckets/)
- [AWS PENETRATION TESTING PART 2. S3, IAM, EC2](https://www.virtuesecurity.com/aws-penetration-testing-part-2-s3-iam-ec2/)
- [Misadventures in AWS](https://labs.f-secure.com/blog/misadventures-in-aws)
- [hacktricks — AWS Pentesting](https://cloud.hacktricks.wiki/en/pentesting-cloud/aws-security/index.html)
- [ScoutSuite](https://github.com/nccgroup/ScoutSuite) — Multi-cloud security auditing tool.
- [Prowler](https://github.com/prowler-cloud/prowler) — AWS/Azure/GCP security best-practices assessment.

### Azure

- [Common Azure Security Vulnerabilities and Misconfigurations](https://rhinosecuritylabs.com/cloud-security/common-azure-security-vulnerabilities/)
- [Cloud Security Risks (Part 1): Azure CSV Injection Vulnerability](https://rhinosecuritylabs.com/azure/cloud-security-risks-part-1-azure-csv-injection-vulnerability/)
- [MicroBurst](https://github.com/NetSPI/MicroBurst) — PowerShell toolkit for assessing Azure security.

### GCP

- [GCP Penetration Testing Tools & Techniques](https://cloud.hacktricks.wiki/en/pentesting-cloud/gcp-security/index.html)
- [GCPBucketBrute](https://github.com/RhinoSecurityLabs/GCPBucketBrute) — Enumerate GCP storage buckets and check permissions.

### NFS

- [NFS | PENETRATION TESTING ACADEMY](https://pentestacademy.wordpress.com/2017/09/20/nfs/)

### DNS Rebinding

- [Attacking Private Networks from the Internet with DNS Rebinding](https://medium.com/@brannondorsey/attacking-private-networks-from-the-internet-with-dns-rebinding-ea7098a2d325)
- [Hacking home routers from the Internet](https://medium.com/@radekk/hackers-can-get-access-to-your-home-router-1ddadd12a7a7)
- [Singularity of Origin](https://github.com/nccgroup/singularity) — Framework for developing DNS rebinding exploits.

---

## Reconnaissance

### Fingerprinting

- [Wappalyzer](https://www.wappalyzer.com/) — Technology stack fingerprinting for websites.
- [BuiltWith](https://builtwith.com/) — Web technology profiler.

### Sub-Domain Enumeration

- [A penetration tester's guide to sub-domain enumeration](https://blog.appsecco.com/a-penetration-testers-guide-to-sub-domain-enumeration-7d842d5570f6)
- [The Art of Subdomain Enumeration](https://blog.sweepatic.com/art-of-subdomain-enumeration/)
- [Certificate Search (crt.sh)](https://crt.sh/) — Search certificate transparency logs for subdomains.

### OSINT

- [Hacking Cryptocurrency Miners with OSINT Techniques](https://medium.com/@s3yfullah/hacking-cryptocurrency-miners-with-osint-techniques-677bbb3e0157)
- [OSINT x UCCU Workshop on Open Source Intelligence](https://www.slideshare.net/miaoski/osint-x-uccu-workshop-on-open-source-intelligence)
- [The most complete guide to finding anyone's email](https://www.blurbiz.io/blog/the-most-complete-guide-to-finding-anyones-email)
- [OSINT Framework](https://osintframework.com/) — Directory of OSINT tools organized by category.

---

## Cryptography

- [Applied Crypto Hardening](https://bettercrypto.org/)
- [What is a Side-Channel Attack?](https://www.csoonline.com/article/3388647/what-is-a-side-channel-attack-how-these-end-runs-around-encryption-put-everyone-at-risk.html)
- [Cryptopals Challenges](https://cryptopals.com/) — Hands-on crypto attack exercises.

## Web Shells & Post-Exploitation

- [Hunting for Web Shells](https://www.tenable.com/blog/hunting-for-web-shells)
- [Hacking with JSP Shells](https://blog.netspi.com/hacking-with-jsp-shells/)
- [GTFOBins](https://gtfobins.github.io/) — Unix binaries usable for post-exploitation privilege escalation.

---

## Browser Exploitation

### Frontend / Logic-Level

- [The world of Site Isolation and compromised renderer](https://speakerdeck.com/shhnjk/the-world-of-site-isolation-and-compromised-renderer)
- [The Cookie Monster in Your Browsers](https://speakerdeck.com/filedescriptor/the-cookie-monster-in-your-browsers)
- [Bypassing Mobile Browser Security For Fun And Profit](https://www.blackhat.com/docs/asia-16/materials/asia-16-Baloch-Bypassing-Browser-Security-Policies-For-Fun-And-Profit-wp.pdf)
- [The inception bar: a new phishing method](https://jameshfisher.com/2019/04/27/the-inception-bar-a-new-phishing-method/)
- [JSON hijacking for the modern web](http://blog.portswigger.net/2016/11/json-hijacking-for-modern-web.html)
- [SOP bypass / UXSS – Stealing Credentials Pretty Fast (Edge)](https://www.brokenbrowser.com/sop-bypass-uxss-stealing-credentials-pretty-fast/)
- [Setting arbitrary request headers in Chromium via CRLF injection](https://blog.bentkowski.info/2018/06/setting-arbitrary-request-headers-in.html)
- [Sending arbitrary IPC messages via overriding Function.prototype.apply](https://hackerone.com/reports/188086)
- [Take Advantage of Out-of-Scope Domains in Bug Bounty Programs](https://ahussam.me/Take-Advantage-of-Out-of-Scope-Domains-in-Bug-Bounty/)

### Engine / Native-Level

- [Breaking UC Browser](https://habr.com/en/company/drweb/blog/452076/)
- [Attacking JavaScript Engines - A case study of JavaScriptCore and CVE-2016-4622](http://www.phrack.org/papers/attacking_javascript_engines.html)
- [Three roads lead to Rome](http://blogs.360.cn/360safe/2016/11/29/three-roads-lead-to-rome-2/)
- [Exploiting a V8 OOB write](https://halbecaf.com/2017/05/24/exploiting-a-v8-oob-write/)
- [Look Mom, I don't use Shellcode - Browser Exploitation Case Study for IE11](https://labs.bluefrostsecurity.de/files/Look_Mom_I_Dont_Use_Shellcode-WP.pdf)
- [PUSHING WEBKIT'S BUTTONS WITH A MOBILE PWN2OWN EXPLOIT](https://www.thezdi.com/blog/2018/2/12/pushing-webkits-buttons-with-a-mobile-pwn2own-exploit)
- [A Methodical Approach to Browser Exploitation](https://blog.ret2.io/2018/06/05/pwn2own-2018-exploit-development/)
- [CVE-2017-2446 or JSC::JSGlobalObject::isHavingABadTime](https://doar-e.github.io/blog/2018/07/14/cve-2017-2446-or-jscjsglobalobjectishavingabadtime/)
- [CLEANLY ESCAPING THE CHROME SANDBOX](https://theori.io/research/escaping-chrome-sandbox)

---

## Evasion Techniques

### XXE Evasion

- [Evil XML with two encodings](https://mohemiv.com/all/evil-xml/)
- [Exploiting XXE with local DTD files](https://mohemiv.com/all/exploiting-xxe-with-local-dtd-files/)
- [Automating local DTD discovery for XXE exploitation](https://www.gosecure.net/blog/2019/07/16/automating-local-dtd-discovery-for-xxe-exploitation)
- [dtd-finder](https://github.com/GoSecure/dtd-finder) — Generate XXE payloads using local DTDs.

### CSP Bypasses

- [Any protection against dynamic module import?](https://github.com/w3c/webappsec-csp/issues/243)
- [CSP: bypassing form-action with reflected XSS](https://labs.detectify.com/2016/04/04/csp-bypassing-form-action-with-reflected-xss/)
- [Neatly bypassing CSP](https://lab.wallarm.com/how-to-trick-csp-in-letting-you-run-whatever-you-want-73cb5ff428aa)
- [Evading CSP with DOM-based dangling markup](https://portswigger.net/research/evading-csp-with-dom-based-dangling-markup)
- [GitHub's CSP journey](https://github.blog/2015-10-19-githubs-csp-journey/)
- [csp evaluator](https://csper.io/evaluator) — Automated tool for evaluating content-security-policies.

### WAF Evasion

- [Web Application Firewall (WAF) Evasion Techniques](https://medium.com/secjuice/waf-evasion-techniques-718026d693d8)
- [Web Application Firewall (WAF) Evasion Techniques #2](https://medium.com/secjuice/web-application-firewall-waf-evasion-techniques-2-125995f3e7b0)
- [Airbnb – When Bypassing JSON Encoding, XSS Filter, WAF, CSP, and Auditor turns into Eight Vulnerabilities](https://buer.haus/2017/03/08/airbnb-when-bypassing-json-encoding-xss-filter-waf-csp-and-auditor-turns-into-eight-vulnerabilities/)
- [How to bypass libinjection in many WAF/NGWAF](https://medium.com/@d0znpp/how-to-bypass-libinjection-in-many-waf-ngwaf-1e2513453c0f)

### JS Framework Sandboxes

- [JavaScript MVC and Templating Frameworks](http://www.slideshare.net/x00mario/jsmvcomfg-to-sternly-look-at-javascript-mvc-and-templating-frameworks)

### Authentication Bypass

- [Trend Micro Threat Discovery Appliance - Session Generation Authentication Bypass (CVE-2016-8584)](http://blog.malerisch.net/2017/04/trend-micro-threat-discovery-appliance-session-generation-authentication-bypass-cve-2016-8584.html)

---

## Notable Write-ups & Case Studies

- [Neat tricks to bypass CSRF-protection](https://zhuanlan.zhihu.com/p/32716181)
- [Exploiting CSRF on JSON endpoints with Flash and redirects](https://blog.appsecco.com/exploiting-csrf-on-json-endpoints-with-flash-and-redirects-681d4ad6b31b)
- [Stealing CSRF tokens with CSS injection (without iFrames)](https://github.com/dxa4481/cssInjection)
- [Cracking Java's RNG for CSRF](https://blog.securityevaluators.com/cracking-javas-rng-for-csrf-ea9cacd231d2)
- [If HttpOnly You Could Still CSRF… Of CORS you can!](https://medium.com/@_graphx/if-httponly-you-could-still-csrf-of-cors-you-can-5d7ee2c7443)
- [Clickjackings in Google worth $14,981.70](https://medium.com/@raushanraj_65039/google-clickjacking-6a04132b918a)
- [CVE-2019-1306: ARE YOU MY INDEX?](https://www.thezdi.com/blog/2019/10/23/cve-2019-1306-are-you-my-index)
- [WebLogic RCE (CVE-2019-2725) Debug Diary](https://paper.seebug.org/910/)
- [Exploiting Node.js deserialization bug for Remote Code Execution](https://opsecx.com/index.php/2017/02/08/exploiting-node-js-deserialization-bug-for-remote-code-execution/)
- [DRUPAL 7.X SERVICES MODULE UNSERIALIZE() TO RCE](https://www.ambionics.io/blog/drupal-services-module-rce)
- [How we exploited a remote code execution vulnerability in math.js](https://capacitorset.github.io/mathjs/)
- [GitHub Enterprise Remote Code Execution](http://exablue.de/blog/2017-03-15-github-enterprise-remote-code-execution.html)
- [Evil Teacher: Code Injection in Moodle](https://blog.ripstech.com/2018/moodle-remote-code-execution/)
- [How I Chained 4 vulnerabilities on GitHub Enterprise](http://blog.orange.tw/2017/07/how-i-chained-4-vulnerabilities-on.html)
- [$36k Google App Engine RCE](https://sites.google.com/site/testsitehacking/-36k-google-app-engine-rce)
- [Poor RichFaces](https://codewhitesec.blogspot.com/2018/05/poor-richfaces.html)
- [Remote Code Execution on a Facebook server](https://blog.scrt.ch/2018/08/24/remote-code-execution-on-a-facebook-server/)
- [Exploiting XSS with 20 characters limitation](https://jlajara.gitlab.io/posts/2019/11/30/XSS_20_characters.html)
- [Upgrade self XSS to Exploitable XSS in 3 Ways](https://www.hahwul.com/2019/11/upgrade-self-xss-to-exploitable-xss.html)
- [XSS without parentheses and semi-colons](https://portswigger.net/research/xss-without-parentheses-and-semi-colons)
- [XSS-Auditor — the protector of unprotected and the deceiver of protected](https://medium.com/bugbountywriteup/xss-auditor-the-protector-of-unprotected-f900a5e15b7b)
- [Query parameter reordering causes redirect page to render unsafe URL](https://hackerone.com/reports/293689)
- [How I found a $5,000 Google Maps XSS (by fiddling with Protobuf)](https://medium.com/@marin_m/how-i-found-a-5-000-google-maps-xss-by-fiddling-with-protobuf-963ee0d9caff)
- [DON'T TRUST THE DOM: BYPASSING XSS MITIGATIONS VIA SCRIPT GADGETS](https://www.blackhat.com/docs/us-17/thursday/us-17-Lekies-Dont-Trust-The-DOM-Bypassing-XSS-Mitigations-Via-Script-Gadgets.pdf)
- [Uber XSS via Cookie](http://zhchbin.github.io/2017/08/30/Uber-XSS-via-Cookie/)
- [DOM XSS – auth.uber.com](http://stamone-bug-bounty.blogspot.tw/2017/10/dom-xss-auth14.html)
- [Stored XSS on Facebook](https://opnsec.com/2018/03/stored-xss-on-facebook/)
- [XSS in Google Colaboratory + CSP bypass](https://blog.bentkowski.info/2018/06/xss-in-google-colaboratory-csp-bypass.html)
- [Another XSS in Google Colaboratory](https://blog.bentkowski.info/2018/09/another-xss-in-google-colaboratory.html)
- [$20000 Facebook DOM XSS](https://vinothkumar.me/20000-facebook-dom-xss/)
- [MySQL Error Based SQL Injection Using EXP](https://www.exploit-db.com/docs/english/37953-mysql-error-based-sql-injection-using-exp.pdf)
- [SQL injection in an UPDATE query - a bug bounty story!](http://zombiehelp54.blogspot.jp/2017/02/sql-injection-in-update-query-bug.html)
- [GitHub Enterprise SQL Injection](http://blog.orange.tw/2017/01/bug-bounty-github-enterprise-sql-injection.html)
- [Making a Blind SQL Injection a little less blind](https://medium.com/@tomnomnom/making-a-blind-sql-injection-a-little-less-blind-428dcb614ba8)
- [Red Team Tales 0x01: From MSSQL to RCE](https://www.tarlogic.com/en/blog/red-team-tales-0x01/)
- [SQL INJECTION AND POSTGRES - AN ADVENTURE TO EVENTUAL RCE](https://pulsesecurity.co.nz/articles/postgres-sqli)
- [AWS takeover through SSRF in JavaScript](http://10degres.net/aws-takeover-through-ssrf-in-javascript/)
- [SSRF in Exchange leads to ROOT access in all instances](https://hackerone.com/reports/341876)
- [PHP SSRF Techniques](https://medium.com/secjuice/php-ssrf-techniques-9d422cb28d51)
- [SSRF in imgur.com/vidgif/url](https://hackerone.com/reports/115748)
- [All you need to know about SSRF](https://www.auxy.xyz/web%20security/2017/07/06/all-ssrf-knowledge.html)
- [SSRF Tips](http://blog.safebuff.com/2016/07/03/SSRF-Tips/)
- [Into the Borg – SSRF inside Google production network](https://opnsec.com/2018/07/into-the-borg-ssrf-inside-google-production-network/)
- [Piercing the Veil: SSRF to NIPRNet access](https://medium.com/bugbountywriteup/piercing-the-veil-server-side-request-forgery-to-niprnet-access-c358fd5e249a)
- [ASP.NET resource files (.RESX) and deserialisation issues](https://www.nccgroup.com/uk/about-us/newsroom-and-events/blogs/2018/august/aspnet-resource-files-resx-and-deserialisation-issues/)
- [How I hacked Google's bug tracking system itself for $15,600](https://medium.com/free-code-camp/messing-with-the-google-buganizer-system-for-15-600-in-bounties-58f86cc9f9a5)
- [Some Tricks From My Secret Group](https://www.leavesongs.com/SHARE/some-tricks-from-my-secret-group.html)
- [Inducing DNS Leaks in Onion Web Services](https://github.com/epidemics-scepticism/writing/blob/master/onion-dns-leaks.md)
- [Stored XSS, and SSRF in Google using the Dataset Publishing Language](https://s1gnalcha0s.github.io/dspl/2018/03/07/Stored-XSS-and-SSRF-Google.html)

---

## Proof-of-Concept Databases

- [js-vuln-db](https://github.com/tunz/js-vuln-db) — Collection of JavaScript engine CVEs with PoCs.
- [awesome-cve-poc](https://github.com/qazbnm456/awesome-cve-poc) — Curated list of CVE PoCs.
- [Darkmoon](https://github.com/ASCIT31/Dark-Moon) - Open source (GPL-3.0) autonomous AI penetration testing platform for web, API, Active Directory and Kubernetes, with proof of exploitation.
- [Some-PoC-oR-ExP](https://github.com/coffeehb/Some-PoC-oR-ExP) — Collection of vulnerability PoCs/exploits.
- [uxss-db](https://github.com/Metnew/uxss-db) — Collection of UXSS CVEs with PoCs.
- [SPLOITUS](https://sploitus.com/) — Exploits & tools search engine.
- [Exploit Database](https://www.exploit-db.com/) — Archive of exploits, shellcode, and security papers.
- [Vulmon](https://vulmon.com/) — Vulnerability and exploit search engine with alerting.
- [Nuclei Templates](https://github.com/projectdiscovery/nuclei-templates) — Community-maintained YAML PoC templates for thousands of CVEs and misconfigurations.

## Cheat Sheets

- [XSS Cheat Sheet - 2018 Edition](https://leanpub.com/xss)
- [Capture the Flag CheatSheet](https://github.com/uppusaikiran/awesome-ctf-cheatsheet)
- [OWASP Cheat Sheet Series](https://cheatsheetseries.owasp.org/) — The canonical, actively maintained set of defensive cheat sheets.
- [PayloadsAllTheThings Methodology & Resources](https://github.com/swisskyrepo/PayloadsAllTheThings/blob/master/Methodology%20and%20Resources/README.md)
- [HackTricks Pentesting Web Methodology](https://book.hacktricks.wiki/en/pentesting-web/index.html)

---

## Tools

### All-in-One Platforms

- [Burp Suite](https://portswigger.net/burp/) — Integrated platform for web application security testing.
- [OWASP ZAP](https://www.zaproxy.org/) — Free, open-source web app scanner and intercepting proxy.
- [Caido](https://caido.io/) — Modern lightweight alternative to Burp Suite.

### Auditing

- [prowler](https://github.com/prowler-cloud/prowler) — Tool for cloud security assessment, auditing, and hardening.
- [slurp](https://github.com/hehnope/slurp) — Evaluate the security of S3 buckets.
- [A2SV](https://github.com/hahwul/a2sv) — Auto scanning for SSL vulnerabilities.

### Command Injection {#tools-command-injection}

- [commix](https://github.com/commixproject/commix) — Automated all-in-one OS command injection and exploitation tool.

### Reconnaissance Tools

- [Shodan](https://www.shodan.io/) — Search engine for internet-connected devices.
- [Censys](https://censys.io/) — Search engine for devices and networks on the internet.
- [urlscan.io](https://urlscan.io/) — Service that analyses websites and the resources they request.
- [ZoomEye](https://www.zoomeye.org/) — Cyberspace search engine.
- [FOFA](https://fofa.info/) — Cyberspace search engine.
- [Photon](https://github.com/s0md3v/Photon) — Fast crawler for OSINT.
- [FOCA](https://github.com/ElevenPaths/FOCA) — Fingerprinting Organizations with Collected Archives; metadata extraction.
- [SpiderFoot](https://github.com/smicallef/spiderfoot) — Open-source footprinting and intelligence-gathering tool.
- [xray](https://github.com/evilsocket/xray) — Recon, mapping, and OSINT gathering from public networks.
- [gitrob](https://github.com/michenriksen/gitrob) — Reconnaissance tool for GitHub organizations.
- [GSIL](https://github.com/FeeiCN/GSIL) — GitHub sensitive-information leak monitor.
- [ReconDog](https://github.com/s0md3v/ReconDog) — Reconnaissance swiss army knife.
- [tinfoleak](https://github.com/vaguileradiaz/tinfoleak) — Open-source tool for Twitter/X intelligence analysis.
- [Raccoon](https://github.com/evyatarmeged/Raccoon) — High-performance offensive recon and vulnerability-scanning tool.
- [Social Mapper](https://github.com/Greenwolf/social_mapper) — Social media enumeration and correlation tool.
- [Amass](https://github.com/owasp-amass/amass) — In-depth attack-surface mapping and asset discovery.
- [theHarvester](https://github.com/laramies/theHarvester) — Gather emails, subdomains, hosts, and names from public sources.

### Fuzzing

- [wfuzz](https://github.com/xmendez/wfuzz) — Web application bruteforcer.
- [ffuf](https://github.com/ffuf/ffuf) — Fast web fuzzer written in Go, widely used for directory/parameter fuzzing.
- [IPObfuscator](https://github.com/OsandaMalith/IPObfuscator) — Convert IPs to obfuscated formats for SSRF/filter bypass testing.
- [domato](https://github.com/googleprojectzero/domato) — DOM fuzzer.
- [FuzzDB](https://github.com/fuzzdb-project/fuzzdb) — Dictionary of attack patterns and primitives for fault injection.
- [dirhunt](https://github.com/Nekmo/dirhunt) — Web crawler optimized for analyzing site directory structure.
- [fuzz.txt](https://github.com/Bo0oM/fuzz.txt) — List of potentially dangerous filenames/paths.
- [SecLists](https://github.com/danielmiessler/SecLists) — The definitive collection of wordlists for fuzzing, brute-forcing, and payloads.

### Scanning

- [wpscan](https://github.com/wpscanteam/wpscan) — Black-box WordPress vulnerability scanner.
- [JoomlaScan](https://github.com/drego85/JoomlaScan) — Component enumeration for Joomla.
- [Nuclei](https://github.com/projectdiscovery/nuclei) — Fast, template-based configurable scanning engine.
- [Nikto](https://github.com/sullo/nikto) — Web server scanner for known vulnerabilities and misconfigurations.

### Penetration Testing Frameworks

- [TIDoS-Framework](https://github.com/theInfectedDrake/TIDoS-Framework) — Web application audit framework covering recon through exploitation.
- [Astra](https://github.com/flipkart-incubator/astra) — Automated security testing for REST APIs.
- [aws_pwn](https://github.com/dagrz/aws_pwn) — Collection of AWS penetration-testing scripts.
- [grayhatwarfare](https://buckets.grayhatwarfare.com/) — Searchable index of publicly exposed cloud storage buckets.
- [Metasploit Framework](https://github.com/rapid7/metasploit-framework) — General-purpose exploitation framework, widely used alongside web app testing.

### Secrets & Repo Leaking

- [HTTPLeaks](https://github.com/cure53/HTTPLeaks) — All possible ways a website can leak HTTP requests.
- [dvcs-ripper](https://github.com/kost/dvcs-ripper) — Rip web-accessible SVN/GIT/HG repositories.
- [GitMiner](https://github.com/UnkL4b/GitMiner) — Advanced mining for sensitive content on GitHub.
- [gitleaks](https://github.com/gitleaks/gitleaks) — Scan git history for secrets and keys.
- [trufflehog](https://github.com/trufflesecurity/trufflehog) — Find leaked credentials across git history and cloud storage.
- [snallygaster](https://github.com/hannob/snallygaster) — Scan for secret files exposed on HTTP servers.
- [LinkFinder](https://github.com/GerbenJavado/LinkFinder) — Discover endpoints inside JavaScript files.

### Offensive — By Vulnerability

**XSS**
- [beef](https://github.com/beefproject/beef) — Browser Exploitation Framework.
- [XSStrike](https://github.com/s0md3v/XSStrike) — Fuzzes/bruteforces parameters for XSS, detects and bypasses WAFs.
- [xssor2](https://github.com/evilcos/xssor2) — XSS'OR, hack with JavaScript.
- [Dalfox](https://github.com/hahwul/dalfox) — Fast parameter-analysis and XSS scanning tool.

**SQL Injection**
- [sqlmap](https://github.com/sqlmapproject/sqlmap) — Automatic SQL injection and database takeover tool.

**Template Injection**
- [tplmap](https://github.com/epinna/tplmap) — Server-side template injection detection/exploitation.

**XXE**
- [dtd-finder](https://github.com/GoSecure/dtd-finder) — List DTDs and generate XXE payloads.

**CSRF**
- [XSRFProbe](https://github.com/0xInfection/XSRFProbe) — CSRF audit and exploitation toolkit.

**SSRF**
- [Interactsh](https://github.com/projectdiscovery/interactsh) — Out-of-band interaction/detection tool for SSRF, XXE, blind RCE, etc.
- [Open redirect/SSRF payload generator](https://tools.intigriti.io/redirector/)

### Detection

- [retire.js](https://github.com/RetireJS/retire.js) — Scanner for JS libraries with known vulnerabilities.
- [malware-jail](https://github.com/HynekPetrak/malware-jail) — Sandbox for JavaScript malware analysis and deobfuscation.
- [repo-supervisor](https://github.com/auth0/repo-supervisor) — Scans code for misconfigurations, passwords, and secrets.
- [bXSS](https://github.com/LewisArdern/bXSS) — Simple blind-XSS collector application.
- [OpenRASP](https://github.com/baidu/openrasp) — Open-source runtime application self-protection.
- [Semgrep](https://github.com/semgrep/semgrep) — Fast static analysis for finding bugs and enforcing code standards.

### Prevention

- [DOMPurify](https://github.com/cure53/DOMPurify) — Super-fast, tolerant XSS sanitizer for HTML, MathML, and SVG.
- [js-xss](https://github.com/leizongmin/js-xss) — Sanitize untrusted HTML with a whitelist configuration.
- [Acra](https://github.com/cossacklabs/acra) — Client-side encryption engine for SQL databases with SQLi prevention.
- [Csper](https://csper.io) — Tools for building, evaluating, and monitoring content-security-policy.

### Proxies

- [Charles](https://www.charlesproxy.com/) — HTTP/HTTPS traffic monitor and reverse proxy.
- [mitmproxy](https://github.com/mitmproxy/mitmproxy) — Interactive, TLS-capable intercepting HTTP proxy.

### Web Shells

- [nano](https://github.com/s0md3v/nano) — Family of code-golfed PHP shells.
- [webshell](https://github.com/tennc/webshell) — Open-source webshell collection.
- [Weevely](https://github.com/epinna/weevely3) — Weaponized web shell.
- [reverse-shell](https://github.com/lukechilds/reverse-shell) — Reverse shell as a service.
- [PhpSploit](https://github.com/nil0x42/phpsploit) — Stealthy C2 framework persisting via a PHP oneliner.

### Disassemblers & Decompilers

- [radare2](https://github.com/radareorg/radare2) — Unix-like reverse-engineering framework and command-line tools.
- [Ghidra](https://github.com/NationalSecurityAgency/ghidra) — NSA's software reverse-engineering suite.
- [CFR](https://www.benf.org/other/cfr/) — Java decompiler.

### DNS Rebinding Tools

- [DNS Rebind Toolkit](https://github.com/brannondorsey/dns-rebind-toolkit) — Frontend JS framework for DNS rebinding exploits against LAN targets.
- [dref](https://github.com/mwrlabs/dref) — DNS rebinding exploitation framework.
- [Singularity of Origin](https://github.com/nccgroup/singularity) — Full toolkit for DNS rebinding attacks.
- [Whonow DNS Server](https://github.com/brannondorsey/whonow) — Malicious DNS server for on-the-fly rebinding attacks.

### Misc Tools

- [CyberChef](https://github.com/gchq/CyberChef) — The "Cyber Swiss Army Knife" for encoding, encryption, and data analysis.
- [ntlm_challenger](https://github.com/b17zr/ntlm_challenger) — Parse NTLM-over-HTTP challenge messages.

---

## Social Engineering

- [haveibeenpwned](https://haveibeenpwned.com/) — Check if your accounts appear in known data breaches.

## Blogs

- [Orange Tsai's blog](https://blog.orange.tw/)
- [leavesongs](https://www.leavesongs.com/)
- [James Kettle / PortSwigger Research](https://portswigger.net/research)
- [Broken Browser](https://www.brokenbrowser.com/)
- [BRETT BUERHAUS](https://buer.haus/)
- [n0tr00t](https://www.n0tr00t.com/)
- [OpnSec](https://opnsec.com/)
- [RIPS Technologies](https://blog.ripstech.com/)
- [Blog of Osanda](https://osandamalith.com/)
- [Detectify Labs](https://labs.detectify.com/)
- [Doyensec Blog](https://blog.doyensec.com/) — GraphQL, mobile, and application security research.
- [Assetnote Blog](https://blog.assetnote.io/) — Attack-surface research and bug bounty write-ups.

## Practice Platforms & CTFs

### General Web Application

- [OWASP Juice Shop](https://github.com/juice-shop/juice-shop) — Sophisticated, intentionally insecure modern web application.
- [BadLibrary](https://github.com/SecureSkyTechnology/BadLibrary) — Vulnerable web application for training.
- [Hackxor](https://hackxor.net/) — Realistic web application hacking game.
- [PortSwigger Web Security Academy](https://portswigger.net/web-security) — Free, extensive theory + labs covering nearly every vulnerability class.
- [PentesterLab](https://pentesterlab.com/) — Hands-on exercises across many vulnerability classes.
- [TryHackMe](https://tryhackme.com/) — Guided, beginner-friendly security learning paths.
- [Hack The Box](https://www.hackthebox.com/) — Practice labs and CTFs for offensive security.
- [Root Me](https://www.root-me.org/) — Large catalog of hands-on challenges by category.
- [DVWA (Damn Vulnerable Web Application)](https://github.com/digininja/DVWA) — Classic vulnerable PHP/MySQL app for learning basics.

### XSS Challenges

- [XSS game](https://xss-game.appspot.com/) — Google's XSS challenge.
- [prompt(1) to win](http://prompt.ml/) — 16-level XSS challenge with hidden levels.
- [alert(1) to win](https://alf.nu/alert1) — Series of XSS challenges.
- [XSS Challenges](http://xss-quiz.int21h.jp/) — Series of XSS challenges.

### Cloud (AWS/Azure/GCP)

- [FLAWS](http://flaws.cloud/) — AWS security CTF challenge.
- [flaws2](http://flaws2.cloud/) — Follow-up AWS challenge covering both attack and defense.
- [CloudGoat](https://github.com/RhinoSecurityLabs/cloudgoat) — "Vulnerable by design" AWS infrastructure deployment tool.
- [Sadcloud](https://github.com/nccgroup/sadcloud) — Deliberately misconfigured AWS infrastructure for scanner testing.

### ModSecurity / WAF Tuning

- [ModSecurity / OWASP CRS tutorials](https://www.netnea.com/cms/apache-tutorials/) — Series of tutorials to install, configure, and tune ModSecurity and the Core Rule Set.

## Bug Bounty Methodology

- [The Bug Hunters Methodology (all versions)](https://github.com/jhaddix/tbhm) — Jason Haddix's widely referenced recon-to-report methodology.
- [awesome-bug-bounty](https://github.com/djadmin/awesome-bug-bounty) — Curated list of bug bounty & disclosure programs plus write-ups.
- [bug-bounty-reference](https://github.com/ngalongc/bug-bounty-reference) — Bug bounty write-ups categorized by vulnerability type.
- [List of bug bounty writeups](https://pentester.land/list-of-bug-bounty-writeups.html) — Aggregated, searchable write-up index.
- [HackerOne Hacktivity](https://hackerone.com/hacktivity) — Live feed of disclosed bug bounty reports.
- [Bugcrowd University](https://github.com/bugcrowd/bugcrowd_university) — Free training material from Bugcrowd.

## Community

- [r/websecurity](https://www.reddit.com/r/websecurity/)
- [r/netsec](https://www.reddit.com/r/netsec/)
- [Stack Overflow — security tag](https://stackoverflow.com/questions/tagged/security)
- [Security StackExchange](https://security.stackexchange.com/)

## Miscellaneous

- [Google VRP and Unicorns](https://sites.google.com/site/bughunteruniversity/behind-the-scenes/presentations/google-vrp-and-unicorns)
- [Brute Forcing Your Facebook Email and Phone Number](http://pwndizzle.blogspot.jp/2014/02/brute-forcing-your-facebook-email-and.html)
- [The Definitive Security Data Science and Machine Learning Guide](http://www.covert.io/the-definitive-security-datascience-and-machinelearning-guide/)
- [notes](https://github.com/ChALkeR/notes) — Assorted public security notes.
- [A glimpse into GitHub's Bug Bounty workflow](https://github.blog/2016-05-24-a-glimpse-into-githubs-bug-bounty-program/)
- [Cybersecurity Campaign Playbook](https://www.belfercenter.org/CyberPlaybook)
- [Infosec_Reference](https://github.com/rmusser01/Infosec_Reference) — Broad information-security reference collection.
- [Internet of Things Scanner](http://iotscanner.bullguard.com/) — Check if home IoT devices are exposed on Shodan.
- [$7.5k Google services mix-up](https://sites.google.com/site/testsitehacking/-7-5k-Google-services-mix-up)
- [How I exploited ACME TLS-SNI-01 issuing Let's Encrypt SSL-certs for any domain using shared hosting](https://labs.detectify.com/2018/01/12/how-i-exploited-acme-tls-sni-01-issuing-lets-encrypt-ssl-certs-for-any-domain-using-shared-hosting/)
- [Escape and Evasion Egressing Restricted Networks](https://www.optiv.com/insights/source-zero/blog/escape-and-evasion-egressing-restricted-networks)
- [Be careful what you copy: Invisibly inserting usernames into text with Zero-Width Characters](https://medium.com/@umpox/be-careful-what-you-copy-invisibly-inserting-usernames-into-text-with-zero-width-characters-18b4e6f17b66)
- [CSS Is So Overpowered It Can Deanonymize Facebook Users](https://www.evonide.com/side-channel-attacking-browsers-through-css3-features/)
- [Finding The Real Origin IPs Hiding Behind CloudFlare or TOR](https://www.secjuice.com/finding-real-ips-of-origin-servers-behind-cloudflare-or-tor/)
- [How I could have stolen your photos from Google - my first 3 bug bounty writeups](https://blog.avatao.com/How-I-could-steal-your-photos-from-Google/)
- [WEB APPLICATION PENETRATION TESTING NOTES](https://techvomit.net/web-application-penetration-testing-notes/)
- [Hacking with a Heads Up Display](https://segment.com/blog/hacking-with-a-heads-up-display/)
- [The bug bounty program that changed my life](http://10degres.net/the-bug-bounty-program-that-changed-my-life/)
- [Implications of Loading .NET Assemblies](https://threatvector.cylance.com/en_us/home/implications-of-loading-net-assemblies.html)
- [How we abused Slack's TURN servers to gain access to internal services](https://www.rtcsec.com/2020/04/01-slack-webrtc-turn-compromise/)
- [How I got my first big bounty payout with Tesla](https://medium.com/heck-the-packet/how-i-got-my-first-big-bounty-payout-with-tesla-8d28b520162d)

## License

[CC0](https://creativecommons.org/publicdomain/zero/1.0/) — Public domain. Use, remix, and redistribute freely.



