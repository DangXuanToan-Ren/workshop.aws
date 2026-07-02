---
title: "Blog 2"
date: 2024-01-01
weight: 1
chapter: false
pre: " <b> 3.2. </b> "
---

# Understanding Multi-Build Solution on Amazon GameLift Servers

## INTRODUCTION

During online game development, updating and testing multiple game server versions is a frequent task. However, deploying each new version to the infrastructure can be time-consuming and impact the testing process.

AWS has introduced the Multi-Build solution on Amazon GameLift Servers, allowing developers to store and run multiple game server versions on the same fleet, helping to speed up game development and testing.


## WHAT IS AMAZON GAMELIFT SERVERS?

Amazon GameLift Servers is a fully managed game server hosting service by AWS. This service helps developers deploy, manage, and scale game server systems globally.

Many major game titles on the market have used GameLift to ensure scalability and stability for millions of players.


## CHALLENGES IN GAME DEVELOPMENT

Typically, whenever there's a new server version, developers must:
- Rebuild the server.
- Redeploy to the infrastructure.
- Test and verify functionality.
- Switch between versions when testing is needed.

This process is quite time-consuming, especially during Alpha and Beta stages where updates happen frequently.


## MULTI-BUILD SOLUTION

Multi-Build is a solution that allows storing multiple game server versions on the same Amazon GameLift fleet.

Instead of having to redeploy the entire system, developers only need to:
1. Upload the new version to Amazon S3.
2. The system automatically syncs down to GameLift servers.
3. When creating a Game Session, specify the BuildVersion to use.
4. The server will automatically launch the corresponding version.

This makes switching between versions much faster and more flexible.


## OPERATING ARCHITECTURE

The solution uses two main containers:

### 1. GAME SERVER CONTAINER
This container is responsible for:
- Running the game server.
- Receiving game session creation requests.
- Launching the correct server version based on BuildVersion.

### 2. S3 SYNC CONTAINER
This container runs continuously in the background:
- Checks for changes on Amazon S3.
- Syncs new builds.
- Deletes old, unused builds.
- Ensures data is fully downloaded before execution.

Both containers use a shared folder to access the synced builds.

<img src="/images/Blog2/716962056_1849193866486013_5935965608591198664_n.jpg" alt="Multi-Build GameLift Architecture 1" class="blog-image" />
<img src="/images/Blog2/719483076_1849193823152684_8697794779991986075_n.jpg" alt="Multi-Build GameLift Architecture 2" class="blog-image" />


## AWS SERVICES USED

The Multi-Build solution combines many AWS services:
- Amazon GameLift Servers
- Amazon S3
- Amazon ECR
- AWS IAM
- AWS CodeBuild
- AWS CloudFormation
- Amazon CloudWatch Logs

Thanks to this, the entire deployment and management process is almost completely automated.


## BENEFITS OF MULTI-BUILD

### SPEED UP DEVELOPMENT
Development teams can test multiple game versions simultaneously without having to redeploy the fleet.

### SAVE TIME
Uploading a new build only takes a few minutes instead of performing a full deployment process.

### SUPPORT ALPHA AND BETA TESTING
Multiple game versions can coexist to serve different groups of test players.

### EASY TO MANAGE
Builds are centrally managed on Amazon S3 and automatically synced to servers.


## CONCLUSION

Amazon GameLift Servers Multi-Build is a useful solution for game development teams wanting to speed up testing and release new versions. By allowing multiple builds to coexist on a single fleet, AWS helps significantly reduce deployment time and optimize the game development process.

For game projects in Alpha, Beta, or new feature development stages, this is a solution worth exploring and applying.

Resource link: https://aws.amazon.com/vi/blogs/gametech/rapid-game-server-iteration-on-amazon-gamelift-servers/