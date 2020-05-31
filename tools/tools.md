While trying to do the Plaid2020 CTF, I realized I was missing a lot of tools (or didn't know how to use the tools I had). This is to gather those tools, make them readily available to setup up my environment, and make sure I know how to use them at a moments notice. For now, this is mostly just a list of things I need. I'll make a reminder to add something to it once a week or month. Need to add when they'll be useful.

Some interesting topics to look for tools on github are `bugbounty`, `bug-bounty`, [`penetration-testing`](https://github.com/topics/penetration-testing), `pentest`, `hacking`, `security`, `infosec`

# List
- [Web Vulnerability Scanners](https://www.concise-courses.com/hacking-tools/web-vulnerability-scanners/)
- [Password Crackers](https://www.concise-courses.com/hacking-tools/password-crackers/)
- [Burp Suite](https://portswigger.net/burp/communitydownload)
  - [HTTP Request Smuggler](https://github.com/PortSwigger/http-request-smuggler)
- Proxy (MitM attack where I can read the requests and intercept, like BurpSuite, but live) - see Catalog challenge
- Site Mirrorer (maybe)
- Public S3 bucket tools
- [Payloads](https://github.com/swisskyrepo/PayloadsAllTheThings)
- [Debugging tools](https://www.concise-courses.com/hacking-tools/debuggers/)
- [Package Sniffers](https://www.concise-courses.com/hacking-tools/packet-sniffers/)
- [Web Proxy Hacking](https://www.concise-courses.com/hacking-tools/web-proxies/)
- [Web Browser Tools](https://www.concise-courses.com/hacking-tools/web-browser-related-tools/)
- [Port Scanner](https://www.concise-courses.com/hacking-tools/port-scanners/)
- [Vulnerability Scanners](https://www.concise-courses.com/hacking-tools/vulnerability-scanners/)
- Binary Decompilers: [Binary Ninja](https://binary.ninja/) (paid) & [Ghidra](https://ghidra-sre.org/) (free)

## [Burp Suite](https://portswigger.net/burp/communitydownload)
### [HTTP Request Smuggler](https://github.com/PortSwigger/http-request-smuggler)
#### How to Use
- Download the BurpSuite Extension (Extender -> BApp Store -> HTTP Request Smuggler)
- Grab the request you want to test (in proxy or repeater)
- Right click the request
- Select Launch Smuggle probe
- Follow [these instructions](https://github.com/PortSwigger/http-request-smuggler)

## [MitM Proxy](https://github.com/drk1wi/Modlishka)
- Allows `sslstrip` will remove TLS (if it's not protected with [HSTS](https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/Strict-Transport-Security)
- Can choose the domain you want to spoof and it’ll transparently grab the real site and serve it from your own domain
- Use in tandem with [Requestbin](https://requestbin.com/) or [ngrok](https://ngrok.com/)

## Public S3 Bucket Tools
- https://www.andreafortuna.org/2018/04/04/how-to-find-unsecured-s3-buckets-some-useful-tools/
- https://github.com/jordanpotti/AWSBucketDump
- https://github.com/swisskyrepo/PayloadsAllTheThings/tree/master/AWS%20Amazon%20Bucket%20S3

# Resources
- https://www.concise-courses.com/hacking-tools/top-ten/
- https://resources.infosecinstitute.com/category/certifications-training/ceh/ethical-hacking-tools/#gref
- https://github.com/zardus/ctf-tools
- https://medium.com/@int0x33/day-18-essential-ctf-tools-1f9af1552214
- https://resources.infosecinstitute.com/tools-of-trade-and-resources-to-prepare-in-a-hacker-ctf-competition-or-challenge/#gref
- https://awesomeopensource.com/projects/ctf-tools
- https://www.yeahhub.com/top-10-essential-ctf-tools-solving-reversing-challenges/ (Reverse Engineering Tools)
- https://trailofbits.github.io/ctf/forensics/
- https://apsdehal.in/awesome-ctf/
