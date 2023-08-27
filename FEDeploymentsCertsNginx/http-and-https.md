# Why host websites on https instead of http

If a website is running on http, then request information made to that website (such as password, credit card info) can easily be intercepted using tools like WireShark.
But if a website is running on https, then request made to that website is completely encrypted and is less prone to information leaking.

# How to make BE server run on https?

By adding certificates.
It can be added using certbot(free tool) or can go to goDaddy and but certificates.
Then can add these certificates in server and point it using nginx.conf file.