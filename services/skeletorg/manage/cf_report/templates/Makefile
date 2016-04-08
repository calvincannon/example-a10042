refresh:
	curl --silent https://raw.githubusercontent.com/cfengine/core/master/contrib/enterprise/report.pl -o report.pl.mustache
	sed -i 's/Hosts.HostName/Hosts.{{{vars.cf_report.query_host_id}}}/g' report.pl.mustache
