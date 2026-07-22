---
title: "Translated Blogs"
date: 2026-06-30
weight: 3
chapter: false
pre: " <b> 3. </b> "
---

This section lists and summarizes the technical blogs translated during the program. For example:

### [Blog 1 - Comprehensive Secrets Management with GitGuardian and AWS Secrets Manager](3.1-Blog1/)
This blog introduces a combined solution using GitGuardian and AWS Secrets Manager to bridge the "visibility gap" in secrets management. You will discover why centralized secrets storage alone is insufficient if credentials have been historically hardcoded in Git history. It explores how the `ggscout` tool hashes secrets into fingerprints locally (via the HMSL protocol) to anonymously match them against source code without exposing raw sensitive data outside your AWS infrastructure. The article also provides a 5-step implementation roadmap (Monitor, Detect, Investigate, Remediate, Guard) for real-time monitoring, alerting, and automated secrets rotation.

### [Blog 2 - AI-Powered Test Automation: A Breakthrough in Automated Testing with Amazon Bedrock and Rapise](3.2-Blog2/)
This blog demonstrates how integrating Amazon Bedrock into the Rapise automated testing tool solves the issue of test scripts breaking due to user interface (UI) changes. You will learn why traditional automation frameworks relying on static IDs/XPaths lead to false positives and high maintenance costs. It highlights how AI enables systems to "understand" UI in context, self-heal scripts upon UI modifications, and automatically generate test scenarios from natural language descriptions. The article outlines a 5-step deployment roadmap to connect the infrastructure, establish baseline UI models, and activate self-healing mechanisms within CI/CD pipelines.

### [Blog 3 - AWS Transform: Automated Technical Debt Remediation Across Thousands of Repositories via AI](3.3-Blog3/)
This blog introduces the Continuous Modernization feature in AWS Transform, an AI-powered tool designed to scan and remediate technical debt across an organization's entire codebase. It discusses why fragmented tools (detecting outdated dependencies, security vulnerabilities, or code smells) fail at large-scale remediation, and explains how the system operates in two modes: Continuous Mode (automatically creating Pull Requests upon detecting repository drift) and Campaign Mode (tailored for large-scale migrations/upgrades). The article also covers deep integration with AWS Security Agent and support for the Model Context Protocol (MCP) to plug directly into existing coding agents.