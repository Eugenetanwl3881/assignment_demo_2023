# Tiktok Tech Immersion Backend Assignment

![Tests](https://github.com/TikTokTechImmersion/assignment_demo_2023/actions/workflows/test.yml/badge.svg)

This is for the backend assignment submission of 2023 TikTok Tech Immersion.

The task is to design and develop an IM system implementing a set of specific APIs using Golang, developing only the backend side of the system.

These are the requirements met by the system implemented in this repo:
1. Architecture: The system contains two services: one HTTP server and one RPC server. The IDL of HTTP API is provided by the template repo. The RPC IDL is  from the demo repository.
2. Data storage: The system stores messages data. Receivers can access this data at any time. Redis database is used.
3. Message delivery: The system ise able to deliver messages to the intended recipients by PULL mode in a timely and consistent manner. Pull mode means there is no need to maintain the connection and push new messages to receivers in real-time. Only the pull API is implemented, so the receiver can use pull API to fetch messages.
4. Performance and scalability: The system is designed to handle a relatively large number of users and messages. (Support more than 20 concurrency in testing)
