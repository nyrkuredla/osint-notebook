# OSINT Fundamentals.md

# Day 1
## Basic schedule
* Day 1: General OSINT resources, what is OSINT?, search engines, email addresses, username searching, reverse image search

* Day 2: Image analysis, geolocation, domain research, WHOIS, DNS queries, IP addresses

## Intro
* We store so much more information on the Internet now than on our computers
* What is OSINT? - idea of "openness" - information that is freely available on the Internet. These may be hidden behind user names/accounts, however. So instead of totally "open" - it's more "easily accessible/low barrier to entry" - you don't need to prove identity or pay or whatnot to get access to the data
* OSINT is also about analysis and figuring out why it's important/how it connects to other data - piecing together disparate pieces of information
* So: grabbing a whole bunch of data (images/text/documents/videos/TV broadcasts/newspapers) and examining it to answer questions
* Roots in older SIGINT techniques - analyzing radio broadcasts and etc. to answer important questions/deliver a final product

Using OSINT at work: there are roles that use it in a primary sense, but far more that use it in a secondary kind of way (recruiters, etc)
* Who else uses OSINT?
** Law enforcement
** Intelligence community
** Criminals/cartels!
** Recruiters
** Business intelligence/competitive intelligence
** Dating
** Scammers!

## What is OSINT?
_Doing a Google search is not OSINT. Gathering info is not OSINT. It is simply the first step._

Collection (raw data) > Machine analysis/crunching to contextualize, streamline, filter data (relevant info) > analysis and curation (why does this matter/how does it relate) > finished analysis/product
* Don't just give your client a dump of data. What does it mean? Why is it relevant? What are the action items from here?
* The intelligence is what makes OSINT, OSINT

Intelligence cycle - in military/intelligence organizations, an overarching guide for moving through a process of gathering and analyzing intelligence data
* See flowchart that Micah made! Sets a foundation to build on - not a step-by-step walkthrough, but a framework. Edit as needed!

## Overall OSINT Process
* In many cases, with transactional/professional OSINT work, start with a clean OSINT platform (clean VM, etc. - all brand new, no OSINT tools run on it ever, etc. - sometimes even a new computer entirely!)
** No way that operating system ID, etc. have been logged on the system. In most cases a clean VM will work fine
* _Acquire customer requirements_ - SUPER important. Also called "scoping". 
** Scope is vital because it enforces efficiency - reduces "rabbit holing" and helps stay on track answering the actual question and ultimately presenting information in a way that is relevant to the client
** "Look at all the work we did" isn't helpful to the client. What is actionable for them? What is the format that will be most useful for them to receive (Excel spreadsheet vs. Word doc….)? Status updates, etc?

### Digging In		
* Receive seed data from customer - and then pivot
* Taking notes throughout is vital - so you don't pivot yourself entirely away from the core goal/forget what you were doing and why
** Good documentation is absolutely critical! More on this in the next section
* Deliver briefing/report to client
* THEN, clean prior data, refine SOPs, update analysis platform with new tools, etc. Take just a little bit of time to refine process/document new tools/techniques, so you don't have to retread the same territory again in six months
** Again, documentation is key
** Also, updating your software is important - new versions of Firefox, Ubuntu, whatever is needed - this is a good time to do that

More on pivoting:
	• Griffin Glynns [blog post](https://hatless1der.com/advanced-osint-the-art-of-pivoting/)

### On Documentation
*DOCUMENTATION IS KEY.* If you are not documenting where you found information, when, how you got there, why you looked it up - it's going to be next to impossible to reconstruct it later
* Not to mention that social media, for example, is extremely changeable from day to day - Tweets get deleted, etc.
* Clients may follow up weeks/months later with questions - you must be able to explain completely how you got what you got/what you are claiming 
* Each page/image/video should have:
** Date of capture
** URL to resource (if applicable)
** Unique identifiers
** CITATION, in other words.
* That said, documentation is cumbersome, admittedly - but you CANNOT skip this step. Find a way that will work for you!
* Show your work - HOW did you get from one piece of data to another/from a group of data to a conclusion?

### Analysis!
How do you get a team with multiple people to collect and analyze data in a similar manner?
* Process
* Practice
** Be aware of cognitive biases (see Wikipedia!)
*** Cultural, sampling, biased sources...
** Collaboration
*** All members have to be on the same page
** Continuous learning
*** Work to minimize logical fallacies (survivorship, strawman, etc.)
*** Work to develop/apply _inductive_ reasoning

Suggestions to minimize bias:
* Consult others
* Write things down and ask "what's missing?"
* Note and investigate content that does NOT support your theory
* Ensure you have a variety of diverse sources
* Learn more about "good" analysis techniques - see resource list (Heuer, Jr. books)
* Write out your logic step by step to show your work. What isn't there that should be there? What are the gaps? Why did I think that…? Where is the evidence for this thing I'm assuming?

## Tools and Techniques
### Search engines!
* The best search engine is the one that gets you the results you want. Use a few to get better results/cover more ground
* Use search engine operators to your advantage; know them, love them
* Robots.txt file: a file that you can find at the beginning of almost every site out there - tells search engine webcrawlers what they can and cannot do/access on the site. Don't index these
* Tips:
** Make a keyword list and refine it
** Keywordtool.io - will spit out the top keywords/hashtags related to a term of your choosing
** Google Advanced Search, more below

### Google:
* Given limited time, let's deep-dive in Google. The other search engines are equally valuable to learn but take longer
* Advanced Search - results from a specific language/region, best to start here
* Trends - figure out what people are googling more frequently in a particular place/when
* Operators - see slide 45
* Search for emojis!! : Windows key + . In search engine
* Search for emoji on a certain site: "site:instagram.com 🥗🍵"
* See slide 47 for more info on emoji searches

### Usernames
* Targets likely have multiple usernames
* For each of them: try whatsmyname.app and/or NAMINT for variations
* Check the workflow on slide 59/Username Process tab
* *For what?* - useful to find other info to pivot on and profile data to harvest further

### Reverse Image Search:
* Use tools as needed! There are a ton of search engines, tools will make this easier
* Armin Sebastian's Search By Image browser extension (free!) is super useful
* Or github.com/dessant/search-by-image
* Lens.google.com and bing visual search can be helpful to find similar clothing, brands, etc.
	
Homework: slide 67 - some challenges
Thought: Reddit femalefashionadvice post - how does this work for finding similar clothes from e.g. Pinterest images? 

# Day 2
## Practice from yesterday
* Finding Twitter account using location and profile quote
* Finding which social media account is associated with an email address
* Skype names associated with an email address

## Image Analysis!
### Why important? What is it used for?
Verifying details, geolocation, identifying people... where are they, what are they doing, who are they with, when?

### Basic process
1. Look at the image
2. Note (preferably on paper by hand!) 10-20 things you can actually see
3. Prioritize things you can search on/look up
4. Search, analyze, repeat

Ben Strick - Australian analyst:
* Analyze foreground
* Analyze background
* Gather map markings
* Gather context from image posting
** Specifically used when there is a person involved who has, e.g., tweeted or posted something before/after - what is the social context?
* Analyze image metadata
** Last resort - often scraped out when posted - but great if you can get it

### Tools
* Google Earth (Bing, Yandex...) - Google Earth is particularly good and also free, also includes info about surrounding locations (where was the pic taken from?), tilt/rotation, etc.
* Google Maps
* Reverse image search, if you have a photo
* Exiftool (local; preferable to uploading images anywhere if working on something sensitive)
* Background removal: https://remove.bg (keep security in mind)
* Foreground removal: https://cleanup.pictures (ditto)

## Geolocation
Very quick primer - could literally spend hours on this

### Why geolocation?
* Corroboration of data
* Identifying normal habits (and deviations)
* Risk assessment
* Aftermath of national disaster, riots, war, etc.
* Locate missing people

### Tools and techniques
Lots in common with image analysis
* Terrain matching (e.g., with Google Earth)
* Peakfinder.org - combine with Google Earth to examine/identify mountains in the background
* Satellite imagery
* Image analysis
* https://geosocialfootprint.com - where are people tweeting from?
* socialbearing.com - analytics for Twitter accounts and handles - sentiment, type, source...
* Untappd! and other special-interest apps for whatever people are into and track their stats on. people sometimes tag each other in posts...
** Profiles and/or posts are often public by default on these apps.
** Aggregated data becomes much more powerful
*** can we see other info on other social media platforms of other places they went? Foursquare, Insta...
** What time are people drinking (can we then deduce, e.g., business hours, sleeping hours, etc.)? Where (airport bars, hotels, etc.)?
** untappd.osint.ninja - tool that aggregates Untappd data and shows trends

Biases and assumptions are really important to be aware of here - "looks like Amsterdam" does not mean Amsterdam!

## Geotagged content
Maybe you want to find emerging content in real-time from a particular location - for natural disasters, riots, terrorist events, etc. 
* Hashtags, locations, etc.
* Geo-tagged Snapchat Stories - map.snapchat.com
* twitter.com/explore - don't need an account
** near:city within:#km/mi
** geocode:lat,lon,#km/mi (you'd need to be luckier to get hits using this method, however)

## Domains
Custom domains can give us a lot of info - who owns it, how is it used, etc.

* WHOIS search
* DNS queries
* Search engine queries
* Computer infrastructure (shodan.io, censys.io, etc.)
* Website analysis

### WHOIS
Who owns which domains?
* I have a domain and want to figure out who owns it
** whoxy.com, viewdns.info RIPE, APNIC, ARIN
** Historical: whoxy > WHOIS History
** Registrar, dates of registration, possibly people data
* I have a name/company/etc. and I want to figure out what domain(s) they own
** reverse WHOIS lookup: whoxy.com, viewdns.info
** Domain(s), registrar(s), date(s) of registration
* I have a domain > I find out who owns it > what else do they own? > pivot
** Can use wildcard queries in e.g. viewdns.info - what domains have been registered with emails from a particular domain? Then do a regular lookup of those domains to narrow down which exact person registered it
*** people using their work/org email addresses to sign up for domains, etc. - also a foothold for social engineering, etc.

*Note:* GDPR restrictions make a lot of this a bit tricker now - but still good to know/check - there's still good information out there
* Keep in mind that different tools may have access to/care about different info - check multiple sites to cross-reference

### Network aggregation technique
* Instant Data Scraper tool to scrape viewdns.info - domain and registrar
* osintcombine.com - Data Visualization Tool - map generation
** CSV visualization directly in browser - useful for mapping mutual Facebook friends, etc. Good for seeing outliers, links...

### DNS Records
* A/AAAA - IPv4/IPv6
* NS (Name server) - can give more info re: business relationships - where is a domain hosted? If AWS, I know I should probably look for cloud infrastructure, etc.
* Mail exchange record (MX) - what is the email server of this domain? 
* Text (TXT) - validation, Sender Policy Framework (SPF), etc. - what past or current relationships do companies have? Which systems/addresses are allowed to send e-mails from a particular domain? (e.g., "this IP range is allowed to send e-mail from @bbc.co.uk")

### DNS Queries
* Retrieve common records (see above) - business relationships, pivots
* DNS enumeration - "do you have this?" - what's it being used for?
* Domain typosquatting - is there some variation in a domain that's similar to but not exactly the same as the target domain, used for phishing, etc.?

### Tools
* DNSDumpster.com - IP block owners, geolocation of associated IP addresses, NS/MX/TXT/A records, domain map
** business relationships, geolocation
** testing domains, more about infrastructure/tools (ooh, they use or have used Concur/Cisco/GCP/Atlassian/Dropbox...)
*** Keep in mind that DNS info is not necessarily current - dig through and see what gems you can find (Instant Data Scraper tool!!)
* Host.io - DNS info, what's on the website?, backlinks (who is sending links to this domain? malware, etc.), co-hosted domains (what else is hosted on the same IP address?)
* DNSTwist.it - Phishing domain scanner - looks for permutations on a domain name; where are they registered? 

## IP Addresses
Who is the owner? Can also use these for reverse DNS searches - what hostnames are associated with this IP?
* Org info, using a VPN or not, has it been used for malware?...geolocation with extreme caveats (VPNs are a thing, not exact, etc. - MIGHT be good for, e.g., ~50-100 mile radius or so) 
* https://securitytrails.com, https://builtwith.com, http://ipinfo.io















