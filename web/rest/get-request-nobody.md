while the HTTP protocol allows sending a BODY with GET, it should not have any semantics on the server, so this is not allowed in REST frameworks like RESTeasy, see also [the related SO answer](http://stackoverflow.com/a/983458/160799) referencing Roy Fielding, the inventor of REST.

You can build a GET request by hand in RESTeasy, but this will only give you an error: `RESTEASY004565: A GET request cannot have a body`
