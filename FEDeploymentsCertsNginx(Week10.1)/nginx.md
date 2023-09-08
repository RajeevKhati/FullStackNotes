# What is reverse Proxy?

1. whenever you hit a url in a browser suppose say google.com, it hits a default port of 80.(internally its google.com:80).

2. Now suppose we have an aws EC2 instance and we're running 2 apps here, one FE app on port 5173(default vite app running port) and one BE app on port 3000.

3. We want 100x.devs.com to hit port 5173 and api.100x.devs to hit 3000.

4. But in browser we know that if we 100x.devs.com it will resolve to 100x.dev.com:80.

5. So we will make our nginx run on port 80 and we will configure it to route to respective ports.

6. So here nginx is acting as a reverse proxy.

# Why is it called reverse proxy?

Forward proxy sits just after a request is made from browser, basically it takes the request.

But in case of reverse proxy it redirects request to a particular port in a machine.
