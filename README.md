# 🅱️ Tracking (Fingerprinting) Domain Blocklists
Based on DuckDuckGo Tracker Radar
  
---
  
- Domain blocklists based on DDG Tracker Radar data.
- Blocks common domains hosting tracking/fingerprinting JS
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
