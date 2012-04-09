json2gource
===========

This is a small perl script which converts JSON from http://dieren.vnurpa.ethylix.be/ to a CSV format
to be consumed by gource http://code.google.com/p/gource/

USAGE
-----
curl "http://dieren.vnurpa.ethylix.be/api/v1/document/?format=json" | perl json2gource

zcat test.json.gz | perl json2gource | gource --log-format custom -

LIMITATIONS
-----------
Currently limited to latin1 charset. Patches welcome.

