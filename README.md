This is a chrome extension which inspects and find domains that don't resolve. This is primarily to help detect Second Order Subdomain Takeover. A second order subdomain takeover is when you're able to register a domain (expired, typoed, etc.) which are being referenced by some pages on some other domains. This may allow full or parital control over the page where the resource is being included/referenced. 

These are some resources on the very topic:    
https://edoverflow.com/2017/broken-link-hijacking/    
https://labs.detectify.com/2014/12/08/hijacking-of-abandoned-subdomains-part-2/    
https://shubs.io/high-frequency-security-bug-hunting-120-days-120-bugs/#secondorder    
https://hackernoon.com/how-i-hijacked-top-celebrities-tweets-including-katy-perry-shakira-fca3a0e751c6    
https://donald-trump.leadstories.com/3020957-belgian-hacker-hijacks-old-donald-trump-tweet-links-to-carnival-video.html    


And these are some relevant tools:    
https://github.com/jolle/expired-tweets    
https://github.com/mhmdiaa/second-order    
https://github.com/misterch0c/twitterBFTD    
https://github.com/stevenvachon/broken-link-checker

### Installation
1. Clone this repository
```
$ git clone https://github.com/1lastBr3ath/2ndOrder
```
2. Open chrome's extension page i.e. chrome://extensions
3. Enable Developer mode (slider on the top-right)
4. Click "Load upacked" and select the directory

### TODO
- Send email notification **
- Get publicsuffix list from cache, if possible (doesn't seem necessary)
- Avoid intercepting already scanned domains, if possible (doesn't seem necessary)
- Check response to determine if the requested domain is parked (need more data)
- Check for 1st order subdomain hijacking from domains listed in can-i-takeover-xyz (usefulness??)
- Add persistent notification or whatever ** (Stacked notifications, clicking opens all previously discovered results)
