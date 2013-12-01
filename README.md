Page Render Relocate Assets
===========================

Idea is quite simple: the module just hooks after page render and alters generated markup, converting any requests to /site/assets/ to another URL specified via module settings. Just to be on the safe side this (at the moment) only alters requests that start with a double quote and /site/assets, ie. "... src="/site/assets/..." would get replaced, while "Look at my /site/assets/!" or "... src="http://example.com/site/assets/..." wouldn't. 


WARNING: this ProcessWire module is a proof of concept, not something you should
use or even install in a production environment. See this thread for context:
http://processwire.com/talk/topic/4127-can-assets-folder-be-moved-to-another-domainsubdomain/

This module is a proof of concept for dynamically altering location of
ProcessWire assets to point to another domain and/or subdomain specifically
configured to serve static content.

http://www.ravelrumba.com/blog/static-cookieless-domain/ explains why this can
be a good idea and how to setup such a domain yourself.
