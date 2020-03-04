# Scanner 
This is a Pro feature, but it really doesn't help you much unless the vulnerable application is super interconnected. However, OWASP Zap seems to spider better (at least for Juiceshop).

Have a passive scanner running anyway as you're going through JuiceShop as it might find something that you don't. Make sure to scope to the application you want.

How to get the scanner flags:  
robots.txt -> /ftp  
robots.txt -> /ftp -> one of the files that has an error

# Target
Scoping! Makes it easier to get rid of all the Mozilla, Google, ad, etc. Removes random unncessary data from a lot of parts of the Burp Suite tool.

# Proxy
This feature is great for checking for client side validation, or XSS that you can't input into a page.

* If you're ever waiting for a page to load, check if your proxy is intercepting and you forgot ┬─┬ノ( º _ ºノ)

The HTTP history makes it so that you can retry a request that passed through the proxy or mutate it. Filtering allows you to search through the whole massive history making it easier to find the request you're looking for. Oh, yeah, the filtering is a button that brings down a drop down.

# Intruder
Where you need to enumerate on data or multiple data sets. I hardly ever use this as most of the work I'm doing requires hands on mutations, but I could see it being useful for trying multiple XSS on multiple fields.

# Repeater
http://localhost:3000/#/contact -> captcha

# Sequencer
Gonna be honest, I have no idea what this does. Never used it. Maybe we can find a use for it tonight!

# Decoder
Locally allows you to encode/decode things rather than having to go to a site. Super useful because you can send encodings or text from requests being sent through.  
-> http://localhost:3000/#/photo-wall -> #german -> src (Open in a new tab) -> URL encode the #  
* Can't encode only portions like symbols and sometimes this is how applications will "accidentally" block hackers: they're looking for field "abc", but the hacker URL encoded the whole thing so the application returns an error because it never found that field

# Comparer
If you're dyslexic, this will be your best friend. You can compare text files by bytes or words and it'll mark differences in easy to see colors. I use this frequently. Especially when I had two requests react differently, and I can't see the difference. Again it's possible to send portions of a request from other parts of Burp Suite. You can also store multiple files / lines to compare.

# Extender
Recently, it was found out that F5 (network bla-deda) had a vulnerability where you could send some bad data and it would desynchronize from the client and lead to request smuggling. Our awesome hacker who found this created a Burp Suite extension, because boy was it impossible to reproduce.
