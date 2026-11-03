# Vytera — Public Product Showcase

**Connecting property sales, messaging, and AI assistance in one CRM**

Real estate teams need to connect incoming conversations with the properties and opportunities they manage. I built Vytera as a full-stack CRM that combines inventory, contacts, sales workflows, and AI-assisted messaging.

[Live website](https://www.vytera.cl) · [Marco Alvarado](https://github.com/7pixel-cl) · [Hire on Upwork](https://www.upwork.com/freelancers/~01dadbf4c232f73f55)

**Role:** Full-Stack Developer  
**Stack:** Next.js, React, TypeScript, tRPC, PostgreSQL, Claude, Gemini

This repository contains public portfolio documentation and approved product imagery. It does not contain the production application's source code.

![Vytera public product view](images/vytera-home.png)

*Public Vytera landing page with an illustrative inbox demo, captured in October 2026. Names, messages, and marketing figures in this image are illustrative and are not verified customer outcomes.*

## Hook

I connected the sales workflow to the conversation: property inventory, leads, pipelines, visits, and quotes sit alongside messaging and AI assistance. The result is a web product that combines CRM operations with document-grounded responses and human-controlled conversation modes.

## Context & Problem

Vytera is a real estate CRM for teams handling property inquiries. A conversation is only useful if the team can relate it to a contact, relevant properties, and a next sales action. My role is full-stack development across the interface, backend integrations, and AI workflows.

## Technical Discovery

Two design concerns shape the product: AI needs relevant business knowledge, and teams need control over when it speaks. Document-grounded answers address the first concern; automatic, assisted, and manual conversation modes address the second. Compared with a single always-on auto-reply behavior, these modes introduce more state and interface decisions, but give the team a review path and a way to keep a conversation entirely human-led. Queued webhook processing separates incoming events from the longer work needed to update the application and generate assistance.

## Implementation Decisions & Challenges

The product combines property inventory, contacts, sales pipelines, visits, and quotes with Meta messaging integrations. I implemented Claude-based classification and replies, Gemini-powered document search, queued webhook processing, and real-time inbox updates. A key engineering challenge is coordinating external messages, business context, AI work, and the visible conversation state. Automatic, assisted, and manual modes provide different levels of human control; the interface needs to communicate that control clearly. This showcase describes the integration pattern without publishing production code, internal schemas, or customer data.

## Outcomes

Delivered functionality includes a unified real estate backoffice, messaging integrations, document-grounded assistance, and three conversation modes: automatic, assisted, and manual. The public website provides a product overview. The landing-page demo is illustrative; this showcase does not claim verified response-time improvements, sales lift, customer counts, or revenue.

## Learnings

The technical takeaway is that AI assistance works as part of a workflow with explicit human control. A useful answer depends on business context, and a usable inbox needs a clear distinction between a suggestion, an automated reply, and a conversation handled by a person.

## Repository contents

- `README.md`: the public project overview and case study.
- `case-study.md`: the case study with metadata for reuse.
- `case-study.html`: a standalone HTML reading version; download and open it locally.
- `images/`: approved public portfolio screenshot.

## Source availability

Production source code remains private. This is a documentation showcase, not a runnable application or an open-source release. No client records, credentials, proprietary source files, or internal database schemas are included.

## Rights

Copyright © 2026 Marco Alvarado. All rights reserved. Product names and third-party marks belong to their respective owners. Publication of this showcase does not license the production software.
