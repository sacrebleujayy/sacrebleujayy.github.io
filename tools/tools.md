While trying to do the Plaid2020 CTF, I realized I was missing a lot of tools (or didn't know how to use the tools I had). This is to gather those tools, make them readily available to setup up my environment, and make sure I know how to use them at a moments notice. For now, this is mostly just a list of things I need. I'll make a reminder to add something to it once a week or month. Need to add when they'll be useful.

# LIST
- HTTP Request Smuggler ()
- Proxy (MitM attack where I can read the requests and intercept, like BurpSuite, but live) - see Catalog challenge
- Site Mirrorer (maybe)

## [HTTP Request Smuggler](https://github.com/PortSwigger/http-request-smuggler)

### How to Use
- Download the BurpSuite Extension (Extender -> BApp Store -> HTTP Request Smuggler)
- Grab the request you want to test (in proxy or repeater)
- Right click the request
- Select Launch Smuggle probe
- Follow [these instructions](https://github.com/PortSwigger/http-request-smuggler)

## [MitM Proxy](https://github.com/drk1wi/Modlishka)
- Allows `sslstrip` will remove TLS (if it's not protected with [HSTS](https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/Strict-Transport-Security)
- Can choose the domain you want to spoof and it’ll transparently grab the real site and serve it from your own domain
- Use in tandem with [Requestbin](https://requestbin.com/) or [ngrok](https://ngrok.com/)
