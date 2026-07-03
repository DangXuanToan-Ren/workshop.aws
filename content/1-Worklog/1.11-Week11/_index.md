---
title: "Week 11 Worklog"
date: 2024-01-01
weight: 2
chapter: false
pre: " <b> 1.11. </b> "
---



### Week 11 Objectives:

* Set up CI/CD (Continuous Integration and Continuous Deployment) pipeline to automate the Frontend application release process.

### Tasks to be carried out this week:
| Day | Task                                                                                                                                                                                                   | Start Date | Completion Date | Reference Material                        |
| --- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ---------- | --------------- | ----------------------------------------- |
| 2   | - Research CI/CD pipeline for Frontend applications. <br> - Evaluate and select tools for pipeline configuration (using AWS CodePipeline, CodeBuild or GitHub Actions).                                 | 30/06/2026 | 30/06/2026      |
| 3   | - Practice: <br>&emsp; + Set up source code on Git repository. <br>&emsp; + Configure the first pipeline step to automatically build source code whenever there are new code changes.                  | 01/07/2026 | 01/07/2026      |
| 4   | - Practice: <br>&emsp; + Integrate the automatic sync step for static files of the Frontend application after successful build to Amazon S3 storage.                                                   | 02/07/2026 | 02/07/2026      |
| 5   | - Practice: <br>&emsp; + Write configuration scripts to automatically perform Invalidation (clear cache) on Amazon CloudFront into the pipeline process.                                              | 03/07/2026 | 03/07/2026      |
| 6   | - Comprehensive testing of the entire CI/CD pipeline. <br> - Push a small code change and monitor the system's automatic build, deploy, and cache clearing process to update the interface immediately without manual intervention. | 04/07/2026 | 04/07/2026      |


### Week 11 Achievements:

* Grasped the basic concepts and workflow of CI/CD (Continuous Integration / Continuous Deployment).
* Successfully selected and configured the pipeline using GitHub Actions (or AWS CodePipeline as chosen).
* Successfully set up the Git repository and connected it to the CI/CD system.
* Automated the Frontend source code build process every time a new commit is pushed to the repo.
* Successfully integrated the static file deployment step to Amazon S3 after the build is complete.
* Performed automatic CloudFront Invalidation to clear cache, allowing users to see the latest changes immediately.
* Successfully tested the entire CI/CD pipeline: just push code, and the system automatically completes build → deploy → invalidate cache.
* Clearly understood the benefits of CI/CD: minimizing manual errors, accelerating release speed, ensuring consistency between environments.

