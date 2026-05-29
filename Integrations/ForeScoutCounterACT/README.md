
# ForeScoutCounterACT

The Forescout device visibility platform provides insight into the diverse types of devices connected to your heterogeneous network—from campus and data center to cloud and operational technology networks. In other words, your extended enterprise. With one platform, you gain a consolidated view of traditional systems, mobile and IoT devices, virtual machines and cloud instances, and now, operational technology (OT) systems.

Python Version - 3
#### Parameters
|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|API Root||True|String|https://{ip address}|
|Username||True|String||
|Password||True|Password|*****|
|CA Certificate File||False|String||
|Verify SSL||False|Boolean|true|


#### Dependencies
| |
|-|
|certifi-2026.4.22-py3-none-any.whl|
|chardet-7.4.3-cp311-cp311-manylinux2014_x86_64.manylinux_2_17_x86_64.manylinux_2_28_x86_64.whl|
|charset_normalizer-3.4.7-cp311-cp311-manylinux2014_x86_64.manylinux_2_17_x86_64.manylinux_2_28_x86_64.whl|
|TIPCommon-1.0.10-py3-none-any.whl|
|requests-2.32.4-py3-none-any.whl|
|urllib3-2.6.3-py3-none-any.whl|
|idna-3.13-py3-none-any.whl|


## Actions
#### Enrich Entities
Enrich entities using information from ForeScout CounterACT. Supported entities: IP, Mac Address.
Timeout - 600 Seconds


|Name|Description|IsMandatory|Type|DefaultValue|
|----|-----------|-----------|----|------------|
|Create Insight|If enabled, action will create insights containing enrichment information.|False|Boolean|True|



##### JSON Results
```json
[{"Entity": "XXX.XX.XXX.XX", "EntityResult": {"ip": "XXX.XX.XXX.XX", "mac": "XXXXXXXXXXXX", "fields": {"nmap_banner7": [{"timestamp": "XXXXXXXXXXXX", "value": "XXXXXXXXXXXXXXXX"}, {"timestamp": "XXXXXXXXXXXX", "value": "XXXXXXXXXXXXXXXX"}], "classification_source_os": {"timestamp": "XXXXXXXXXXXX", "value": "XXXXXXXXXXXXXXXX"}, "onsite": {"timestamp": "XXXXXXXXXXXX", "value": "XXXXXXXXXXXXXXXX"}, "linux_manage": {"timestamp": "XXXXXXXXXXXX", "value": "XXXXXXXXXXXXXXXX"}, "access_ip": {"timestamp": "XXXXXXXXXXXX", "value": "XXXXXXXXXXXXXXXX"}, "classification_source_vendor": {"timestamp": "XXXXXXXXXXXX", "value": "XXXXXXXXXXXXXXXX"}, "openports": [{"timestamp": "XXXXXXXXXXXX", "value": "XXXXXXXXXXXXXXXX"}, {"timestamp": "XXXXXXXXXXXX", "value": "XXXXXXXXXXXXXXXX"}], "mac_vendor_string": {"timestamp": "XXXXXXXXXXXX", "value": "XXXXXXXXXXXXXXXX"}, "seen-appliances": [{"timestamp": "XXXXXXXXXXXX", "value": "XXXXXXXXXXXXXXXX"}], "cl_type": {"timestamp": "XXXXXXXXXXXX", "value": "XXXXXXXXXXXXXXXX"}, "fingerprint": {"timestamp": "XXXXXXXXXXXX", "value": "XXXXXXXXXXXXXXXX"}, "nmap_netfunc7": {"timestamp": "XXXXXXXXXXXX", "value": "XXXXXXXXXXXXXXXX"}, "flow_out_bps2": {"timestamp": "XXXXXXXXXXXX", "value": "XXXXXXXXXXXXXXXX"}, "agent_install_mode": {"timestamp": "XXXXXXXXXXXX", "value": "XXXXXXXXXXXXXXXX"}, "flow_out_bps1": {"timestamp": "XXXXXXXXXXXX", "value": "XXXXXXXXXXXXXXXX"}, "user_def_fp": {"timestamp": "XXXXXXXXXXXX", "value": "XXXXXXXXXXXXXXXX"}, "in-group": [{"timestamp": "0", "value": "XXXXXXXXXXXX"}, {"timestamp": "0", "value": "XXXXXX/XXXXX"}], "agent_visible_mode": {"timestamp": "XXXXXXX", "value": "XXXX"}, "classification_source_func": {"timestamp": "XXXXXXXXXXXX", "value": "XXXXXXXXXXXXXXXX"}, "samba_open_ports": {"timestamp": "XXXXXXXXXXXX", "value": "XXXXXXXXXXXXXXXX"}, "mac_prefix32": {"timestamp": "XXXXXXXXXXXX", "value": "XXXXXXXXXXXXXXXX"}, "wifi_client_login": {"timestamp": "XXXXXXXXXXXX", "value": "XXXXXXXXXXXXXXXX"}, "matched_fingerprints": [{"timestamp": "XXXXXXXXXXXX", "value": "XXXXXXXXXXXXXXXX"}, {"timestamp": "XXXXXXXXXXXX", "value": "XXXXXXXXXXXXXXXX"}], "macs": [{"timestamp": "XXXXXXXXXXXX", "value": "XXXXXXXXXXXXXXXX"}], "nmap_fp7": {"timestamp": "XXXXXXXXXXXX", "value": "XXXXXXXXXXXXXXXX"}, "os_classification": {"timestamp": "XXXXXXXXXXXX", "value": "XXXXXXXXXXXXXXXX"}, "flow_out_pktlen2": {"timestamp": "XXXXXXXXXXXX", "value": "XXXXXXXXXXXXXXXX"}, "flow_out_pktlen1": {"timestamp": "XXXXXXXXXXXX", "value": "XXXXXXXXXXXXXXXX"}, "mac": {"timestamp": "XXXXXXXXXXXX", "value": "XXXXXXXXXXXXXXXX"}, "cl_rule": {"timestamp": "XXXXXXXXXXXX", "value": "XXXXXXXXXXXXXXXX"}, "vendor": {"timestamp": "XXXXXXXXXXXX", "value": "XXXXXXXXXXXXXXXX"}, "manage_domain_strict": {"timestamp": "XXXXXXXXXXXX", "value": "XXXXXXXXXXXXXXXX"}, "gst_signed_in_stat": {"timestamp": "XXXXXXXXXXXX", "value": "XXXXXXXXXXXXXXXX"}, "misc": {"timestamp": "XXXXXXXXXXXX", "value": "XXXXXXXXXXXXXXXX"}, "prim_classification": {"timestamp": "XXXXXXXXXXXX", "value": "XXXXXXXXXXXXXXXX"}, "vendor_classification": {"timestamp": "XXXXXXXXXXXX", "value": "XXXXXXXXXXXXXXXX"}, "flow_out_idle2": {"timestamp": "XXXXXXXXXXXX", "value": "XXXXXXXXXXXXXXXX"}, "flow_out_idle1": {"timestamp": "XXXXXXXXXXXX", "value": "XXXXXXXXXXXXXXXX"}, "last_nbt_report_time": {"timestamp": "XXXXXXXXXXXX", "value": "XXXXXXXXXXXXXXXX"}, "agent_version": {"timestamp": "XXXXXXXXXXXX", "value": "XXXXXXXXXXXXXXXX"}, "manage_agent": {"timestamp": "XXXXXXXXXXXX", "value": "XXXXXXXXXXXXXXXX"}, "flow_out_pps2": {"timestamp": "XXXXXXXXXXXX", "value": "XXXXXXXXXXXXXXXX"}, "flow_out_pps1": {"timestamp": "XXXXXXXXXXXX", "value": "XXXXXXXXXXXXXXXX"}, "_times": [{"timestamp": "XXXXXXXXXXXX", "value": "XXXXXXXXXXXXXXXX"}], "local-credentials-OK": {"timestamp": "XXXXXXXXXXXX", "value": "XXXXXXXXXXXXXXXX"}, "online": {"timestamp": "XXXXXXXXXXXX", "value": "XXXXXXXXXXXXXXXX"}, "nmap_def_fp7": {"timestamp": "XXXXXXXXXXXX", "value": "XXXXXXXXXXXXXXXX"}, "ipv4_report_time": {"timestamp": "XXXXXXXXXXXX", "value": "XXXXXXXXXXXXXXXX"}, "nmap_def_fp5": {"timestamp": "XXXXXXXXXXXX", "value": "XXXXXXXXXXXXXXXX"}, "va_netfunc": {"timestamp": "XXXXXXXXXXXX", "value": "XXXXXXXXXXXXXXXX"}, "engine_seen_packet": {"timestamp": "XXXXXXXXXXXX", "value": "XXXXXXXXXXXXXXXX"}}, "id": "XXXXXXXXX"}}]
```



#### Ping
Test connectivity to the ForeScout CounterACT with parameters provided at the integration configuration page on the Marketplace tab.
Timeout - 600 Seconds









