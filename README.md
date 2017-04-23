# DD-WRT SNMP exporter configuration

This repostiory contains an artisanally handcrafted `snmp.yml` that can be used with
the Prometheus SNMP Exporter to scrape DD-WRT devices.

It's based on the `ddwrt` module the from prometheus/snmp_exporter#147 but adds support
for wireless client statistics that are hooked into the `unknown`, `.255.` part of the
UCD-SNMP-MIB tree by `wl_snmpd.sh`.
