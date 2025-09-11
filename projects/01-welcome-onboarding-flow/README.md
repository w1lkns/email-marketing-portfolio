# Welcome & Onboarding Flow

## Goal

The goal of this flow is to activate trial users within their first week by delivering early value. Engaged users receive a feature highlight, while inactive users get a reminder email to reduce drop-off. The flow is designed around a 5-day trial period but can be adapted to different timelines.

## Strategy

- Trigger: New signup
- Segments: Active vs inactive users
- Channels: Email
- KPIs: Activation %, Conversion %, CTR

## Flow Diagram

![Welcome Flow](diagram.png)

### Legend

- 🟨 **Trigger** = Signup event
- 🟪 **Email** = Automated email step
- ⬦ **Decision** = Condition check (e.g. Opened? Converted?)
- 🟨 **CRM Update** = Tag in database (e.g. Converted, Inactive)
- 🟥 **End** = Exit point

## Email Examples

- **Day 0 – Welcome Email**: Quick start guide + value proposition.
- **Day 2 – Feature Highlight**: Showcase a key feature that drives activation.
- **Day 2 – Nudge Email**: Reminder for inactive users, stressing benefits.
- **Day 5 – Upgrade Offer**: Discount or benefit for moving to paid plan.

## Results (Hypothetical)

- 40% open rate (Welcome Email)
- 12% CTR (Feature Highlight)
- 8% reactivation rate (Nudge Email)
- 15% trial-to-paid conversion uplift (Upgrade Offer)
