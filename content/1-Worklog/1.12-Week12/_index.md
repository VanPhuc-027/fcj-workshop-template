---
title: "Week 12 Worklog"
date: 2026-07-03
weight: 12
chapter: false
pre: " <b> 1.12 </b> "
---

### Week 12 Objectives:

* Deploy all infrastructure and application source code to AWS, finalize the project report, and complete the workshop documentation.

### Tasks to Implement This Week:

| Day | Task | Start Date | Completion Date | Resource Links |
| --- | --- | --- | --- | --- |
| Fri | - Update the `entrypoint.js` script inside the Dockerfile; test S3 storage logic locally before rebuilding and redeploying the container image to Amazon ECR. | 2026/07/03 | 2026/07/03 | |
| Sat | - Proceed with creating the Amazon ECS cluster and configuring Task Definitions; test task execution logic. | 2026/07/04 | 2026/07/04 | |
| Sun | - Perform manual testing and discover logic bugs preventing AWS Lambda from reading `test-scripts` stored in S3; research and patch the Docker configuration file. | 2026/07/05 | 2026/07/05 | |
| Mon | - Troubleshoot missing environment variables; debug manual execution returning a 401 Unauthorized status code with test execution stuck in the `running` state. | 2026/07/06 | 2026/07/06 | |
| Tue | - Fix logic issue preventing AI integration from reading CloudWatch Log Streams for error summarization; adjust API keys to Free Tier to restore log stream access. | 2026/07/07 | 2026/07/07 | |
| Wed | - Fix blank body issue in error summary emails sent post-testing; resolve minor frontend state bugs and integrate updates into the workshop documentation. | 2026/07/08 | 2026/07/08 | <https://www.youtube.com/watch?v=AQlsd0nWdZk&list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> |
| Thu | - Perform final end-to-end testing, validate all workshop user flows, and finalize the project report. | 2026/07/09 | 2026/07/09 | <https://www.youtube.com/watch?v=AQlsd0nWdZk&list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i> |

### Week 12 Achievements:

* Successfully updated and optimized the `entrypoint.js` script within the Dockerfile, validating S3 storage persistence locally prior to building and pushing the final image version to Amazon ECR.
* Provisioned and fully configured the Amazon ECS Cluster alongside detailed ECS Task Definitions; resolved Amazon S3 integration issues.
* Resolved environment variable configuration gaps and 401 authentication errors; fixed execution states being stuck in `running`.
* Debugged and restored AI & CloudWatch log streams integration, resolving issue where AI services could not consume Amazon CloudWatch Log Streams for error summarization.
* Optimized email notification mechanisms and Frontend states, fixing email body formatting to ensure complete, intuitive AI error summaries are delivered to users.