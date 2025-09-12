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
- 🔷 **Decision** = Condition check (e.g. Opened? Converted?)
- 🟨 **CRM Update** = Tag in database (e.g. Converted, Inactive)
- 🟥 **End** = Exit point

## Email Examples

- **Day 0 – Welcome Email**</br>
  <!-- ![Welcome Email Mockup](email-mockups/welcome.png) -->
  _Subject_: Welcome to [Product] — here’s your first quick win  
  _Purpose_: Guide users to quick setup and highlight immediate value.
  _Body_:
```
Hi [First Name],

Welcome to [Product]! You’re all set to start your free trial.
To help you get the most value right away, we’ve put together a quick 2-minute setup guide:

[CTA Button][Get Started Now]

The sooner you explore, the faster you’ll see how [Product] can [core benefit, e.g. save you time / improve your workflow].

Cheers,
The [Product] Team
```
---

- **Day 2 – Feature Email (Active Users)**</br>
  <!-- ![Feature Email Mockup](email-mockups/feature.png) -->
  _Subject_: Unlock the feature our power users love most
  _Purpose_: Drive activation of key product feature.
  _Body (plain text)_:

---

- **Day 2 – Nudge Email (Inactive Users)**</br>
  <!-- ![Nudge Email Mockup](email-mockups/nudge.png) -->
  _Subject_: Haven’t had a chance to explore? Here’s why it’s worth it
  _Purpose_: Reactivate inactive users with a value reminder.
  _Body (plain text)_:

---

- **Day 5 – Upgrade Offer**</br>
  <!-- ![Upgrade Offer Mockup](email-mockups/upgrade.png) -->
  _Subject_: Your trial is almost up — upgrade today and save 20%
  _Purpose_: Create urgency, push trial users to paid plan.
  _Body (plain text)_:

## Results (Hypothetical)

- 40% open rate (Welcome Email)
- 12% CTR (Feature Highlight)
- 8% reactivation rate (Nudge Email)
- 15% trial-to-paid conversion uplift (Upgrade Offer)
