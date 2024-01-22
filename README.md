# 🅱️ Tracking (Fingerprinting) Domain Blocklists
Based on DuckDuckGo Tracker Radar
  
---
  
- Domain blocklists based on DDG Tracker Radar data.
- Blocks common domains hosting tracking/fingerprinting/advertising JS etc.
- Can be used adjacent to [Tracking (Fingerprinting) JS Blocklist](https://github.com/Zen-Initiative/Tracking-Fingerprinting-JS-Blocklist) that blocks specific scripts but not whole domains (more detail below)
  
---
  
#### Direct download links
Trackers_domain_blocklist.txt:  
[coming soon]  
  
Trackers_and_social_media_blocklist.txt:  
[coming soon]  
  
See below for differences.  
  
---
  
These domain blocklists are generated using DuckDuckGo Tracker Radar data (categorized trackers):   
[https://github.com/duckduckgo/tracker-radar/blob/main/build-data/static/categorized_trackers.csv](https://github.com/duckduckgo/tracker-radar/blob/main/build-data/static/categorized_trackers.csv)  

Two versions available:  
- ``` Trackers_domain_blocklist.txt``` blocks common domains hosting tracking/fingerprinting/advertising scripts etc.
- ``` Trackers_and_social_media_blocklist.txt``` additionally blocks social media domains (that host both regular content and tracking scripts etc.) and may also break social media share/comment functions on third-party websites
  
---
  
#### 🔐 Domain Inclusion/Exclusion
Domains are included based on DDG Tracker Radar categories:  
[https://github.com/duckduckgo/tracker-radar/blob/main/docs/CATEGORIES.md](https://github.com/duckduckgo/tracker-radar/blob/main/docs/CATEGORIES.md)  
  
The following categories are included in the blocklists: 
  
---
  
#### 🔓 Whitelisting & potential false positives
- Currently no whitelist is applied when generating the blocklists.
- You can create local exceptions to handle any false positives 
  
---
  
#### Using 🅱️ Domain Blocklist together with 🛡️ JS Blocklists
- The domain blocklists on this page will block whole domains (more suitable for DNS blocking, Pi-Hole blocklists, hosts files, etc.)
- The [JS Blocklists](https://github.com/Zen-Initiative/Tracking-Fingerprinting-JS-Blocklist) only blocks specific JS files (more suitable for uBO/ABP/AdGuard etc.)

It is recommended to use both lists together for more protection, as sometimes it is not possible to block the whole domains of popular websites (the entire websites will be blocked including all the content and functions), in which case the JS blocklists will kick in to block specific tracking/fingerprinting JS files hosted on these popular websites.  
  
---
  
## License
  
Creative Commons Zero v1.0 Universal ([https://github.com/Zen-Initiative/Tracking-Fingerprinting-Domain-Blocklists/blob/main/LICENSE](https://github.com/Zen-Initiative/Tracking-Fingerprinting-Domain-Blocklists/blob/main/LICENSE)  

  ---
  
