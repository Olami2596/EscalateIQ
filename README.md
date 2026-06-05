# EscalateIQ

### Intelligent Customer Support Automation with AI-Powered Sentiment Detection

---

# Summary

This is a customer support automation solution designed to improve response times, maintain consistent customer communication, and proactively identify customer dissatisfaction.

The system automatically receives customer inquiries through Telegram, analyzes sentiment using AI, generates context-aware responses in the customer's original language, and escalates negative interactions to internal teams via Slack.

---

# Overview

The system:

1. Receives customer messages through Telegram.
2. Detects customer sentiment using AI.
3. Generates professional responses in the customer's language.
4. Provides solution-oriented responses for negative feedback.
5. Alerts internal teams when negative sentiment is detected.

This creates a hybrid support model where AI handles routine interactions while humans focus on critical cases.

---

# System Architecture

## Workflow Overview

<img width="1462" height="602" alt="Capture" src="https://github.com/user-attachments/assets/14df0cb4-608c-4c0b-a0da-c8eecd72bd86" />

---

# Technology Stack

## Automation Platform

* Make.com

## Artificial Intelligence

* Make AI Toolkit
* AI Sentiment Analysis
* AI Text Generation

## Communication Channels

* Telegram Bot API
* Slack API

---

# Workflow Breakdown

## Step 1: Customer Interaction

A customer sends a message to the Telegram support bot.

The Telegram Watch Updates module acts as the workflow trigger.

---

## Step 2: Message Validation

A filter ensures only text-based messages proceed through the workflow.

This prevents unsupported content such as:

* Images
* Voice Notes
* Unsupported Media

---

## Step 3: Sentiment Analysis

The incoming message is analyzed using AI to classify sentiment.

Potential classifications include:

* Positive
* Neutral
* Negative

The resulting sentiment score determines downstream routing decisions.

---

## Step 4: AI Response Generation

A second AI module generates a professional response.

The prompt is designed to:

* Match the customer's language
* Maintain a professional tone
* Provide contextual assistance
* Offer solutions when dissatisfaction is detected

---

## Step 5: Intelligent Routing

A router evaluates sentiment classification.

### Route A: Negative Sentiment

When negative sentiment is detected:

* Internal teams receive a Slack notification
* Support staff gain visibility into potentially critical issues
* Human intervention can occur if necessary

### Route B: Customer Response

All messages continue through the response path.

The AI-generated reply is delivered directly to the customer through Telegram.

---

# Key Features

## Multilingual Customer Support

Automatically responds in the same language used by the customer.

## AI-Powered Sentiment Detection

Identifies dissatisfied customers in real time.

## Automated Escalation

Routes potentially critical conversations to internal teams.

## Consistent Communication

Ensures every customer receives a professional response.

## Faster Resolution Times

Reduces delays caused by manual triage.

## Human-in-the-Loop Support

Escalates important conversations without removing human oversight.

---

# Business Impact

This solution helps organizations:

* Improve customer response speed
* Reduce support workload
* Increase visibility into customer dissatisfaction
* Standardize communication quality
* Create scalable support operations

---

# Setup Instructions

## Prerequisites

* Make.com Account
* Telegram Bot
* Slack Workspace
* Make AI Toolkit Access

## Installation

1. Create a Telegram Bot.
2. Configure the Telegram Watch Updates trigger.
3. Connect Make AI Toolkit modules.
4. Configure sentiment analysis prompts.
5. Connect Slack integration.
6. Configure routing logic.
7. Test positive, neutral, and negative scenarios.
8. Deploy workflow.


---

## 🔗 Live Automation Workflow

👉 [View Automation Blueprint](https://eu2.make.com/public/shared-scenario/Id2lgzF3qIl/integration-telegram-bot-make-ai-toolki)
