jsh
===

Bash wrapper for SSH. Resolves a full FQDN based on a set of DNS suffixes, then determines connectivity to SSH ports.
Two conf files are involved with jsh:

**etc/dns_suffixes.conf**
: This file contains a list of all dns suffixes you will use. For example, if you wanted to look up mybox.localdomain.com, you would place .localdomain.com in this file and run 'jsh mybox'.
**etc/ssh_ports.conf**
: This file indicates which ports it should check to see are open. This is in order, so if you want an optional port checked before the standard SSH port, place it earlier in the file.
