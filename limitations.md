---
order: 99
icon: tools
label: Limitations
---

# Limitations

The ComicUpdates API service has limits on resources and request rates to ensure stability and prevent abuse. Only one account per IP address is allowed.

## Connection Requirements

The API supports HTTP/1.1, HTTP/2, and HTTP/3 over QUIC. SSL/TLS is required for secure connections. Requests must include a valid `User-Agent` header without spoofing. Multiple accounts from the same IP address are not allowed and may result in a blacklist.

## Rate Limits

There is a general limit of approximately 60 requests per second per Account. However, free accounts have a lower limit as detailed below:

==- Free Account Limits

The limit of free users are limited to 10 requests per second.

===

==- Paid Account Limits

Paid plan accounts receive the full 60 requests per second limit. Higher rates are possible by contacting sales@comicupdates.org.

===

==- Exceeding Limits

If you exceed the request limits, you may see error code 429 in the responses. Repeatedly going too far over could lead to your IP address being blocked with error code 403 or no response at all. The more you try to reconnect right away after a block, the longer you'll have to wait before accessing the API again. We have to enforce blocks and potential blacklisting in extreme cases where limits are ignored continuously, to maintain a stable experience for all users. Please get in touch if you need help understanding or working within the rate limits.

===
