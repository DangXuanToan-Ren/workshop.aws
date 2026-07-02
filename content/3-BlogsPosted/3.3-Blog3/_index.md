---
title: "Blog 3"
date: 2024-01-01
weight: 1
chapter: false
pre: " <b> 3.3. </b> "
---

# [AWS Tech Share] Turning Viewers into Players: Building Interactive Game Experiences with GameLift Streams

Today I'd like to share how AWS solves the "Interactive Streaming" problem – turning game stream viewing into real-time two-way interactive communication.

In game development, organizing playtests often takes a lot of time (downloading builds, setup, reviewing videos). At the same time, interacting with the viewer community also faces barriers when viewers can only type dynamic chat. To solve this problem, AWS has introduced an extremely powerful combined architecture.


## 3 "PILLARS" OF THE SOLUTION ARCHITECTURE:

- **Amazon GameLift Streams**: Supports streaming games directly from the server to the browser (WebRTC) with extremely low latency, reaching quality up to 1080p at 60 FPS without requiring players to download or install the game.
- **Amazon IVS (Interactive Video Service)**: Receives gameplay streams and distributes them globally with subsecond latency (under 1 second).
- **AWS AppSync**: Acts as a bridge, providing WebSocket APIs to transmit signals, reactions, and control commands from viewers back into the game instantly.


## HOW DOES THE PROCESS FLOW WORK?

1. Users interact on the React Frontend interface, authenticated securely through Amazon Cognito.
2. Amazon API Gateway and AWS Lambda will handle communication and initialize the stream session.
3. On the server side, GameLift Streams runs the game, while also launching a background process called "Broadcast Sidecar".
4. This Sidecar application will capture image/audio, encode standard H.264 video, and push the stream directly to Amazon IVS's stage with latency under 300ms.

<img src="/images/Blog3/717792483_1542699650893252_4468378101643065781_n.jpg" alt="GameLift Streams Architecture 1" class="blog-image" />
<img src="/images/Blog3/718204942_1542699634226587_8876440514239223290_n.jpg" alt="GameLift Streams Architecture 2" class="blog-image" />
<img src="/images/Blog3/718597666_1542699647559919_5008900173891667306_n.jpg" alt="GameLift Streams Architecture 3" class="blog-image" />


## TECHNICAL HIGHLIGHT: "CONTROL HANDOFF" MECHANISM

The most impressive point in this solution is how to handle "handing over control" (Control Handoff) to participants. The system uses AWS AppSync Event API to coordinate clear status control messages, such as:
- **TAKEOVER_REQUEST**: Request to take control from the current player.
- **TAKEOVER_APPROVED**: Approve and start sharing the session via CreateStreamConnection API.


## CONCLUSION

This architecture not only optimizes the internal Playtesting process of studios but also opens up endless potential for marketing campaigns: where stream viewers can directly participate in the game (e.g., vote on direction, spawn monsters) right in the browser without any obstacles.


Original article link: https://aws.amazon.com/blogs/gametech/creating-interactive-gaming-experiences-with-amazon-gamelift-streams-and-amazon-interactive-video-service/