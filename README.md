orcidt2
=======

ORCID Tier 2 api framework

The purpose of this plugin is to provide a framework for working with the ORCID Tier 2 api.
The plugin does require a sandbox account which can be obtained for free. Use of the actual tier 2 api does require ORCID membership which is not free.

Config

It is necessary to configure this plugin before it will work.
1. Update the client id, secret and redirect uri In the file <repoid>cfg/cfg.d/z_orcid_credentials.pl
The id and the secret will be contained in the email you receive when you register to use the sandbox
The redirect uri will be the address you specified when you registered plus the path to the cgi script that will handle the ORCID callbacks (i.e. /cgi/orcid/auth)

2. The files <repoid>cfg/cfg.d/z_orcid.pl and <repoid>cfg/cfg.d/z_orcid_tier2.pl contain config that will add fields to the user dataset or allow you to map the orcid fields to your existing fields. In particular the field "orcid" is added to the user dataset and the doi and pubmed fields are mapped to the fields doi and pubmed_id in the eprint dataset.



