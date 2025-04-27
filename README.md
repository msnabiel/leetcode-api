<h1 align="center">LeetCode API</h1>
<div align="center">

### A comprehensive REST API for accessing LeetCode profile data and problem statistics

<img src="https://img.shields.io/badge/License-MIT-green.svg"/>
<img src="https://img.shields.io/npm/v/npm.svg?logo=nodedotjs"/>

![TypeScript](https://img.shields.io/badge/typetscript-%2320232a.svg?style=for-the-badge&logo=typescript&logoColor=%fff)
![Node.js](https://img.shields.io/badge/Node.js-%2320232a?style=for-the-badge&logo=node.js&logoColor=43853D)
![Express.js](https://img.shields.io/badge/express-%2320232a.svg?style=for-the-badge&logo=express&logoColor=%23F7DF1E)
![REST API](https://img.shields.io/badge/RestApi-%2320232a.svg?style=for-the-badge&logo=restAPI&logoColor=%23F7DF1E)

</div>

## Introduction ✨

The LeetCode GraphQL API lacks proper documentation, making it challenging for developers to integrate with the platform. After searching extensively for comprehensive resources, I developed this API to bridge that gap.

This project provides well-documented endpoints for accessing various LeetCode data including user profiles, badges, solved problems, contest information, submission history, daily challenges, and more. Everything is accessible through simple REST endpoints.

## API Base URL 🌐
```
https://leetcode-api-03wd.onrender.com
```
## Docker Deployment 🐳

```
docker run -p 3000:3000 leetcode-api:2.0.1
```
## Contribution Guidelines 🤔

Interested in contributing? Check out our guide: <a href="CONTRIBUTING.md" target="_blank">CONTRIBUTING.md</a>

### Rate Limiting 💡

The API implements rate limiting to ensure service stability and prevent abuse.

### Development Note ‼️

For development purposes, we recommend running the API locally. Follow the instructions in <a href="CONTRIBUTING.md" target="_blank">Local Deployment</a>.

## Available Endpoints 🚀

### User Data Endpoints 👤

| Endpoint | Description | Demo |
| :--- | :--- | :--- |
| `/:username` | Retrieve user profile information | <a href="./public/demo/demo2.png" target="_blank">View Example</a> |
| `/:username/badges` | Get user's earned badges | <a href="./public/demo/demo3.png" target="_blank">View Example</a> |
| `/:username/solved` | Get statistics on solved problems | <a href="./public/demo/demo4.png" target="_blank">View Example</a> |
| `/:username/contest` | Access contest participation data | <a href="./public/demo/demo5.png" target="_blank">View Example</a> |
| `/:username/contest/history` | View complete contest history | <a href="./public/demo/demo6.png" target="_blank">View Example</a> |
| `/:username/submission` | Fetch last 20 submissions | <a href="./public/demo/demo7.png" target="_blank">View Example</a> |
| `/:username/submission?limit=number` | Fetch custom number of submissions | <a href="./public/demo/demo8.png" target="_blank">View Example</a> |
| `/:username/acSubmission` | Get last 20 accepted submissions | <a href="./public/demo/demo16.png" target="_blank">View Example</a> |
| `/:username/acSubmission?limit=7` | Get specified count of accepted submissions | <a href="./public/demo/demo17.png" target="_blank">View Example</a> |
| `/:username/calendar` | Get submission activity calendar | <a href="./public/demo/demo9.png" target="_blank">View Example</a> |

### Enhanced Endpoints 🚀

| Endpoint | Description |
| :--- | :--- |
| `/userProfile/:username` | Comprehensive profile data in a single request |
| `/userProfileCalendar?username=yourname&year=2024` | Year-specific calendar activity |
| `/languageStats?username=yourname` | Programming language usage statistics |
| `/userProfileUserQuestionProgressV2/:userSlug` | Detailed question progress metrics |
| `/skillStats/:username` | User skill distribution analytics |
| `/userContestRankingInfo/:username` | Detailed contest performance ranking |
| `/trendingDiscuss?first=20` | Top trending community discussions |
| `/discussTopic/:topicId` | Specific discussion topic content |
| `/discussComments/:topicId` | Comments for a specific discussion |
| `/dailyQuestion` | Raw data for the daily challenge |

### Problem Data Endpoints ❓

| Endpoint | Description | Demo |
| :--- | :--- | :--- |
| `/daily` | Current daily challenge details | <a href="./public/demo/demo10.png" target="_blank">View Example</a> |
| `/select?titleSlug=selected-question` | Information about a specific problem | <a href="./public/demo/demo11.png" target="_blank">View Example</a> |
| `/problems` | List of 20 problems | <a href="./public/demo/demo12.png" target="_blank">View Example</a> |
| `/problems?limit=number` | Custom-sized list of problems | <a href="./public/demo/demo13.png" target="_blank">View Example</a> |
| `/problems?tags=tag1+tag2` | Filter problems by tags | <a href="./public/demo/demo14.png" target="_blank">View Example</a> |
| `/problems?skip=number` | Skip specified number of problems | *Coming soon* |
| `/problems?difficulty=EASY` | Filter by difficulty (EASY, MEDIUM, HARD) | *Coming soon* |
| `/problems?tags=tag1+tag2+tag3&limit=number` | Combined tag filtering with limit | <a href="./public/demo/demo15.png" target="_blank">View Example</a> |
| `/problems?limit=number&skip=number` | Pagination with limit and skip | *Coming soon* |
| `/problems?tags=tag1+tag2+tag3&limit=number&skip=number` | Complete filtering with pagination | *Coming soon* |

## Author ✒️

- [@msnabiel](https://www.github.com/msnabiel)

## Connect With Me 📲

[![LinkedIn](https://img.shields.io/badge/linkedin-%2320232a.svg?style=normal&logo=linkedIn&logoColor=%230077B5)](https://linkedin.com/in/msnabiel)
[![LeetCode](https://img.shields.io/badge/LeetCode-%2320232a.svg?style=normal&logo=LeetCode&logoColor=%FFA116)](https://leetcode.com/msnabiel)
