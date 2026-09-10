# 🔴 Archive Candidates — dynatrace-oss

These repositories are already archived on GitHub or meet the criteria for archiving: no meaningful recent commits, superseded technology, or confirmed product EOL. All already-archived repos are marked **⛔ ARCHIVED**.

---

## Already Archived by GitHub

### `barista` ⛔ ARCHIVED
**URL:** https://github.com/dynatrace-oss/barista  
**Language:** TypeScript | **Stars:** 146 ⭐ | **Forks:** 74

| Dimension | Assessment |
|---|---|
| **Business / Ecosystem Purpose** | Barista — the Dynatrace design system; Angular component library tailored to scale |
| **Strategic Relevance** | ❌ Archived — superseded by internal design system evolution |
| **Notable Signals** | Highest fork count in the org (74); 146 stars — significant legacy community footprint |
| **Action Required** | Add README banner pointing to any successor design system; ensure no dependent projects are still actively importing from this repo |
| **Recommended Disposition** | 🔴 **Archive Candidate** ✅ Already archived|

---

### `OneAgent-SDK-Python-AutoInstrumentation` ⛔ ARCHIVED
**URL:** https://github.com/dynatrace-oss/OneAgent-SDK-Python-AutoInstrumentation  
**Language:** Python | **Stars:** 64 ⭐ | **Forks:** 32 | **Open Issues:** 6

| Dimension | Assessment |
|---|---|
| **Business / Ecosystem Purpose** | `autodynatrace` — Python library implementing automatic instrumentation using the OneAgent SDK |
| **Strategic Relevance** | ❌ Archived — superseded by OpenTelemetry-based instrumentation |
| **Action Required** | 6 open issues remain unresolved; update README to direct users to OTel instrumentation examples (`dynatrace-ai-agent-instrumentation-examples`) |
| **Recommended Disposition** | 🔴 **Archive Candidate** ✅ Already archived|

---

### `dynatrace-aws-log-forwarder` ⛔ ARCHIVED
**URL:** https://github.com/dynatrace-oss/dynatrace-aws-log-forwarder  
**Language:** Python | **Stars:** 14 ⭐ | **Forks:** 11

| Dimension | Assessment |
|---|---|
| **Business / Ecosystem Purpose** | Streams logs from AWS CloudWatch into Dynatrace Logs via Lambda |
| **Strategic Relevance** | ❌ Archived — superseded by `dynatrace-aws-s3-log-forwarder` and native OTel log ingestion |
| **Action Required** | README should link to `dynatrace-aws-s3-log-forwarder` as the active successor |
| **Recommended Disposition** | 🔴 **Archive Candidate** ✅ Already archived |

---

### `opentelemetry-metric-python` ⛔ ARCHIVED
**URL:** https://github.com/dynatrace-oss/opentelemetry-metric-python  
**Language:** Python | **Stars:** 13 ⭐ | **Forks:** 6

| Dimension | Assessment |
|---|---|
| **Business / Ecosystem Purpose** | Dynatrace OpenTelemetry Metrics Exporter for Python |
| **Strategic Relevance** | ❌ Archived — superseded by the upstream OTel Python SDK OTLP exporter with Dynatrace native OTLP ingest |
| **Action Required** | README should redirect to upstream OTel Python SDK |
| **Recommended Disposition** | 🔴 **Archive Candidate** ✅ Already archived |

---

### `opentelemetry-metric-java` ⛔ ARCHIVED
**URL:** https://github.com/dynatrace-oss/opentelemetry-metric-java  
**Language:** Java | **Stars:** 9 ⭐ | **Forks:** 1

| Dimension | Assessment |
|---|---|
| **Business / Ecosystem Purpose** | Dynatrace OpenTelemetry Metrics Exporter for Java |
| **Strategic Relevance** | ❌ Archived — superseded by upstream OTel Java SDK OTLP exporter |
| **Recommended Disposition** | 🔴 **Archive Candidate** ✅ Already archived |

---

### `opentelemetry-metric-dotnet` ⛔ ARCHIVED
**URL:** https://github.com/dynatrace-oss/opentelemetry-metric-dotnet  
**Language:** C# | **Stars:** 8 ⭐ | **Forks:** 2

| Dimension | Assessment |
|---|---|
| **Business / Ecosystem Purpose** | Dynatrace OpenTelemetry Metrics Exporter for .NET |
| **Strategic Relevance** | ❌ Archived — superseded by upstream OTel .NET SDK OTLP exporter |
| **Recommended Disposition** | 🔴 **Archive Candidate** ✅ Already archived |

---

### `opentelemetry-metric-go` ⛔ ARCHIVED
**URL:** https://github.com/dynatrace-oss/opentelemetry-metric-go  
**Language:** Go | **Stars:** 3 ⭐ | **Forks:** 2

| Dimension | Assessment |
|---|---|
| **Business / Ecosystem Purpose** | Dynatrace OpenTelemetry Metrics Exporter for Go |
| **Strategic Relevance** | ❌ Archived — superseded by upstream OTel Go SDK OTLP exporter |
| **Recommended Disposition** | 🔴 **Archive Candidate** ✅ Already archived |

---

### `opentelemetry-metric-js` ⛔ ARCHIVED
**URL:** https://github.com/dynatrace-oss/opentelemetry-metric-js  
**Language:** TypeScript | **Stars:** 6 ⭐ | **Forks:** 2

| Dimension | Assessment |
|---|---|
| **Business / Ecosystem Purpose** | Dynatrace OpenTelemetry Metrics Exporter for JavaScript |
| **Strategic Relevance** | ❌ Archived — superseded by upstream OTel JS SDK OTLP exporter |
| **Recommended Disposition** | 🔴 **Archive Candidate** ✅ Already archived |

---

### `db-load-generator` ⛔ ARCHIVED
**URL:** https://github.com/dynatrace-oss/db-load-generator  
**Language:** Python | **Stars:** 6 ⭐ | **Forks:** 2 | **Open Issues:** 2

| Dimension | Assessment |
|---|---|
| **Business / Ecosystem Purpose** | Mock database activity and scalable database load simulation tool |
| **Strategic Relevance** | ❌ Archived — demo/test tooling; superseded by `easytrade` and other demo apps |
| **Recommended Disposition** | 🔴 **Archive Candidate** ✅ Already archived |

---

### `invadium` ⛔ ARCHIVED
**URL:** https://github.com/dynatrace-oss/invadium  
**Language:** TypeScript | **Stars:** 11 ⭐ | **Forks:** 4

| Dimension | Assessment |
|---|---|
| **Business / Ecosystem Purpose** | Runs exploit playbooks against vulnerable target applications in a reproducible, intuitive manner |
| **Strategic Relevance** | ❌ Archived — security research tool; superseded by `kimera` and `unguard` for current demos |
| **Recommended Disposition** | 🔴 **Archive Candidate** ✅ Already archived |

---

### `jmeter-dynatrace-plugin` ⛔ ARCHIVED
**URL:** https://github.com/dynatrace-oss/jmeter-dynatrace-plugin  
**Language:** Java | **Stars:** 13 ⭐ | **Forks:** 8

| Dimension | Assessment |
|---|---|
| **Business / Ecosystem Purpose** | JMeter Backend Listener that sends load test metrics to Dynatrace via the API |
| **Strategic Relevance** | ❌ Archived — JMeter integration; load testing patterns now use OTel |
| **Recommended Disposition** | 🔴 **Archive Candidate** ✅ Already archived |

---

### `dynatrace-metric-utils-dotnet` ⛔ ARCHIVED
**URL:** https://github.com/dynatrace-oss/dynatrace-metric-utils-dotnet  
**Language:** C# | **Stars:** 1 ⭐ | **Forks:** 0

| Dimension | Assessment |
|---|---|
| **Business / Ecosystem Purpose** | .NET utility for interacting with the Dynatrace Metrics v2 API |
| **Strategic Relevance** | ❌ Archived — superseded by OTel .NET SDK |
| **Recommended Disposition** | 🔴 **Archive Candidate** ✅ Already archived |

---

### `dynatrace-metric-utils-python` ⛔ ARCHIVED
**URL:** https://github.com/dynatrace-oss/dynatrace-metric-utils-python  
**Language:** Python | **Stars:** 1 ⭐ | **Forks:** 0

| Dimension | Assessment |
|---|---|
| **Business / Ecosystem Purpose** | Python utility for interacting with the Dynatrace Metrics v2 API |
| **Strategic Relevance** | ❌ Archived — superseded by OTel Python SDK |
| **Recommended Disposition** | 🔴 **Archive Candidate** ✅ Already archived |

---

### `dynatrace-metric-utils-js` ⛔ ARCHIVED
**URL:** https://github.com/dynatrace-oss/dynatrace-metric-utils-js  
**Language:** TypeScript | **Stars:** 1 ⭐ | **Forks:** 0

| Dimension | Assessment |
|---|---|
| **Business / Ecosystem Purpose** | JavaScript utility for interacting with the Dynatrace Metrics v2 API |
| **Strategic Relevance** | ❌ Archived — superseded by OTel JS SDK |
| **Recommended Disposition** | 🔴 **Archive Candidate** ✅ Already archived |

---

### `kached-properties` ⛔ ARCHIVED
**URL:** https://github.com/dynatrace-oss/kached-properties  
**Language:** Kotlin | **Stars:** 5 ⭐ | **Forks:** 0 | **Open Issues:** 2

| Dimension | Assessment |
|---|---|
| **Business / Ecosystem Purpose** | Caching in Kotlin made simple — Kotlin property delegation library |
| **Strategic Relevance** | ❌ Archived — internal utility library; no longer maintained |
| **Recommended Disposition** | 🔴 **Archive Candidate** ✅ Already archived |

---

### `junit-jupiter-open-telemetry-extension` ⛔ ARCHIVED
**URL:** https://github.com/dynatrace-oss/junit-jupiter-open-telemetry-extension  
**Language:** Java | **Stars:** 8 ⭐ | **Forks:** 3

| Dimension | Assessment |
|---|---|
| **Business / Ecosystem Purpose** | JUnit 5 extension for OpenTelemetry — traces unit test execution |
| **Strategic Relevance** | ❌ Archived — experimental OTel testing integration |
| **Recommended Disposition** | 🔴 **Archive Candidate** ✅ Already archived |

---

### `ebpf-dump` ⛔ ARCHIVED
**URL:** https://github.com/dynatrace-oss/ebpf-dump  
**Language:** C | **Stars:** 12 ⭐ | **Forks:** 2 | **Open Issues:** 3

| Dimension | Assessment |
|---|---|
| **Business / Ecosystem Purpose** | Kubernetes operator that logs and forwards all HTTP requests over TCP/IPv4 using an eBPF program |
| **Strategic Relevance** | ❌ Archived — superseded by `eBPF-Discovery` and `nettracer-bpf` |
| **Recommended Disposition** | 🔴 **Archive Candidate** ✅ Already archived — close open issues; add redirect to successor repos |

---

### `aws-health-events-integration` ⛔ ARCHIVED
**URL:** https://github.com/dynatrace-oss/aws-health-events-integration  
**Language:** JavaScript | **Stars:** 3 ⭐ | **Forks:** 0

| Dimension | Assessment |
|---|---|
| **Business / Ecosystem Purpose** | AWS Health Events integration with Dynatrace |
| **Strategic Relevance** | ❌ Archived — superseded by native AWS integrations and `dynatrace-aws-s3-log-forwarder` |
| **Recommended Disposition** | 🔴 **Archive Candidate** ✅ Already archived |

---

### `rautee` ⛔ ARCHIVED
**URL:** https://github.com/dynatrace-oss/rautee  
**Language:** Python | **Stars:** 0 ⭐ | **Forks:** 0

| Dimension | Assessment |
|---|---|
| **Business / Ecosystem Purpose** | Links to Dynatrace Application Security page — appears to be an internal tool or placeholder |
| **Strategic Relevance** | ❌ Archived — no description; zero adoption |
| **Recommended Disposition** | 🔴 **Archive Candidate** ✅ Already archived — candidate for deletion |

---

### `dt-awslayertool` ⛔ ARCHIVED
**URL:** https://github.com/dynatrace-oss/dt-awslayertool  
**Language:** Python | **Stars:** 6 ⭐ | **Forks:** 0

| Dimension | Assessment |
|---|---|
| **Business / Ecosystem Purpose** | Utility to download or clone AWS Lambda Layers, including Dynatrace extensions distributed as layers |
| **Strategic Relevance** | ❌ Archived — Lambda Layer distribution pattern superseded |
| **Recommended Disposition** | 🔴 **Archive Candidate** ✅ Already archived |

---

### `PTC-Windchill` ⛔ ARCHIVED
**URL:** https://github.com/dynatrace-oss/PTC-Windchill  
**Language:** Go | **Stars:** 7 ⭐ | **Forks:** 6

| Dimension | Assessment |
|---|---|
| **Business / Ecosystem Purpose** | PTC Windchill integration — industrial PLM software monitoring with Dynatrace |
| **Strategic Relevance** | ❌ Archived — very niche industrial segment |
| **Recommended Disposition** | 🔴 **Archive Candidate** ✅ Already archived |

---

### `log4j-metadata-provider` ⛔ ARCHIVED
**URL:** https://github.com/dynatrace-oss/log4j-metadata-provider  
**Language:** Java | **Stars:** 0 ⭐ | **Forks:** 0

| Dimension | Assessment |
|---|---|
| **Business / Ecosystem Purpose** | Log4j metadata provider — Java logging integration |
| **Strategic Relevance** | ❌ Archived — zero adoption; Log4j 2 Log4Shell context makes this historically sensitive |
| **Recommended Disposition** | 🔴 **Archive Candidate** ✅ Already archived — candidate for deletion given zero adoption and Log4Shell connotations |

---

## Not Yet Archived — Recommended for Archive

### `Perform-Hackathon-2026`
**URL:** https://github.com/dynatrace-oss/Perform-Hackathon-2026  
**Language:** JavaScript | **Stars:** 2 ⭐ | **Forks:** 15

| Dimension | Assessment |
|---|---|
| **Business / Ecosystem Purpose** | Materials from the Dynatrace Perform 2026 Hackathon |
| **Strategic Relevance** | ❌ Event-specific; no ongoing value after the event |
| **Activity Level** | 🔴 Will naturally become inactive post-event |
| **Action Required** | Archive after 3 months post-event; 15 forks from participants |
| **Recommended Disposition** | 🔴 **Archive Candidate** ✅ Already archived |
