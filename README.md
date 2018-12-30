CORSProxy
==========

A simple forward proxy server for processing API calls to servers that don't send CORS headers or support HTTPS. Forked from https://github.com/Freeboard/thingproxy

### CORSProxy vs Thingproxy

CORSProxy is a fork of Thingproxy with additional documentation + in-deph configuration that will be maintained. You can read our feature list below.

### What is the point of CORSProxy

CORSProxy allows your site to access resources on other domains that would normally be blocked due to the same-origin policy. It acts as a proxy between your browser and a remote server and adds the proper CORS headers to the response.

### Installation

You must have Node.js and NPM installed on your server / computer first. 

To run locally, fork this repo into your server and run:

1. npm Install
2. npm Start

To run on an HTTPS / HTTP domain, follow same steps as above and install nginx and then refer to our NGINX.conf file for how to proxy pass it onto your domain.

Usage:

Once server is running you can make requests by the following:

```
https://myHTTPSdomain/fetch/APITOFETCH
```

### CORSPRoxy To-do
1. Config.json documentation + additional values to whitelist IP's, request URLS
2. Throttle requests and set max requests / s
3. Send specific headers depending on the request
