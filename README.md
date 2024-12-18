# 📛 Tracking (Fingerprinting) Domain Blocklists
Based on DuckDuckGo Tracker Radar
  
---
  
- Domain blocklists based on DDG Tracker Radar data.
- Blocks common domains hosting tracking/fingerprinting/advertising JS etc.
- Can be used adjacent to [Tracking (Fingerprinting) JS Blocklist](https://github.com/Zen-Initiative/Tracking-Fingerprinting-JS-Blocklist) that blocks JS files but not whole domains (more detail below)
  
---
  
#### ⬇️ Direct links
**Trackers_domain_blocklist.txt**:  
[https://raw.githubusercontent.com/Zen-Initiative/Tracking-Fingerprinting-Domain-Blocklists/main/Trackers_domain_blocklist.txt](https://raw.githubusercontent.com/Zen-Initiative/Tracking-Fingerprinting-Domain-Blocklists/main/Trackers_domain_blocklist.txt)
  
**Trackers_and_social_media_blocklist.txt**:  
[https://raw.githubusercontent.com/Zen-Initiative/Tracking-Fingerprinting-Domain-Blocklists/main/Trackers_and_social_media_blocklist.txt](https://raw.githubusercontent.com/Zen-Initiative/Tracking-Fingerprinting-Domain-Blocklists/main/Trackers_and_social_media_blocklist.txt) 
  
Differences:  
- ```Trackers_domain_blocklist.txt``` blocks common domains hosting tracking/fingerprinting/advertising scripts etc.
- ```Trackers_and_social_media_blocklist.txt``` additionally blocks a few social media domains and may also break social media share/comment functions on some third-party websites; however, it doesn't block social media domains that are also used for federated login, CDN, and/or embedded content.

Currently, the differences between the two lists are very small.   
  
The first list (trackers only) is recommended for most users.  
  
---
  
#### 🔐 Domain Inclusion/Exclusion
These domain blocklists are generated using DuckDuckGo Tracker Radar data (categorized trackers):   
[https://github.com/duckduckgo/tracker-radar/blob/main/build-data/static/categorized_trackers.csv](https://github.com/duckduckgo/tracker-radar/blob/main/build-data/static/categorized_trackers.csv)  

Domains are selected based on DDG Tracker Radar categories:  
[https://github.com/duckduckgo/tracker-radar/blob/main/docs/CATEGORIES.md](https://github.com/duckduckgo/tracker-radar/blob/main/docs/CATEGORIES.md)  
  
The following categories are included (differences between the two blocklists are labeled with❗):  
  
|**Category**|**Trackers Domain Blocklist**|**Trackers & Social Media Blocklist**|
|---|---|---|
|**Ad Motivated Tracking**|:heavy_check_mark:|:heavy_check_mark:|
|**Advertising**|:heavy_check_mark:|:heavy_check_mark:|
|**Ad Fraud**|:heavy_check_mark:|:heavy_check_mark:|
|**Analytics**|:heavy_check_mark:|:heavy_check_mark:|
|**Audience Measurement**|:heavy_check_mark:|:heavy_check_mark:|
|**Federated Login**|:x:|:x:|
|**SSO**|:x:|:x:|
|**Third-Party Analytics Marketing**|:heavy_check_mark:|:heavy_check_mark:|
|**Social - Comment** (❗)|:x:|:heavy_check_mark:|
|**Social - Share** (❗)|:x:|:heavy_check_mark:|
|**Online Payment**|:x:|:x:|
|**Action Pixels**|:heavy_check_mark:|:heavy_check_mark:|
|**Unknown High Risk Behavior**|:heavy_check_mark:|:heavy_check_mark:|
|**Obscure Ownership**|:heavy_check_mark:|:heavy_check_mark:|
|**CDN**|:x:|:x:|
|**Badge**|:heavy_check_mark:|:heavy_check_mark:|
|**Embedded Content**|:x:|:x:|
|**Session Replay**|:heavy_check_mark:|:heavy_check_mark:|
|**Social Network** (❗)|:x:|:heavy_check_mark:|
|**Non-Tracking**|:x:|:x:|
|**Malware**|:heavy_check_mark:|:heavy_check_mark:|
|**Fraud Prevention**|:heavy_check_mark:|:heavy_check_mark:|
|**Consent Management Platform**|:heavy_check_mark:|:heavy_check_mark:|
|**Tag Manager**|:heavy_check_mark:|:heavy_check_mark:|
|**Support Chat Widget**|:x:|:x:|
  
  
---
  
#### 🔓 Whitelisting & potential false positives
- Currently no whitelist is applied when generating the blocklists.
- Create local exceptions if needed to handle any false positives 
  
---
  
#### Using 📛 Domain Blocklists together with 🛡️ JS Blocklists
- The domain lists block whole domains (for DNS blocking, Pi-Hole blocklists, hosts files, etc.)
- The [JS Blocklists](https://github.com/Zen-Initiative/Tracking-Fingerprinting-JS-Blocklist) only blocks specific JS files (for uBO/ABP/AdGuard etc.)

Use both lists together for more protection.  
  
Sometimes it is not possible to block the whole domains of popular websites (the entire websites will be blocked including all the content and functions), in which case the JS blocklists will kick in to block specific tracking/fingerprinting JS files hosted on these popular websites.  
  
---
  
## License
  
- This project: [Creative Commons Zero v1.0 Universal](https://github.com/Zen-Initiative/Tracking-Fingerprinting-Domain-Blocklists/blob/main/LICENSE)
- DuckDuckGo Tracker Radar data: [CC BY-NC-SA 4](https://creativecommons.org/licenses/by-nc-sa/4.0/). This repository is not endorsed by DuckDuckGo.
  
  ---
  
