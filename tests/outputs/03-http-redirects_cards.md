# Knowledge Cards: HTTP 301 and 302 Redirects

> Source: 03-http-redirects.txt　3 cards
>
> Note: The source contains limited information, so only 3 distinct knowledge points were extracted; no cards were added to reach a higher count.

## Card 1: 301 Means a Permanent Move

- **Core knowledge**: A 301 status code ("Moved Permanently") tells the client that the original URL should no longer be used.
- **Explanation**: Because the move is permanent, clients may remember the new location on their own — browsers can cache a 301 so that later visits go straight to the new URL without contacting the server again.
- **Example / self-test**: Q: After a browser receives a 301, what may happen on subsequent visits to the original URL?

## Card 2: 302 Means a Temporary Redirect

- **Core knowledge**: A 302 status code ("Found") means the resource is temporarily elsewhere, while the original URL remains valid and should keep being requested.
- **Explanation**: Since the move is temporary, clients do not permanently remember the new location; they keep asking the original URL in case the resource returns.
- **Example / self-test**: Q: Why do browsers not permanently remember the new location after receiving a 302?

## Card 3: The Two Codes Are Treated Differently for SEO

- **Core knowledge**: A 301 generally signals that ranking signals such as link equity should be passed to the new URL, whereas a 302 usually does not pass them in the same way.
- **Explanation**: Search engines treat the redirect according to its permanence: a permanent move means the new URL inherits the old one's signals; a temporary move means the original URL is expected to return, so the signals stay with it.
- **Example / self-test**: Q: Which status code passes ranking signals to the new URL, and what is the reason given in the text?
