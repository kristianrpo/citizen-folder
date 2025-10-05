---
name: "NFR"
about: "Define a measurable Non-Functional Requirement (NFR)"
title: "NFR-<ID>: <Short descriptive name>"
labels: ["type:NFR","priority:P?","tier:?","area:?"]
assignees: []
---

## Short Description
<!-- Briefly describe the intent of this NFR and why it is important (e.g., scalability, reliability, performance, security). -->

---

## Scope (services / context / duration)
- **Scope:** <!-- e.g., Entire system / Specific microservice / API endpoint -->
- **Time horizon:** <!-- e.g., 6 months / 12–18 months -->
- **Environments:** <!-- dev / staging / prod -->
- **Applicable schedule:** <!-- 24x7 / business hours / peak periods -->

---

## SLI (Service Level Indicators)
<!-- List what metrics will be measured to validate this NFR. Examples: -->
<!-- - DAU projections -->
<!-- - QPS per critical path -->
<!-- - Latency p95/p99 -->
<!-- - Error rate -->
<!-- - Concurrency ratio -->
<!-- - Storage growth -->
<!-- - Throughput -->

---

## SLO (Service Level Objectives)
<!-- Define the quantitative or qualitative goals/thresholds for the SLIs. Examples: -->
<!-- - p95 < 800 ms -->
<!-- - 99.95% availability monthly -->
<!-- - Scaling plan reviewed quarterly -->
<!-- - Error rate < 0.1% -->
<!-- - Documented model updated every quarter -->

---

## Measurement / Instrumentation
- **How:** <!-- e.g., APM, OpenTelemetry metrics, synthetic checks, log analysis -->
- **Where:** <!-- e.g., Grafana dashboard, Kibana panel, alert channel -->
- **Frequency:** <!-- continuous / weekly / per deploy / quarterly review -->

---

## Reference Data / Load Hypotheses
<!-- List the assumptions and estimated values used to size or evaluate the system. Examples: -->
- Registered Users (UR): <!-- e.g., 4M -->
- Daily Active Users (DAU): <!-- e.g., 10% (≈400k) -->
- Peak Factor: <!-- e.g., 2.5× over average hour -->
- Average Payload Size: <!-- e.g., ≤10 MB -->
- Latency Target: <!-- e.g., p95 ≤ 2 s -->
- Transactions or Transfers per Day: <!-- e.g., 12k/day -->
- Other relevant assumptions: <!-- concurrency, storage growth, etc. -->

---

## Acceptance Criteria (Definition of Done)
- [ ] SLI metrics defined and instrumented
- [ ] Dashboard showing real-time SLI values
- [ ] Alerts configured for SLO breaches
- [ ] Documentation and runbook updated
- [ ] Review meeting or quarterly validation completed
- [ ] No compatibility or regression issues introduced

---

## Risks / Dependencies
<!-- List potential risks or external dependencies that can affect this NFR. Examples: -->
<!-- network limitations, third-party APIs, storage scaling, messaging systems, etc. -->

---

## Granularity Notes (Cohesion / Volatility)
<!-- Indicate whether this NFR affects one or several microservices, -->
<!-- and if differences in load, volatility, or SLA suggest splitting or merging components. -->
