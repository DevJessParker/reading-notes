# OAuth and Authorization

What is OAuth?
- Open-standard authorization protocol.

Give an example of what using OAuth would look like.
- Logging into GrubHub using your Facebook account.

How does OAuth work? What are the steps that it takes to authenticate the user?
- The first authentification provider verifies the user's credentials, and then the user authorizes secondary apps and website to allow access to those credentials without them being directly shared with the secondary apps. This is done via request and approved access tokens.

What is OpenID?
- A authorization program that allows a user to have one login for multiple websites.

## Authorization and Authentication Flows

What is the difference between authorization and authentication?
- Authentication verifies a user's identity. Authorization verifies the access a user gives other programs to piggyback on the original authentication.

What is Authorization Code Flow?
- A user is able to exchange an Authorization Code for an access token.

What is Authorization Code Flow with Proof Key for Code Exchange (PKCE)?
- A Code Verifier creates a Code Challenge, which is then sent over HTTPS to retrieve an Authorization Code. If intercepted, only the Authorization Code can be stolen, and a hacker cannot retrieve an access token without also having the Code Verifier.

What is Implicit Flow with Form Post?
- No longer considered best practice. used when applications are unable to securely store Client Secrets.

What is Client Credentials Flow?
- Systems authenticate other systems rather than authenticating a user.

What is Device Authorization Flow?
- Authorization that occurs via a link on a computer or smartphone to improve user experience when input is difficult to achieve without impacting UX.

What is Resource Owner Password Flow?
- Only used by highly trusted organizations. Uses forms to collect username and password.