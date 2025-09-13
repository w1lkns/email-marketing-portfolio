# Churn Reduction Flow

## Goal

Reduce voluntary churn by re-engaging at-risk customers before cancellation. The flow aims to remind users of the value they’re getting, reinforce trust with social proof, and offer a last-chance incentive to retain them.

## Strategy

- Trigger: Low activity in last 14 days || Attempt to cancel or downgrade
- Segments: at-risk (inactive + downgrade intent) vs active (no action taken, excluded from the flow)
- Channels: Email (plus in-app if relevant)  
- Timing: 2–3 touches across the final 14 days before cancellation/renewal
- KPIs: Retention rate, CTR, “Save offer” acceptance, Reduced cancellations

## Flow Diagram

![Churn Flow](diagram-churn.png)

### Legend

- 🟨 **Trigger** = Inactivity or cancel intent event  
- 🟪 **Email** = Automated email step  
- 🔷 **Decision** = Condition check (e.g. Opened? Clicked? Accepted?)  
- ⏱️ **Delay** = Wait period before next step (e.g. 24h, 72h, 96h)  
- 🟨 **CRM Update** = Tag in database (e.g. Retained, Churned)  
- 🟥 **End** = Exit point  


## Email Examples
_Note: Personalisation tokens shown in generic format for clarity. Actual syntax varies by ESP (e.g., {$name} in MailerLite)._

- **Email #1 – Value Reminder**  
  **Subject**: Keep [Product] working for you every day  
  **Preheader**: [Feature] makes your work easier — don’t lose it now  
  **Purpose**: Remind users of the product’s core value and benefits they’ve already experienced  
  **Body (plain text)**:  

```
Hello [First Name|there],

We noticed you haven’t been as active in [Product] recently.  
Before you make any changes, here’s what [Product] is already doing for you:

• [Feature 1] — helps you [save time / reduce effort]  
• [Feature 2] — gives you [clearer insights / faster results]  
• [Feature 3] — trusted by [X,000] users every day  

Your account is still active — log back in today and keep those benefits working for you:  

[CTA Button: Continue with [Product]]

Cheers,
The [Product] Team
```

<!-- ![Value Reminder Email Mockup](email-mockups/value-mockup.png) -->
---

- **Email #2 – Success Story (Proof/Trust Builder)**  
  **Subject**: See how [Client] achieved [outcome] with [Product]  
  **Preheader**: Real results that you could be getting too  
  **Purpose**: Reinforce credibility with a case study or testimonial, show that others succeed, so they can too  
  **Body (plain text)**:  

```
Hello [First Name|there],

Still on the fence about [Product]? You’re not alone, many of our customers 
started in the same place.

Here’s how [Client Name] turned things around:
• Challenge: [They were struggling with X problem]  
• Solution: They activated [Feature] in [Product]  
• Result: Within [timeframe], they achieved [specific measurable outcome]  

Their story is just one of thousands and your account is still ready to 
deliver the same results.  

[CTA Button: Try It Again]

See what’s possible when you give [Product] another chance.

Cheers,
The [Product] Team
```
<!-- ![Success Story Email Mockup](email-mockups/success-story.png) -->
---

- **Email #3 – Save Offer**  
  **Subject**: Enjoy 20% off your next 3 months  
  **Preheader**: A limited offer to keep [Product] working for you  
  **Purpose**: Provide a financial or feature-based incentive as the last attempt to retain the user  
  **Body (plain text)**:  

```
Hello [First Name|there],

We’d love for you to keep working with [Product].  
To make your decision easier, here’s an exclusive offer:  

Save 20% on your next 3 months when you continue your subscription today.  

By staying, you’ll keep access to everything you already rely on:  
• [Feature 1] — [specific outcome]  
• [Feature 2] — [specific outcome]  
• [Premium support/benefit]  

This special offer expires when your subscription is set to end on [date].  

[CTA Button: Claim My 20% Discount]

If you have questions, just reply to this email, our team is available 24/7.  

Cheers,
The [Product] Team
```
<!-- ![Save Offer Email Mockup](email-mockups/offer.png) -->

## Results (Hypothetical)
- 18% of at-risk users re-engaged after receiving the Value Reminder
- 10% retention uplift among those exposed to the Success Story vs. control
- 22% Save Offer acceptance rate
- Overall churn reduced by 12% in test cohort

## Insights
- Timing matters: Engaged users responded best when offered the Save incentive within 24h of re-engagement, while inactive users needed longer delays (72h, 96h).
- Proof before discount: The Success Story email built credibility and softened resistance — making the Save Offer feel like added value rather than a desperate discount.
- Not all users should see offers: Reserving incentives only for high-risk users prevented revenue leakage from healthy accounts.
- Personalization increases trust: Using customer names, relevant features, and outcomes raised CTRs vs. generic reminders.

**Conclusion**: A structured churn reduction sequence can significantly cut voluntary churn by combining value reminders, social proof, and targeted save incentives, while protecting revenue by limiting discounts to truly at-risk users.
