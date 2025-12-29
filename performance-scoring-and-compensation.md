# 💰 Performance Scoring and Compensation

<figure><img src=".gitbook/assets/Design sem nome (3).png" alt=""><figcaption></figcaption></figure>

## How Performance Turns Into Rewards

The Cellframe Ambassador Program does not reward presence. It rewards measurable contribution.

Compensation is distributed through a points based model combined with fixed monthly pools. Each activity has a defined weight. The more relevant and verified value you deliver, the larger your share of the pool.

This module explains:

* How points are earned per activity
* What the hard caps are
* How points convert into USD
* How the Effective Pool works
* How the 100 point multiplier works

#### Seasons & Evaluation Cycles

#### The Cellframe Ambassador Program operates in monthly Seasons.

> Each Season represents a complete evaluation cycle, including activity execution, performance measurement, scoring, and reward distribution.
>
> Points, leaderboards, and eligibility reset at the beginning of every Season.

#### Threshold Progression by Season

> During the first two Seasons, a reduced eligibility threshold of 30 points may be applied to support onboarding and adaptation.
>
> From Season 3 onward, the standard eligibility threshold of 40 points applies.

#### Why Seasons Matter

> Treating each month as a Season reinforces performance based participation. Rewards are earned per Season, not accumulated by tenure.

***

## The Season Performance Cycle

{% stepper %}
{% step %}
### Ambassadors execute activities aligned with their category

Ambassadors perform the activities expected for their category throughout the month.
{% endstep %}

{% step %}
### Activities are tracked

Tracking is performed via bots, tools, and manual validation.
{% endstep %}

{% step %}
### Monthly activity report submission

A monthly activity report is submitted. No report means no points.
{% endstep %}

{% step %}
### Points are assigned

Points are assigned per activity category based on the rules for each category.
{% endstep %}

{% step %}
### Eligible ambassadors share the pool

Eligible ambassadors share the Effective Pool proportionally based on Weighted\_Points.
{% endstep %}
{% endstepper %}

No report means no points. No points means no payment.

***

## General Payment Rules

To be eligible for payment in a given month, an ambassador must:

* Reach the minimum points threshold for their category
* Submit a valid monthly report within the reporting window
* Deliver verifiable, non-spam, non-botted activity

Eligibility grants access to the pool. It does not guarantee a fixed payout.

***

## Monthly Pools

* Regional Ambassadors: USD X pool
* Rising Ambassadors: USD Y pool

Core Ambassadors are compensated under individual agreements and do not participate in pooled distribution.

***

## Regional Ambassadors - Scoring Breakdown (Monthly)

**Maximum: 100 points**\
**Payment eligibility threshold: 40 points**

### Community Growth (Quality Based) - up to 30 points

* 5 quality members verified on local telegram or discord: 15 points
* 20 or more quality members verified on local telegram or discord (not cumulative): 30 points

Rules:

* Only real, non spam members count
* Growth below 5 quality members scores zero points

***

### Localized Content - up to 25 points (based on manual report)

* 7 quality contents (posts, articles, guides, translations): 10 points
* 15 quality contents: 25 points

Rules:

* Content must be original and relevant
* Hard cap applies regardless of volume

Points are capped and assigned manually

***

### Community Activity & Support - up to 15 points

Evaluated qualitatively based on:

* Presence and responsiveness
* Engajament quality and quantity
* Helpfulness to users

Tracked automatically via Telegram Bot and measured monthly&#x20;

***

### Raid Participation - up to 10 points

* Active and consistent participation: 10 points

Tracked automatically via the official raid bot on telegram.

***

### Events & Initiatives - up to 20 points

* One approved online or offline event: 20 points

Rules:

* Proof required (photos, recordings, agenda, attendance)
* Maximum one event counted per month

***

## Rising Ambassadors - Scoring Breakdown

**Maximum: 100 points**\
**Payment eligibility threshold: 40 points**

{% stepper %}
{% step %}
### Leaderboard Position - up to 50 points

* Top 10 Rising Ambassadors: 50 points
* Positions 11 to 50: 40 points
* Positions 51 to 100: 30 points

Leaderboard resets monthly.
{% endstep %}

{% step %}
### Mission Completion - up to 25 points

* 80% completion: 18 points
* 100% completion: 25 points

Tracked via mission forms or bots.
{% endstep %}

{% step %}
### Consistency & Behavior in community chats - up to 25 points

Qualitative evaluation based on:

* Monthly activity
* Reliability
* Alignment with community standards
{% endstep %}
{% endstepper %}

***

## Effective Pool Model

### Why it exists

If the category underdelivers, it is not fair for the same category to drain the entire Monthly Pool.

The Effective Pool model makes distribution proportional to how much the category collectively delivered.

### Step 1: Compute the category average performance ratio

For each ambassador:

Performance\_Ratio\_i = Points\_i / 100

Then:

Average\_Performance\_Ratio = (Sum of all Performance\_Ratio\_i) / N

### Step 2: Compute the Effective Pool

Effective\_Pool = Monthly\_Pool × Average\_Performance\_Ratio

Only the Effective Pool is distributed. The remainder stays reserved.

Reserved\_Amount = Monthly\_Pool − Effective\_Pool

### Practical result

* High performance month: most of the pool is distributed
* Low performance month: a large portion stays reserved

This pushes the category to improve, without needing drama or subjective decisions.

***

## Excellence Multiplier for 100 Point Performers

### Why it exists

In large groups, being the only person to hit 100 points can still produce a weak payout if the rest of the category underdelivers.

To keep excellence meaningful, 100 point performers can receive a multiplier applied to their points only for payment weighting.

### Recommended rule

If Points\_i = 100, then:

Weighted\_Points\_i = Points\_i × M

Where M is typically **1.25**.

If Points\_i < 100:

Weighted\_Points\_i = Points\_i

Distribution uses Weighted\_Points, but the Effective Pool still uses real points for performance ratio. That keeps the system honest.

***

## Payment Formula (Final)

{% stepper %}
{% step %}
### Compute the Effective\_Pool

Use Average\_Performance\_Ratio to calculate Effective\_Pool = Monthly\_Pool × Average\_Performance\_Ratio.
{% endstep %}

{% step %}
### Compute Weighted\_Points for distribution

Apply the Excellence Multiplier to any 100-point performers; others keep their points as-is.
{% endstep %}

{% step %}
### Filter eligible ambassadors

Only ambassadors who meet eligibility (points threshold, valid report, verified activity) are included.
{% endstep %}

{% step %}
### Compute individual payments

Payment\_i = (Weighted\_Points\_i / Total\_Weighted\_Points\_Eligible) × Effective\_Pool
{% endstep %}
{% endstepper %}

***

## Examples

### Example A: 10 Regional Ambassadors, Monthly Pool USD 1,000

Only 2 hit 100 points. The other 8 are below 60.

Assume:

* 2 ambassadors: 100 pts
* 4 ambassadors: 50 pts
* 4 ambassadors: 40 pts

Average performance ratio: (1.0 + 1.0 + (0.5 × 4) + (0.4 × 4)) / 10\
(2.0 + 2.0 + 1.6) / 10 = 5.6 / 10 = 0.56

Effective Pool: 1000 × 0.56 = USD 560\
Reserved = USD 440

If multiplier M = 1.25:

* Each 100 pt becomes 125 weighted points

Total weighted points: (125 × 2) + (50 × 4) + (40 × 4)\
250 + 200 + 160 = 610

Payouts:

* 100 pt performer: (125 / 610) × 560 ≈ USD 114.75 each
* 50 pt performer: (50 / 610) × 560 ≈ USD 45.90 each
* 40 pt performer: (40 / 610) × 560 ≈ USD 36.72 each

***

### Example B: 25 Regional Ambassadors, Monthly Pool USD 700

Only 1 person hits 100 points. The other 24 are below 100.

Assume:

* 1 ambassador: 100 pts
* 6 ambassadors: 70 pts
* 10 ambassadors: 50 pts
* 8 ambassadors: 40 pts

Average performance ratio: (1.0 + (0.7 × 6) + (0.5 × 10) + (0.4 × 8)) / 25\
(1.0 + 4.2 + 5.0 + 3.2) / 25 = 13.4 / 25 = 0.536

Effective Pool: 700 × 0.536 = USD 375.20\
Reserved = USD 324.80

Apply multiplier M = 1.25 to the 100 pt performer:

* 100 pts → 125 weighted points

Total weighted points: 125 + (70 × 6) + (50 × 10) + (40 × 8)\
125 + 420 + 500 + 320 = 1365

Payouts:

* 100 pt performer: (125 / 1365) × 375.20 ≈ USD 34.36
* 70 pt performer: (70 / 1365) × 375.20 ≈ USD 19.25 each
* 50 pt performer: (50 / 1365) × 375.20 ≈ USD 13.74 each
* 40 pt performer: (40 / 1365) × 375.20 ≈ USD 10.99 each

***

## Two Extreme Scenarios (Stress Tests)

<details>

<summary>Stress Test 1: Very strong month</summary>

* 25 ambassadors
* Average points = 90
* Monthly Pool = USD 700

Average ratio = 0.90\
Effective Pool = 700 × 0.90 = USD 630\
Reserved = USD 70

Result: almost the whole pool is distributed, because the category performed.

</details>

<details>

<summary>Stress Test 2: Very weak month</summary>

* **6 ambassadors**
* **Only 1 hits 100**
* **1 hits 80**
* **Everyone else averages 60**
* **Monthly Pool = USD 300**

Average ratio = (1.0 + 0.8 + (0.6 × 4)) / 6\
(1.0 + 0.8 + 2.4) / 6 = 4.2 / 6 = **0.70**

Effective Pool = 300 × 0.70 = **USD 210.00**\
Reserved = **USD 90.00**

Result: the category cannot drain the full pool on a weak month.

</details>

***

### Important Clarifications

* Points reset every month.
* Hard caps are enforced to prevent metric abuse.
* Manual validation overrides automation whenever quality is questionable.
* Cellframe reserves the right to invalidate low quality, artificial, or manipulated activity.

#### Reserved Pool & Rebase Logic

* Any undistributed portion of the Monthly Pool becomes a **Reserved Pool**.
* The Reserved Pool is carried forward to the next season.
* In the following month, the protocol **only tops up the pool to reach the Effective Pool unlocked by collective performance**.
* This creates a balanced rebase mechanism where strong performance unlocks higher rewards, and weak performance naturally reduces spending without penalizing contributors.

#### Eligibility and Threshold Handling

* Ambassadors who fail to meet the minimum eligibility threshold do not receive payments for the month.
* Their performance is still included in the category's average performance calculation used to determine how much of the Monthly Pool is unlocked.

***

## Final Note

This model is intentionally strict.

It rewards consistency, quality, and real impact. Spam, shortcuts, and artificial engagement do not survive this system.
