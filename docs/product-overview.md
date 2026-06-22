# Product Overview

## What KidPlanner Solves

Parents often need quick, practical help with everyday questions: routines, sleep, activities, behavior, learning, meals, and family planning. Searching through many articles takes time, while generic chatbots usually do not remember context or enforce usage limits.

KidPlanner turns this into a structured Telegram-based assistant with memory, limits, automation, and optional paid usage.

## Target Users

- parents of preschool and school-age children;
- busy families who prefer Telegram over a separate mobile app;
- parenting communities;
- family coaches and consultants;
- small educational projects that need an AI support layer.

## Main User Scenarios

### 1. Ask a Parenting Question

```text
Parent sends a question
        ↓
Telegram bot receives message
        ↓
n8n checks user and request limit
        ↓
AI generates a practical answer
        ↓
Conversation is saved to PostgreSQL
        ↓
Answer is returned in Telegram
```

### 2. Receive a Daily Tip

```text
Scheduled n8n workflow
        ↓
Select active users
        ↓
Generate or retrieve parenting tip
        ↓
Send tip in Telegram
        ↓
Save delivery result
```

### 3. Buy Extra Requests

```text
User reaches free limit
        ↓
Bot offers paid requests
        ↓
Payment provider sends webhook
        ↓
n8n validates event
        ↓
PostgreSQL limit is updated
        ↓
User receives confirmation
```

## Core Product Modules

- Telegram interface;
- user and tariff management;
- request limit control;
- AI answer generation;
- PostgreSQL conversation memory;
- vector storage for contextual retrieval;
- daily tips scheduler;
- payment webhook handling;
- delivery and error logging.

## Business Value

KidPlanner can be used as:

- a standalone subscription bot;
- a lead magnet for parenting specialists;
- a support tool for educational communities;
- a white-label automation template;
- a demo of an AI product built with low-code orchestration and a relational database.

## Current MVP Status

The portfolio version demonstrates the complete business flow without exposing production credentials or real user data.

Implemented in the documented architecture:

- Telegram conversations;
- AI responses;
- request limits;
- PostgreSQL storage;
- tariff logic;
- daily tips;
- payment event processing;
- safe screenshots and demo configuration.

## Recommended Next Steps

1. add multilingual prompt profiles;
2. add parental preference settings;
3. add structured child profiles without storing unnecessary sensitive data;
4. add admin dashboard and usage analytics;
5. improve payment retry and idempotency handling;
6. add automated workflow tests;
7. prepare a white-label deployment guide.
