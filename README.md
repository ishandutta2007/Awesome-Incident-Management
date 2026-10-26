# Awesome-Incident-Management

## Top Incident Management Ecosystem



**Curated List of SaaS Products & Open-Source GitHub Projects**  

*Focused on Alerting, On-Call Scheduling & Incident Response Orchestration*  

**Last updated: October 2026**



This repository tracks notable **SaaS platforms** and **open-source projects** for **Incident Management**. These tools enable engineering and IT operations teams to detect critical issues, route alerts to the right responders, coordinate resolution across teams, and conduct post-incident reviews—minimizing downtime and restoring service quickly.



**Examples** include ServiceNow Incident Management, PagerDuty, Opsgenie, VictorOps (Splunk On-Call), xMatters, AlertOps, Better Uptime, Jira Service Management, Freshservice, and Squadcast (the category leaders).



**Open-source emphasis**: This section is expanded with active projects for self-hosted on-call scheduling, alert routing, and incident response platforms—ideal for organizations building sovereign incident management infrastructure without per-user or per-alert licensing lock-in.



Contributions welcome! Open a PR to add/update entries. Keep descriptions factual and link to official sites.



## Table of Contents

- [SaaS/Hosted Platforms](#saas-products)

- [Open-Source GitHub Projects](#open-source-github-projects)

- [How to Contribute](#how-to-contribute)

- [Disclaimer](#disclaimer)



## SaaS/Hosted Platforms



- **[ServiceNow Incident Management](https://www.servicenow.com/)**  

  Enterprise incident management on the Now Platform with major incident management, communication plans, and response templates; the Australia release adds granular admin roles (sn_incident_admin, sn_mim_admin) for separating incident and major incident configuration permissions, and form channel access for response templates directly from incident records .



- **[PagerDuty](https://www.pagerduty.com/)**  

  Named a Leader and Outperformer in the 2026 GigaOm Radar for IT Incident Response Platforms for the fourth consecutive year; the Operations Cloud provides incident lifecycle orchestration from detection through post-incident learning, with AI agents (SRE, Scribe, Insights, Shift) for autonomous response, real-time call transcription via Scribe Agent, and mobile incident operations for distributed teams .



- **[Opsgenie](https://www.atlassian.com/software/opsgenie)**  

  Atlassian's incident management platform with on-call scheduling, alert routing, and escalation policies; users praise its user-friendly interface and customizable alerting rules, though there is ongoing concern about the impact of its migration into the Atlassian ecosystem on app integrations .



- **[VictorOps (Splunk On-Call)](https://www.splunk.com/)**  

  Incident management platform integrated with Splunk observability; the Splunk Add-on for On-Call ingests users, teams, on-call schedules, and incidents into Splunk for unified dashboards and granular reporting across multiple On-Call instances .



- **[xMatters](https://www.xmatters.com/)**  

  Everbridge's automated incident management platform with Flow Designer for no-code workflow automation, signal enrichment to reduce alert fatigue, AI Incident Agent for root cause identification and next-action recommendations, and intelligent on-call scheduling with automated escalations .



- **[AlertOps](https://alertops.com/)**  

  AI-driven incident response platform with OpsIQ Intelligence Suite; features automated alert correlation to group related alerts into single incidents, Intellifield Reasoning Agents for structured analysis of unstructured alerts, AI-generated post-mortems, and Ada conversational agent for querying and acting on alerts, users, groups, and schedules .



- **[Better Uptime (Better Stack)](https://betterstack.com/)**  

  Observability and incident management platform with integrated uptime monitoring, on-call scheduling, and status pages; recent pricing includes call routing for incoming phone calls to on-call personnel, AI post-mortems, and SOC 2 Type 2 / ISO 27001 compliance .



- **[Jira Service Management](https://www.atlassian.com/software/jira/service-management)**  

  Incident management capabilities within Atlassian's ITSM platform: aggregates alerts from monitoring and logging tools, supports employee incident reporting via service portal, routes alerts through multiple channels (SMS, email, push, chat, voice), includes incident response templates, runbook attachment, Statuspage integration for customer communication, and auto-generated post-incident reviews .



- **[Freshservice](https://www.freshworks.com/freshservice/)**  

  IT incident management with Freddy AI for detection and correlation, dynamic service maps connecting alerts to business impact, automated on-call routing and war room creation, and AI-generated postmortems; integrates with Azure AD, Jira, Datadog, Zoom, Teams, and Slack for context enrichment .



- **[Squadcast](https://www.squadcast.com/)**  

  Incident management platform purpose-built for SRE teams; features Intelligent Alert Grouping for alert fatigue reduction, Live Call Routing for customer-reported incidents, Stakeholder Groups for targeted notifications, ServiceNow extension for centralized ticketing, and AI Suggestions and Incident Summaries for faster response .



## Open-Source GitHub Projects



- **[GoAlert](https://github.com/target/goalert)**  

  Open-source on-call scheduling, automated escalation, and notification platform (Apache-2.0, ~1,800 GitHub stars); provides on-call rotations with multi-team scheduling, escalation policies with conditional routing, and multi-channel notifications (SMS, voice, Slack, email); designed to ensure critical alerts never go unanswered; actively maintained with releases over the past six years .



- **[Catalyst](https://github.com/SecurityBrewery/catalyst)**  

  Self-hosted open-source incident response platform and ticket system (SecurityBrewery) for automating alert handling and incident response procedures; features ticket management for alerts, incidents, and investigations, task assignment, reaction-based automation (triggers + actions for HTTP/Webhooks and Python), investigation timelines, dashboards, and custom fields for MITRE ATT&CK information and affected systems .



- **[versus-incident](https://pkg.go.dev/github.com/VersusControl/versus-incident)**  

  Open-source incident management service (Go) with on-call functionality, escalation with configurable acknowledgment windows, and multi-channel alerting to Slack, Telegram, Email, Microsoft Teams, and AWS SNS; supports AWS Incident Manager response plan integration and Redis-backed state management for on-call coordination .



### Additional Strong Open-Source Options



- **Grafana OnCall** — Grafana's open-source on-call management tool (AGPL) for alert routing and escalation, tightly integrated with Grafana alerting and Prometheus.

- **Keep** — Open-source AIOps and alert management platform that aggregates alerts, deduplicates events, and provides workflow automation; complements on-call tools by reducing noise before paging.

- **Uptime Kuma** — Lightweight self-hosted uptime monitoring with notification integrations; useful as a detection layer feeding into incident management workflows.



**Frameworks for building custom systems**: Combine **GoAlert** for on-call scheduling and escalation, **Catalyst** for incident response ticket management and automation, and **versus-incident** for multi-channel alerting with on-call acknowledgment workflows in a self-hosted incident management stack; layer **Keep** for alert correlation and noise reduction upstream of paging.



## How to Contribute



1. Fork the repo.

2. Add/edit entries in `README.md` (follow existing format).

3. Include: name, link, 1–2 sentence description, and whether it's SaaS or open-source.

4. Submit PR with a short explanation.



Star the repo if you find it useful!



## Disclaimer



- This is a **community-curated** list — not exhaustive and not an endorsement.

- Incident management platforms handling production alerts and responder data must comply with applicable security policies and regulations; alert payloads may contain sensitive system information requiring access controls.

- Self-hosted open-source solutions vary in scope—GoAlert provides mature on-call scheduling, while Catalyst focuses on incident response workflow automation; full incident lifecycle coverage typically requires combining multiple tools or adopting a commercial platform.

- Verify license terms for commercial use; GoAlert uses Apache-2.0 , and Catalyst is open-source (check repository for license details).



---



**Made for SREs, DevOps engineers, on-call responders, and IT operations teams.**  

Let's make incident management more open, reliable, and responder-friendly.
