# Install and Setup OWASP Juice Shop
https://github.com/bkimminich/juice-shop

I suggest using the Docker set up. It works whereas the NPM ones gave me issues about where my XCode tools were stored. Might work better for any windows computers.  
The docker setup is easy to restart locally, but has the downside of not storing any flags on restart.

# Install Burp Suite Community
https://portswigger.net/burp/releases/professional-community-2020-2

Make sure to select community edition! Defaults to professional which you have to pay for.

If you have a mac, you'll probably see the following error:  
![Mac Burp Download Error](/images/burp_download_error.png)

To allow downloading, you'll have to go into System Preferences -> Security & Privacy -> bottom of the General tab, you'll have to allow it to download:  
![Enable Mac Burp Download](/images/enable_burp_download.png)

# Setup Burp Suite Proxy
I suggest using Firefox when using Burp Suite and downloading the [FoxyProxy Standard add-on](https://addons.mozilla.org/en-US/firefox/addon/foxyproxy-standard/?src=search). This allows you to turn the proxy on or off rather than having to remove it completely from system settings.

However, tthere are instructions for how to add it for different browsers and configurations: https://portswigger.net/burp/documentation/desktop/penetration-testing/configuring-your-browser

## Add the Burp Suite Certificate to Trusted Certs
In BurpSuite -> Proxy -> Options -> Import / Export CA certificate  
-> Export -> Certificate and private key in PKCS#12 keystore  
Add .p12 extension to whatever you give the file name  
Open Keychain Access (Applications -> Utilities or search Spotlight)  
-> File -> Import Items ~(may have to select options and change to all files)~

If you have a windows computer, hopefully this will help you: https://support.securly.com/hc/en-us/articles/360026808753-How-to-manually-install-the-Securly-SSL-certificate-on-Windows  
Or linux/windows: https://thomas-leister.de/en/how-to-import-ca-root-certificate/




