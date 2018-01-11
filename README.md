# LogProcessing

getForumTransaction and getForumTransactionObfusc are identical apart from setting of $obfuscate at the top.
This variable controls whether IP addresses and FQDNs are masked in the output.
It would be better if the obfuscation code was wrapped up into a function so that it wasn't repeated.

These scripts extract all the records for transactions matching the supplied argument from a Forum Sentry system log.

Obfuscation involves replacing the first two components of things that look like IP addresses with XXX.XXX and
the later domain components of GPN FQDNs with XXX.XXX.
