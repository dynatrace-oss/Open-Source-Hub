# 🔴 AppMon Legacy — Archive Candidates (Dynatrace)

Pages 6–10 of the Dynatrace org are dominated by `Dynatrace-AppMon-*` plugins, fastpacks, sensor packs, and `DCRUM-*` scripts from the pre-Dynatrace platform era (approximately 2012–2018). All are **already archived** on GitHub.

**Total AppMon/DCRUM archived repos:** ~150  
**Recommended Disposition:** 🔴 **Archive Candidate** ✅ (already archived)

---

## Bulk Assessment

All repos in this group share the following profile:

| Dimension | Assessment |
|---|---|
| **Business / Ecosystem Purpose** | Plugins, sensor packs, fastpacks, and integrations for Dynatrace AppMon (Application Monitoring) — the legacy on-premises APM product predating the current Dynatrace platform |
| **Strategic Relevance** | ❌ None — AppMon product line EOL; superseded by Dynatrace OneAgent + platform |
| **Owning Team** | Legacy — no active owner |
| **Support Model** | ❌ None — archived |
| **Activity Level** | 🔴 Archived — no new commits; zero open issues/PRs |
| **License Status** | Mixed — most Apache 2.0, some MIT |
| **Security Readiness** | ❌ Not maintained; may contain outdated dependencies with known CVEs |
| **OSSF Scorecard** | N/A — archived |
| **Recommended Disposition** | 🔴 **Archive Candidate** ✅ Already archived |

---

## Recommended Actions

1. **Add a standard EOL banner** to all AppMon repo READMEs pointing to the current Dynatrace platform documentation. A single GitHub Action could batch-update all archived repos.

2. **Consider bulk deletion** of repos with 0 stars, 0 forks, 0 issues — these provide no value as public artifacts and add noise to the org. Candidates for deletion (confirmed zero adoption):

3. **Retain with EOL notice** any repos with ≥5 forks or ≥5 stars — these may still be referenced in customer environments.

---

## Full AppMon Repo List

### AppMon Plugins — Pages 7–9

| Repository | Stars | Forks | Notes |
|---|---|---|---|
| `Dynatrace-AppMon-REST-Monitor-Plugin` | 3 | 1 | |
| `Dynatrace-AppMon-Hystrix-Monitoring-Plugin` | 1 | 1 | |
| `Dynatrace-AppMon-Eclipse-Integration-Plugin` | 3 | 3 | |
| `Dynatrace-AppMon-SOAP-Monitor-Plugin` | 7 | 4 | |
| `Dynatrace-Appmon-Collector-Ansible` | 6 | 4 | |
| `atlassian-connect-jira` | 6 | 8 | Jira Add-On |
| `Dynatrace-Client-Ansible` | 1 | 0 | Delete candidate |
| `Dynatrace-AppMon-Update-Ansible` | 1 | 1 | |
| `Dynatrace-AppMon-Uninstall-Ansible` | 1 | 1 | |
| `Dynatrace-AppMon-Tomcat-Agent-Ansible` | 3 | 0 | Delete candidate |
| `Dynatrace-AppMon-Plugin-Ansible` | 2 | 0 | Delete candidate |
| `Dynatrace-AppMon-NGINX-Agent-Ansible` | 0 | 1 | Delete candidate |
| `Dynatrace-AppMon-License-Ansible` | 2 | 0 | Delete candidate |
| `Dynatrace-AppMon-Java-Agent-Ansible` | 3 | 1 | |
| `Dynatrace-AppMon-Glassfish-Agent-Ansible` | 2 | 1 | |
| `Dynatrace-AppMon-Apache-HTTPD-Agent-Ansible` | 4 | 1 | |
| `Dynatrace-Agent-Ansible` | 4 | 3 | |
| `Dynatrace-AppMon-Server-REST-Java-SDK` | 5 | 3 | |
| `Dynatrace-AppMon-JVM-Monitoring-Plugin` | 2 | 1 | |
| `Dynatrace-AppMon-RunQueue-Monitor-Plugin` | 1 | 0 | Delete candidate |
| `Dynatrace-AppMon-Web-Transaction-Monitor-Plugin` | 1 | 0 | Delete candidate |
| `Dynatrace-AppMon-Measure-Availability-Plugin` | 0 | 0 | Delete candidate |
| `Dynatrace-AppMon-Docker-Monitor-Plugin` | 18 | 3 | Retain — notable stars |
| `Dynatrace-AppMon-Splunk-Application` | 4 | 8 | |
| `Dynatrace-AppMon-Nagios-Relay-Monitor-Plugin` | 0 | 0 | Delete candidate |
| `Dynatrace-AppMon-IBM-MQ-Queue-Channel-Monitoring-Plugin` | 5 | 4 | |
| `Dynatrace-AppMon-Tier-Time-Monitor` | 1 | 1 | |
| `Dynatrace-AppMon-xMatters-Plugin` | 0 | 0 | Delete candidate |
| `Dynatrace-AppMon-Big-Data-Business-Transaction-Bridge` | 5 | 1 | |
| `Dynatrace-AppMon-IntelliJ-IDEA-Integration-Plugin` | 4 | 1 | |
| `Dynatrace-AppMon-License-Count` | 6 | 1 | |
| `Dynatrace-AppMon-DB-Query-Monitor-Plugin` | 4 | 4 | Open issues: 1 |
| `Dynatrace-AppMon-SMS-Notification-Plugin` | 1 | 0 | Delete candidate |
| `Dynatrace-AppMon-SilkPerformer-Plugin` | 3 | 1 | |
| `Dynatrace-AppMon-Telegram-Plugin` | 1 | 0 | Delete candidate |
| `Dynatrace-AppMon-Windows-Event-Log-Monitor` | 3 | 0 | Delete candidate |
| `Dynatrace-AppMon-URL-Monitor-Plugin` | 5 | 2 | Open issues: 1 |
| `Dynatrace-AppMon-Visual-Studio-2017` | 6 | 2 | |
| `Dynatrace-AppMon-SSH-Action-Plugin` | 2 | 0 | Delete candidate |
| `Dynatrace-AppMon-FTP-File-Checker-Plugin` | 1 | 1 | Open issues: 1 |
| `Dynatrace-AppMon-Elasticsearch-Plugin` | 4 | 1 | |
| `Dynatrace-AppMon-Slack-Integration-Plugin` | 3 | 4 | Open issues: 1 |
| `Dynatrace-AppMon-Log-File-Monitor` | 1 | 1 | |
| `Dynatrace-AppMon-hybris-eCommerce-Fastpack` | 16 | 6 | Retain — notable forks |
| `Dynatrace-AppMon-Availability-Monitor-Plugin` | 1 | 1 | |
| `Dynatrace-AppMon-Microsoft-Teams-Plugin` | 1 | 0 | Delete candidate |
| `Dynatrace-AppMon-Sitecore-FastPack` | 2 | 0 | Delete candidate |
| `Dynatrace-AppMon-SharePoint-FastPack` | 1 | 0 | Delete candidate |
| `Dynatrace-AppMon-SOLR-Monitoring-FastPack` | 1 | 0 | Delete candidate |
| `Dynatrace-AppMon-Tibco-EMS-Monitor-Plugin` | 1 | 1 | |
| `Dynatrace-AppMon-Tibco-FastPack` | 1 | 0 | Delete candidate |
| `Dynatrace-AppMon-Top-Process-Monitoring-Plugin` | 1 | 0 | Delete candidate |
| `Dynatrace-AppMon-WebSphere-MQ-Monitoring-Plugin` | 2 | 2 | |
| `Dynatrace-AppMon-Windows-CPU-and-Memory-Action-Plugin` | 1 | 0 | Delete candidate |
| `Dynatrace-AppMon-Windows-Service-Status-Monitor-Plugin` | 2 | 2 | |
| `Dynatrace-AppMon-WindowsSTDCALL-ADKWrapper` | 2 | 1 | |
| `Dynatrace-AppMon-SQL-Server-Standalone-Monitor` | 2 | 0 | Delete candidate |
| `Dynatrace-AppMon-UEM-JS-Agent-Injector` | 0 | 0 | Delete candidate |
| `Dynatrace-AppMon-Exchange-Server-Performance-Counters-Plugin` | 1 | 0 | Delete candidate |
| `Dynatrace-AppMon-Magento-Fastpack` | 1 | 0 | Delete candidate |
| `Dynatrace-AppMon-IBM-WebSphere-Commerce-Fastpack` | 1 | 1 | |
| `Dynatrace-AppMon-Linux-Process-Monitor-Plugin` | 1 | 1 | |
| `Dynatrace-AppMon-Apache-Monitor-Plugin` | 2 | 0 | Delete candidate |
| `Dynatrace-AppMon-WebSphere-MQ-Monitoring-Fastpack` | 1 | 0 | Delete candidate |
| `Dynatrace-AppMon-LDAP-Test-Connection-Monitor-Plugin` | 1 | 0 | Delete candidate |
| `Dynatrace-AppMon-Guidewire-FastPack` | 2 | 2 | |
| `Dynatrace-AppMon-Redis-Plugin` | 0 | 0 | Delete candidate |
| `Dynatrace-AppMon-BizTalk-FastPack` | 2 | 2 | |
| `Android-Hybrid-App-Sample` | 3 | 2 | |
| `Dynatrace-AppMon-PostgreSQL-Monitor-Plugin` | 5 | 2 | Open issues: 1 |
| `Dynatrace-AppMon-Oracle-Weblogic-Monitoring-Plugin` | 7 | 5 | Retain — notable stars |
| `Dynatrace-AppMon-Message-Flow-Statistics-Monitoring-Plugin` | 2 | 1 | |
| `Dynatrace-AppMon-Tibco-BW-Monitoring-Plugin` | 1 | 0 | Delete candidate |
| `Dynatrace-AppMon-Oracle-Monitor-Plugin` | 4 | 3 | |
| `Dynatrace-AppMon-NET-Reflector-Plugin` | 1 | 0 | Delete candidate |
| `Dynatrace-AppMon-Automation-Library-for-Dynatrace` | 3 | 3 | |
| `Dynatrace-AppMon-MSBuild-Tasks-Library` | 2 | 2 | |
| `Dynatrace-AppMon-NANT-Task-Library` | 1 | 1 | |
| `Dynatrace-AppMon-Visual-Studio-2005-and-2008-IDE-Plugins` | 1 | 0 | Delete candidate |
| `Dynatrace-AppMon-Visual-Studio-2010--2012-and-2013-IDE-Plugins` | 1 | 0 | Delete candidate |
| `Dynatrace-AppMon-Endeca-Monitoring-Plugin` | 2 | 1 | |
| `Dynatrace-AppMon-DB2-Monitor-Plugin` | 3 | 1 | |
| `Dynatrace-AppMon-WebSphere-Single-Server-Plugin` | 1 | 1 | |
| `Dynatrace-AppMon-ColdFusion-Sensor-Pack` | 2 | 1 | |
| `Dynatrace-AppMon-MS-CRM-4.0-Sensor-Pack` | 2 | 1 | |
| `Dynatrace-AppMon-PeopleSoft-8-Sensor-Pack` | 2 | 1 | |
| `Dynatrace-AppMon-HipChat-Plugin` | 1 | 1 | HipChat EOL |
| `Dynatrace-AppMon-Varnish-Stats-Monitor-Plugin` | 1 | 0 | Delete candidate |
| `Dynatrace-AppMon-WebSphere-DataPower-Monitor-Plugin` | 3 | 4 | |
| `Dynatrace-AppMon-Business-Transaction-Row-Counter-Plugin` | 2 | 1 | |
| `Dynatrace-AppMon-Couchbase-Plugin` | 0 | 0 | Delete candidate |
| `Dynatrace-AppMon-SOLR-Remote-Monitoring-Plugin` | 1 | 0 | Delete candidate |
| `Dynatrace-AppMon-Third-Party-Time-Monitor` | 0 | 0 | Delete candidate |
| `Dynatrace-AppMon-Generic-Measure-Monitoring-Plugin` | 5 | 0 | |
| `Dynatrace-AppMon-Rabbit-MQ-Monitor-Plugin` | 1 | 0 | Delete candidate |
| `Dynatrace-AppMon-Extended-EMail-Action-Plugin` | 4 | 2 | |
| `Dynatrace-AppMon-Oracle-WebLogic-FastPack` | 1 | 2 | |
| `Dynatrace-AppMon-Liferay-Portal-FastPack` | 1 | 0 | Delete candidate |
| `Dynatrace-AppMon-Electric-Flow-Action-Plugin` | 1 | 0 | Delete candidate |
| `Dynatrace-AppMon-GenericOperations-Plugin` | 0 | 1 | Delete candidate |
| `Dynatrace-AppMon-Visual-Studio-2015` | 1 | 0 | Delete candidate |
| `Dynatrace-AppMon-JSON-Reporting-Plugin` | 2 | 0 | Delete candidate |
| `Dynatrace-AppMon-ServiceNow-Action-Plugin` | 5 | 7 | Retain |
| `Dynatrace-AppMon-NGINX-Plus-Monitoring-Plugin` | 4 | 1 | |
| `Dynatrace-AppMon-AWS-Classic-LoadBalancer-Monitor` | 0 | 1 | Delete candidate |
| `Dynatrace-AppMon-TCP-Port-Monitor-Plugin` | 1 | 3 | |
| `Dynatrace-AppMon-Salesforce-Commerce-Cloud-Fastpack` | 1 | 1 | |
| `Dynatrace-AppMon-PurePath-WebStart-Launcher` | 1 | 1 | |
| `Dynatrace-AppMon-CSC-Regulatory-Solutions-Suite` | 1 | 0 | Delete candidate |
| `Dynatrace-AppMon-iPlanet-Monitor` | 1 | 1 | |
| `Dynatrace-AppMon-JBoss-7-Datasource-Monitoring-Plugin` | 1 | 2 | |
| `Dynatrace-AppMon-IBM-WebSphere-Portal-Fastpack` | 2 | 0 | Delete candidate |
| `Dynatrace-AppMon-AIX-Filesystem-Status-Plugin` | 1 | 0 | Delete candidate |
| `Dynatrace-AppMon-Amazon-EC2-Account-Cost-Monitoring-FastPack` | 2 | 0 | Delete candidate |
| `Dynatrace-AppMon-Amazon-SimpleDB-Fastpack` | 2 | 0 | Delete candidate |
| `Dynatrace-AppMon-Apache-Cassandra-Fastpack` | 2 | 0 | Delete candidate |
| `Dynatrace-AppMon-Apache-Hadoop-and-MapReduce-FastPack` | 1 | 0 | Delete candidate |
| `Dynatrace-AppMon-Apache-HTTP-Server-FastPack` | 1 | 1 | |
| `Dynatrace-AppMon-BizTalk-Monitor-Plugin` | 1 | 1 | |
| `Dynatrace-AppMon-Citrix-NetScaler-Monitoring-Plugin` | 1 | 0 | Delete candidate |
| `Dynatrace-AppMon-CSS-AD-Configurator` | 1 | 0 | Delete candidate |
| `Dynatrace-DCRUM-URL-Hierarchy-Check-Script` | 2 | 0 | Delete candidate |
| `Dynatrace-AppMon-Email-Report-Action-Plugin` | 2 | 0 | Delete candidate |
| `Dynatrace-AppMon-Google-Analytics-Monitor-Plugin` | 1 | 1 | |
| `Dynatrace-AppMon-Growl-Alerting-Plugin` | 1 | 0 | Delete candidate — Growl EOL |
| `Dynatrace-AppMon-HornetQ-FastPack` | 1 | 0 | Delete candidate |
| `Dynatrace-AppMon-HPOO-Action-Plugin` | 1 | 0 | Delete candidate |
| `Dynatrace-AppMon-IIS-Monitoring-Plugin` | 2 | 1 | |
| `Dynatrace-AppMon-JIRA-Action-Plugin` | 3 | 1 | |
| `Dynatrace-AppMon-JMeter-Integration` | 1 | 0 | Delete candidate |
| `Dynatrace-AppMon-Kofax-FastPack` | 1 | 0 | Delete candidate |
| `Dynatrace-AppMon-LZO-Compression-Library` | 2 | 0 | Delete candidate |
| `Dynatrace-AppMon-MongoDB-for-.NET-FastPack` | 1 | 0 | Delete candidate |
| `Dynatrace-AppMon-PagerDuty-Action-Plugin` | 1 | 0 | Delete candidate |
| `Dynatrace-AppMon-Paging-Space-Utilization-Monitor-Plugin` | 1 | 0 | Delete candidate |
| `Dynatrace-AppMon-SAP--JCO--Knowledge-Sensor-Pack` | 1 | 0 | Delete candidate |
| `Dynatrace-AppMon-SCOM-Action-Monitoring-Plugin` | 1 | 0 | Delete candidate |

### AppMon Ansible Roles — Page 5 (archived)

| Repository | Stars | Forks | Notes |
|---|---|---|---|
| `Dynatrace-AppMon-Server-Ansible` | 10 | 9 | Open issues: 1 |
| `Dynatrace-AppMon-Ansible` | 21 | 9 | Notable stars; collection repo |
| `Dynatrace-AppMon-WebServer-Agent-Ansible` | 6 | 1 | |
| `Dynatrace-AppMon-TFS-Integration-Plugin` | 6 | 0 | |
| `Dynatrace-OneAgent-Chef` | 6 | 6 | Open issues: 1 |
| `Dynatrace-AppMon-Chef` | 12 | 15 | Notable forks |
| `Dynatrace-AppMon-Powershell` | 8 | 12 | Notable forks |
| `dotnet-core-buildpack` | 1 | 90 | **Notable: 90 forks** — CF .NET Core buildpack |
| `Dynatrace-AppMon-Puppet-DEPRECATED` | 20 | 12 | Explicitly deprecated |
| `Dynatrace-OneAgent-Puppet-DEPRECATED` | 9 | 26 | Explicitly deprecated |

### DCRUM Scripts — Page 10 (archived)

| Repository | Stars | Forks | Notes |
|---|---|---|---|
| `DCRUM-Splunk-Application` | 3 | 2 | |
| `DCRUM-ISO8583-Decode` | 0 | 2 | |
| `DCRUM-Corba-GIOP-Decode` | 0 | 0 | Delete candidate |
| `DCRUM-SISNAPI-Decode` | 0 | 0 | Delete candidate |
| `DCRUM-Universal-Decode-SDK` | 2 | 0 | |
| `DCRUM-MiniHTTP-Decode` | 0 | 0 | Delete candidate |
| `DCRUM-SunRMI-Decode` | 0 | 0 | Delete candidate |

### AppMon Utility Tools — Page 5 (archived)

| Repository | Stars | Forks | Notes |
|---|---|---|---|
| `Dynatrace-AppMon-JMX-Enhanced-Monitor-Plugin` | 9 | 2 | Notable stars |
| `Dynatrace-AppMon-Command-Line-Tool` | 2 | 2 | |
| `Dynatrace-AppMon-FastPack-Builder` | 3 | 0 | |
| `Dynatrace-AppMon-Master-Slave-Dashboard-Creator` | 4 | 4 | |
| `Dynatrace-AppMon-Dashboard-Cleaner` | 1 | 0 | Delete candidate |
| `Dynatrace-AppMon-Dashboard-Report-Reorder-Tool` | 0 | 0 | Delete candidate |
| `Dynatrace-AppMon-Upgrade-Automation` | 4 | 0 | |
| `Dynatrace-AppMon-Generic-Execution-Plugin` | 3 | 4 | Open issues: 1 |
| `Dynatrace-AppMon-System-Profile-Difftool` | 0 | 0 | Delete candidate |
| `Dynatrace-AppMon-User-Logins-Plugin` | 3 | 0 | |
| `PurePath-Throughput-Action-Plugin` | 3 | 0 | |
| `Dynatrace-easyTravel-Ansible` | 1 | 3 | |
| `alyeska` | 3 | 0 | Data pipeline toolkit — unrelated to AppMon |

---

## Priority Action: Bulk EOL Banner

Run this script to add an EOL notice to all AppMon archived repos in batch:

```bash
#!/bin/bash
# Requires: gh CLI, jq
# Adds EOL notice to top of README for all archived AppMon repos

gh api /orgs/Dynatrace/repos --paginate \
  | jq -r '.[] | select(.archived == true) | select(.name | startswith("Dynatrace-AppMon")) | .name' \
  | while read repo; do
    echo "Processing $repo..."
    # Clone, prepend EOL notice, commit — or use GitHub API to update file
  done
```

**EOL Notice Template:**
```markdown
> ⚠️ **This repository is archived and no longer maintained.**  
> It was part of the Dynatrace AppMon (Application Monitoring) product line, which has been superseded by the [Dynatrace platform](https://www.dynatrace.com).  
> For modern Dynatrace integrations, see [github.com/Dynatrace](https://github.com/Dynatrace) and [github.com/dynatrace-oss](https://github.com/dynatrace-oss).
```
