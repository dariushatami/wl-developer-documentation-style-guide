In WellnessLiving, our customers set up class schedules, manage client records, and pull business reports through APIs and the web portal. Accurate metadata ensures that every tutorial, reference page, and code sample is discoverable and accessible.

Outlined below are various best practices related to metadata to consider.

## Page titles and headings

* Your H1 should reflect the customer’s goal (e.g. “Automating Class Waitlist Notifications”).
* Use H2 for discrete steps (“Create Notification Template,” “Subscribe to Waitlist Events”).

## Image and diagram alt text

* Every visual (e.g., UI screenshots, flow diagrams, architecture diagrams) needs `alt=` that summarizes its function.
* Complex diagrams require a caption or short paragraph below to flesh out details.

## Structured frontmatter and tags

* Include metadata to filter by use case.

YAML example:
``` yaml
title: Setting Up Webhooks
version: v2.1
tags:
  - webhooks
  - api
audience: external
layout: guide
```