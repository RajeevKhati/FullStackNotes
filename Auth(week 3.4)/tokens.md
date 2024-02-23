# how server will know that its the right user?

1. After user signup or login, and user makes any subsequent request to the server, how would server know that this is the right user?
2. To make server recognize the user, one way is that user can send username, password in request headers to server and then server can validate this.
3. But this is security threat and its not a good practice to send username, password in headers.
4. So to avoid this scenario, we can make use of tokens.

# What are auth tokens?

1. When user signup or login, using this username, password server creates a token (JWT token).
2. This token is send as response to client.
3. Now Its client responsibilty to send this token with every subsequent requests.

# How it works?

1. When user is signing in or logging out, user will send username and password in object.
2. Then in backend, we will generate jwt token using a secret key and send this token in response.
3. Now when user will hit any authorized api, he/she will send this token in Authorization header as "Bearer token".
4. Now backend will decypher this token using that same secret key to get back the previously sent username and password object.
5. This is how token will be used to recognize the user.
