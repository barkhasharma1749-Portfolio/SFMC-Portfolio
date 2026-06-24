# Journey Builder

## Overview

Journey Builder is a powerful Salesforce Marketing Cloud tool used to create automated, personalized customer journeys across multiple channels such as Email, SMS, Push Notifications, and Mobile Messaging.

It helps marketers engage customers at the right time with the right message based on customer behavior and interactions.

## Skills Covered

* Customer Journey Design
* Entry Sources
* Decision Splits
* Email Activities
* Wait Activities
* Goal Tracking
* Multi-Channel Marketing
* Customer Lifecycle Automation

---

## Project 1: Welcome Journey

### Objective

Automatically send a welcome email series to newly registered customers.

### Journey Flow

1. Customer Registration
2. Entry Data Extension
3. Welcome Email
4. Wait 2 Days
5. Product Introduction Email
6. Wait 3 Days
7. Promotional Offer Email

### Outcome

Improved customer onboarding and engagement.

---

## Project 2: Re-Engagement Journey

### Objective

Reconnect inactive subscribers who have not engaged in the last 90 days.

### Journey Flow

1. Inactive Subscribers Entry
2. Re-Engagement Email
3. Wait 5 Days
4. Check Open Activity
5. Send Reminder Email
6. Exit Journey

### Outcome

Increased subscriber engagement and reduced inactive audience size.

---

## Project 3: Birthday Journey

### Objective

Send personalized birthday wishes and offers.

### Journey Flow

1. Birthday Date Entry
2. Birthday Email
3. Personalized Discount Offer
4. Journey Exit

### Outcome

Enhanced customer experience through personalized communication.

---

## Project 4: Cart Abandonment Journey

### Objective

Recover lost sales by targeting customers who abandoned their shopping cart.

### Journey Flow

1. Cart Abandonment Event
2. Reminder Email
3. Wait 24 Hours
4. Discount Offer Email
5. Purchase Check
6. Exit Journey

### Outcome

Improved conversion rates and recovered abandoned carts.

---

## Common Journey Builder Activities

### Entry Source

Defines how contacts enter a journey.

Examples:

* Data Extension Entry
* API Event Entry
* Salesforce Data Entry

### Email Activity

Sends marketing emails within a journey.

### Wait Activity

Pauses contacts for a defined period before the next step.

### Decision Split

Routes contacts based on conditions.

Example:

```text
Opened Email?
│
├── Yes → Send Offer
│
└── No → Send Reminder
```

### Goal

Measures journey success based on defined objectives.

Example:

* Purchase Completed
* Form Submitted
* Product Registered

---

## Interview Questions & Answers

### What is Journey Builder?

Journey Builder is a Salesforce Marketing Cloud tool used to create automated, personalized customer journeys based on customer behavior, data, and interactions.

---

### What are Entry Sources in Journey Builder?

Entry Sources define how contacts enter a journey.

Examples:

* Data Extension Entry Source
* API Event Entry Source
* Salesforce Data Entry Source

---

### What is a Decision Split?

Decision Split is used to route contacts to different paths based on specific conditions or customer behavior.

---

### What is the difference between Journey Builder and Automation Studio?

| Journey Builder             | Automation Studio               |
| --------------------------- | ------------------------------- |
| Customer-focused automation | Process-focused automation      |
| Real-time engagement        | Scheduled automation            |
| Uses customer behavior      | Uses data processing activities |
| Personalized journeys       | Backend workflows               |

---

## Tools Used

* Salesforce Marketing Cloud
* Journey Builder
* Email Studio
* Contact Builder
* Data Extensions

---

## Outcome

Designed and implemented automated customer journeys to improve engagement, customer retention, lead nurturing, and overall campaign performance using Salesforce Marketing Cloud Journey Builder.

