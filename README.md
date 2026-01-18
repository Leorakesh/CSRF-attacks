# CSRF-attacks
Day 25 of 100 days challenge

Day 25 – Cross-Site Request Forgery (CSRF)
 Overview

On Day 25, I explored Cross-Site Request Forgery (CSRF), a web security vulnerability that tricks authenticated users into performing unintended actions on a web application without their knowledge. Since the victim is already logged in, the application trusts the request and executes it.

How CSRF Works

CSRF attacks exploit the trust a website has in a user’s browser. An attacker creates a malicious request and lures a logged-in victim into triggering it, often through a hidden link, image, or form submission.

For example:

Changing account details

Transferring funds

Resetting passwords

Deleting data

All without the user realizing what happened.

Key Learning Points

CSRF targets authenticated sessions.

Browsers automatically include cookies in requests.

Attackers abuse this behavior to send unauthorized commands.

Even a single click can compromise an account.

 Prevention Techniques

Implement CSRF tokens.

Use SameSite cookie attributes.

Verify Origin and Referer headers.

Require re-authentication for sensitive actions.

Avoid using GET requests for state-changing operations.
