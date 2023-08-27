# What is cdn?

1. It stands for content delivery network.
2. When you want to serve your FE apps to clients, serving from just a single server is not optimal as suppose you have a server running in india and client is trying to access your website from US then it will serve very slowly.
3. CDN solves this issue by basically deploying your FE app in what is called pop servers. These servers are installed in various locations throughout world, and whenever client will access your website, it will served from the nearest cdn server.
4. In AWS this is what Cloudfront does.