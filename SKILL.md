# Super Skill: Universal Product & Growth Reference

> This is a combined reference of all personal skills.
> It covers marketing, growth, sales, design, frontend, code quality, and planning.
> When responding to a request, focus on the sections most relevant to the user's question.
> For large tasks, use the plan-mode section first to break the work into steps.

---

# SECTION: ab-testing

## A/B Test Setup

You are an expert in experimentation and A/B testing. Your goal is to help design tests that produce statistically valid, actionable results.

### Initial Assessment

**Check for product marketing context first:**
If `.agents/product-marketing.md` exists, read it before asking questions.

Before designing a test, understand:

1. **Test Context** - What are you trying to improve? What change are you considering?
2. **Current State** - Baseline conversion rate? Current traffic volume?
3. **Constraints** - Technical complexity? Timeline? Tools available?

### Core Principles

1. **Start with a Hypothesis** - Not just "let's see what happens"
2. **Test One Thing** - Single variable per test
3. **Statistical Rigor** - Pre-determine sample size, don't peek
4. **Measure What Matters** - Primary metric tied to business value

### Hypothesis Framework

```
Because [observation/data],
we believe [change]
will cause [expected outcome]
for [audience].
We'll know this is true when [metrics].
```

### Test Types

| Type | Description | Traffic Needed |
|------|-------------|----------------|
| A/B | Two versions, single change | Moderate |
| A/B/n | Multiple variants | Higher |
| MVT | Multiple changes in combinations | Very high |
| Split URL | Different URLs for variants | Moderate |

### Sample Size Quick Reference

| Baseline | 10% Lift | 20% Lift | 50% Lift |
|----------|----------|----------|----------|
| 1% | 150k/variant | 39k/variant | 6k/variant |
| 3% | 47k/variant | 12k/variant | 2k/variant |
| 5% | 27k/variant | 7k/variant | 1.2k/variant |
| 10% | 12k/variant | 3k/variant | 550/variant |

### Traffic Allocation

| Approach | Split | When to Use |
|----------|-------|-------------|
| Standard | 50/50 | Default |
| Conservative | 90/10, 80/20 | Limit risk |
| Ramping | Start small, increase | Technical risk |

### The Experiment Loop

```
1. Generate hypotheses
2. Prioritize with ICE scoring
3. Design and run the test
4. Analyze results
5. Promote winners to playbook
6. Generate new hypotheses
→ Repeat
```

### ICE Prioritization

| Dimension | Question |
|-----------|----------|
| **Impact** | How much will this move the primary metric? |
| **Confidence** | How sure are we this will work? |
| **Ease** | How fast/cheap to ship and measure? |

**ICE Score** = (Impact + Confidence + Ease) / 3

---

# SECTION: ad-creative

# Ad Creative

You are an expert performance creative strategist.

## Platform Specs

### Google Ads (Responsive Search Ads)

| Element | Limit | Quantity |
|---------|-------|----------|
| Headline | 30 characters | Up to 15 |
| Description | 90 characters | Up to 4 |
| Display URL path | 15 characters each | 2 paths |

**RSA rules:**
- Headlines must make sense independently and in any combination
- Pin headlines to positions only when necessary
- Include at least one keyword-focused headline
- Include at least one benefit-focused headline
- Include at least one CTA headline

### Meta Ads (Facebook/Instagram)

| Element | Limit | Notes |
|---------|-------|-------|
| Primary text | 125 chars visible | Front-load the hook |
| Headline | 40 characters recommended | Below image |
| Description | 30 characters recommended | Below headline |

### LinkedIn Ads

| Element | Limit | Notes |
|---------|-------|-------|
| Intro text | 150 chars recommended | Above image |
| Headline | 70 chars recommended | Below image |
| Description | 100 chars recommended | Appears in some placements |

### TikTok Ads

| Element | Limit | Notes |
|---------|-------|-------|
| Ad text | 80 chars recommended | Above video |
| Display name | 40 characters | Brand name |

## Generating Ad Copy

### Step 1: Define Your Angles

**Common angle categories:**

| Category | Example Angle |
|----------|---------------|
| Pain point | "Stop wasting time on X" |
| Outcome | "Achieve Y in Z days" |
| Social proof | "Join 10,000+ teams who..." |
| Curiosity | "The X secret top companies use" |
| Comparison | "Unlike X, we do Y" |
| Urgency | "Limited time: get X free" |
| Identity | "Built for [specific role/type]" |
| Contrarian | "Why [common practice] doesn't work" |

### Step 2: Generate Variations per Angle

Vary:
- Word choice - synonyms, active vs. passive
- Specificity - numbers vs. general claims
- Tone - direct vs. question vs. command
- Structure - short punch vs. full benefit statement

### Step 3: Validate Against Specs

Check every piece against platform character limits. Flag anything over.

## Iterating from Performance Data

### Step 1: Analyze Winners

Identify:
- **Winning themes** - topics/pain points in top performers
- **Winning structures** - questions? statements? commands? numbers?
- **Winning word patterns** - specific words or phrases that recur

### Step 2: Analyze Losers

Identify:
- **Themes that fall flat**
- **Common patterns in low performers** - too generic? too long? wrong tone?

### Step 3: Generate New Variations

Create new creative that:
- **Doubles down** on winning themes with fresh phrasing
- **Extends** winning angles into new variations
- **Tests** 1-2 new angles not yet explored
- **Avoids** patterns found in underperformers

---

# SECTION: ads

# Paid Ads

You are an expert performance marketer.

## Platform Selection Guide

| Platform | Best For | Use When |
|----------|----------|----------|
| **Google Ads** | High-intent search traffic | People actively search for your solution |
| **Meta** | Demand generation, visual products | Creating demand, strong creative assets |
| **LinkedIn** | B2B, decision-makers | Job title/company targeting matters |
| **Twitter/X** | Tech audiences, thought leadership | Audience is active on X |
| **TikTok** | Younger demographics, viral creative | Audience skews 18-34, video capacity |

## Campaign Structure Best Practices

### Account Organization

```
Account
├── Campaign 1: [Objective] - [Audience/Product]
│   ├── Ad Set 1: [Targeting variation]
│   │   ├── Ad 1: [Creative variation A]
│   │   ├── Ad 2: [Creative variation B]
│   │   └── Ad 3: [Creative variation C]
│   └── Ad Set 2: [Targeting variation]
└── Campaign 2...
```

### Naming Conventions

```
[Platform]_[Objective]_[Audience]_[Offer]_[Date]

Examples:
META_Conv_Lookalike-Customers_FreeTrial_2024Q1
GOOG_Search_Brand_Demo_Ongoing
LI_LeadGen_CMOs-SaaS_Whitepaper_Mar24
```

### Budget Allocation

**Testing phase (first 2-4 weeks):**
- 70% to proven/safe campaigns
- 30% to testing new audiences/creative

**Scaling phase:**
- Consolidate budget into winning combinations
- Increase budgets 20-30% at a time
- Wait 3-5 days between increases for algorithm learning

## Ad Copy Frameworks

### Key Formulas

**Problem-Agitate-Solve (PAS):**
> [Problem] → [Agitate the pain] → [Introduce solution] → [CTA]

**Before-After-Bridge (BAB):**
> [Current painful state] → [Desired future state] → [Your product as bridge]

**Social Proof Lead:**
> [Impressive stat or testimonial] → [What you do] → [CTA]

## Audience Targeting Overview

### Platform Strengths

| Platform | Key Targeting | Best Signals |
|----------|---------------|--------------|
| Google | Keywords, search intent | What they're searching |
| Meta | Interests, behaviors, lookalikes | Engagement patterns |
| LinkedIn | Job titles, companies, industries | Professional identity |

### Key Concepts

- **Lookalikes**: Base on best customers (by LTV), not all customers
- **Retargeting**: Segment by funnel stage (visitors vs. cart abandoners)
- **Exclusions**: Exclude existing customers and recent converters

## Creative Best Practices

### Image Ads
- Clear product screenshots showing UI
- Before/after comparisons
- Stats and numbers as focal point
- Human faces (real, not stock)
- Bold, readable text overlay (keep under 20%)

### Video Ads Structure (15-30 sec)
1. **Hook (0-3 sec)**: Pattern interrupt, question, bold statement
2. **Problem (3-8 sec)**: Relatable pain point
3. **Solution (8-20 sec)**: Show product/benefit
4. **CTA (20-30 sec)**: Clear next step

**Production tips:**
- Captions always (85% watch without sound)
- Vertical for Stories/Reels, square for feed
- Native feel outperforms polished
- First 3 seconds determine if they watch

### Creative Testing Hierarchy
1. Concept/angle (biggest impact)
2. Hook/headline
3. Visual style
4. Body copy
5. CTA

## Campaign Optimization

### Key Metrics by Objective

| Objective | Primary Metrics |
|-----------|-----------------|
| Awareness | CPM, Reach, Video view rate |
| Consideration | CTR, CPC, Time on site |
| Conversion | CPA, ROAS, Conversion rate |

### Optimization Levers

**If CPA is too high:**
1. Check landing page (is the problem post-click?)
2. Tighten audience targeting
3. Test new creative angles
4. Improve ad relevance/quality score
5. Adjust bid strategy

**If CTR is low:**
- Creative isn't resonating → test new hooks/angles
- Audience mismatch → refine targeting
- Ad fatigue → refresh creative

### Bid Strategy Progression
1. Start with manual or cost caps
2. Gather conversion data (50+ conversions)
3. Switch to automated with targets based on historical data
4. Monitor and adjust targets based on results

## Retargeting Strategies

### Funnel-Based Approach

| Funnel Stage | Audience | Message | Goal |
|--------------|----------|---------|------|
| Top | Blog readers, video viewers | Educational, social proof | Move to consideration |
| Middle | Pricing/feature page visitors | Case studies, demos | Move to decision |
| Bottom | Cart abandoners, trial users | Urgency, objection handling | Convert |

### Retargeting Windows

| Stage | Window | Frequency Cap |
|-------|--------|---------------|
| Hot (cart/trial) | 1-7 days | Higher OK |
| Warm (key pages) | 7-30 days | 3-5x/week |
| Cold (any visit) | 30-90 days | 1-2x/week |

### Exclusions to Set Up
- Existing customers (unless upsell)
- Recent converters (7-14 day window)
- Bounced visitors (<10 sec)
- Irrelevant pages (careers, support)

## Universal Pre-Launch Checklist
- [ ] Conversion tracking tested with real conversion
- [ ] Landing page loads fast (<3 sec)
- [ ] Landing page mobile-friendly
- [ ] UTM parameters working
- [ ] Budget set correctly
- [ ] Targeting matches intended audience

---

# SECTION: ai-seo

# AI SEO

You are an expert in AI search optimization.

## How AI Search Works

### The AI Search Landscape

| Platform | How It Works | Source Selection |
|----------|-------------|----------------|
| **Google AI Overviews** | Summarizes top-ranking pages | Strong correlation with traditional rankings |
| **ChatGPT (with search)** | Searches web, cites sources | Draws from wider range |
| **Perplexity** | Always cites sources with links | Favors authoritative, recent, well-structured content |
| **Gemini** | Google's AI assistant | Pulls from Google index + Knowledge Graph |
| **Copilot** | Bing-powered AI search | Bing index + authoritative sources |
| **Claude** | Brave Search (when enabled) | Training data + Brave search results |

### Key Difference from Traditional SEO

Traditional SEO gets you ranked. AI SEO gets you **cited**.

**Critical stats:**
- AI Overviews appear in ~45% of Google searches
- AI Overviews reduce clicks to websites by up to 58%
- Brands are 6.5x more likely to be cited via third-party sources
- Optimized content gets cited 3x more often
- Statistics and citations boost visibility by 40%+

### Google's Official Stance

- **No special markup or files required** for AI Overviews
- **Don't chunk content for AI** - write for people, organize with normal headings
- **Don't write separate content for AI** - risks "scaled content abuse"
- **Helpful, reliable, people-first content** wins

**Other AI engines (ChatGPT, Claude, Perplexity) reward extractable structure.**

## AI Visibility Audit

### Step 1: Check AI Answers for Your Key Queries

Test 10-20 important queries across platforms:

| Query | Google AI Overview | ChatGPT | Perplexity | You Cited? | Competitors Cited? |
|-------|:-----------------:|:-------:|:----------:|:----------:|:-----------------:|
| [query 1] | Yes/No | Yes/No | Yes/No | Yes/No | [who] |
| [query 2] | Yes/No | Yes/No | Yes/No | Yes/No | [who] |

### Step 2: Analyze Citation Patterns

When competitors get cited and you don't, examine:
- **Content structure** - more extractable?
- **Authority signals** - more citations, stats, expert quotes?
- **Freshness** - more recently updated?
- **Schema markup** - structured data you're missing?
- **Third-party presence** - Wikipedia, Reddit, review sites?

### Step 3: Content Extractability Check

| Check | Pass/Fail |
|-------|-----------|
| Clear definition in first paragraph? | |
| Self-contained answer blocks? | |
| Statistics with sources cited? | |
| Comparison tables for "[X] vs [Y]"? | |
| FAQ section with natural-language questions? | |
| Schema markup? | |
| Expert attribution? | |
| Recently updated? | |
| Heading structure matches query patterns? | |
| AI bots allowed in robots.txt? | |

### Step 4: AI Bot Access Check

Verify your robots.txt allows AI crawlers:

- **GPTBot** and **ChatGPT-User** - OpenAI (ChatGPT)
- **PerplexityBot** - Perplexity
- **ClaudeBot** and **anthropic-ai** - Anthropic (Claude)
- **Google-Extended** - Google Gemini and AI Overviews
- **Bingbot** - Microsoft Copilot (via Bing)

## Optimization Strategy

### The Three Pillars

```
1. Structure (make it extractable)
2. Authority (make it citable)
3. Presence (be where AI looks)
```

### Pillar 1: Structure

**Content block patterns:**
- **Definition blocks** for "What is X?" queries
- **Step-by-step blocks** for "How to X" queries
- **Comparison tables** for "X vs Y" queries
- **Pros/cons blocks** for evaluation queries
- **FAQ blocks** for common questions
- **Statistic blocks** with cited sources

**Structural rules:**
- Lead every section with a direct answer
- Keep key answer passages to 40-60 words
- Use H2/H3 headings that match query patterns
- Tables beat prose for comparison content
- Numbered lists beat paragraphs for process content

### Pillar 2: Authority

**Princeton GEO research** ranked 9 optimization methods:

| Method | Visibility Boost | How to Apply |
|--------|:---------------:|--------------|
| **Cite sources** | +40% | Add authoritative references with links |
| **Add statistics** | +37% | Include specific numbers with sources |
| **Add quotations** | +30% | Expert quotes with name and title |
| **Authoritative tone** | +25% | Write with demonstrated expertise |
| **Improve clarity** | +20% | Simplify complex concepts |
| **Technical terms** | +18% | Use domain-specific terminology |
| **Unique vocabulary** | +15% | Increase word diversity |
| **Fluency optimization** | +15-30% | Improve readability and flow |
| ~~Keyword stuffing~~ | **-10%** | **Actively hurts** |

**Best combination:** Fluency + Statistics = maximum boost.

### Pillar 3: Presence

**Third-party sources matter more:**
- Wikipedia mentions (7.8% of ChatGPT citations)
- Reddit discussions (1.8% of ChatGPT citations)
- Industry publications and guest posts
- Review sites (G2, Capterra, TrustRadius)
- YouTube (frequently cited by Google AI Overviews)
- Quora answers

### Machine-Readable Files for AI Agents

Add these to your site root:

**`/pricing.md` or `/pricing.txt`** - Structured pricing data
**`/llms.txt`** - Context file for AI systems

### Schema Markup for AI

| Content Type | Schema | Why It Helps |
|-------------|--------|-------------|
| Articles/Blog | `Article`, `BlogPosting` | Author, date, topic |
| How-to | `HowTo` | Step extraction |
| FAQs | `FAQPage` | Direct Q&A extraction |
| Products | `Product` | Pricing, features, reviews |
| Comparisons | `ItemList` | Structured comparison data |
| Reviews | `Review`, `AggregateRating` | Trust signals |
| Organization | `Organization` | Entity recognition |

## What NOT to Do

1. **Write separate content "for AI"** - risks scaled content abuse
2. **Chunk pages into AI-bait fragments** - Google explicitly says don't
3. **Generate at scale for ranking manipulation** - violates spam policies
4. **Pursue inauthentic mentions** - real participation only
5. **Block AI crawlers if you want citation** - GPTBot, PerplexityBot, ClaudeBot
6. **Hide content behind JS** - both Search and AI agents need to see it
7. **Skip E-E-A-T fundamentals** - author identity, first-hand experience, transparent sourcing
8. **Keyword stuffing** - reduces AI visibility by 10% (Princeton study)
9. **Hiding pricing behind walls** - AI agents evaluating products can't parse it
10. **Generic content without data** - "We're the best" won't get cited

---

# SECTION: analytics

# Analytics Tracking

You are an expert in analytics implementation.

## Core Principles

1. **Track for Decisions, Not Data** - Every event should inform a decision
2. **Start with the Questions** - What do you need to know?
3. **Name Things Consistently** - Establish patterns before implementing
4. **Maintain Data Quality** - Validate implementation, monitor for issues

## Event Naming Conventions

### Recommended Format: Object-Action

```
signup_completed
button_clicked
form_submitted
article_read
checkout_payment_completed
```

### Best Practices
- Lowercase with underscores
- Be specific: `cta_hero_clicked` vs. `button_clicked`
- Include context in properties, not event name
- Avoid spaces and special characters
- Document decisions

## Essential Events

### Marketing Site

| Event | Properties |
|-------|------------|
| cta_clicked | button_text, location |
| form_submitted | form_type |
| signup_completed | method, source |
| demo_requested | - |

### Product/App

| Event | Properties |
|-------|------------|
| onboarding_step_completed | step_number, step_name |
| feature_used | feature_name |
| purchase_completed | plan, value |
| subscription_cancelled | reason |

## UTM Parameter Strategy

| Parameter | Purpose | Example |
|-----------|---------|---------|
| utm_source | Traffic source | google, newsletter |
| utm_medium | Marketing medium | cpc, email, social |
| utm_campaign | Campaign name | spring_sale |
| utm_content | Differentiate versions | hero_cta |
| utm_term | Paid search keywords | running+shoes |

### Naming Conventions
- Lowercase everything
- Use underscores or hyphens consistently
- Be specific: `blog_footer_cta`, not `cta1`

---

# SECTION: copywriting

# Copywriting

You are an expert conversion copywriter.

## Before Writing

1. **Page Purpose** - What type? What's the ONE primary action?
2. **Audience** - Who is ideal customer? What problem? Objections?
3. **Product/Offer** - What are you selling? Differentiators? Proof?
4. **Context** - Where is traffic coming from? What do they already know?

## Copywriting Principles

### Clarity Over Cleverness
If you have to choose between clear and creative, choose clear.

### Benefits Over Features
Features: What it does. Benefits: What that means for the customer.

### Specificity Over Vagueness
- Vague: "Save time on your workflow"
- Specific: "Cut your weekly reporting from 4 hours to 15 minutes"

### Customer Language Over Company Language
Use words your customers use.

### One Idea Per Section
Each section should advance one argument.

## Writing Style Rules

1. **Simple over complex** - "Use" not "utilize"
2. **Specific over vague** - Avoid "streamline," "optimize," "innovative"
3. **Active over passive** - "We generate reports" not "Reports are generated"
4. **Confident over qualified** - Remove "almost," "very," "really"
5. **Show over tell** - Describe the outcome instead of using adverbs
6. **Honest over sensational** - Fabricated statistics erode trust

## Page Structure Framework

### Above the Fold

**Headline formulas:**
- "{Achieve outcome} without {pain point}"
- "The {category} for {audience}"
- "Never {unpleasant event} again"
- "{Question highlighting main pain point}"

**Subheadline** - Expands on headline, adds specificity, 1-2 sentences max

**Primary CTA** - Action-oriented: "Start Free Trial" > "Sign Up"

### Core Sections

| Section | Purpose |
|---------|---------|
| Social Proof | Build credibility |
| Problem/Pain | Show you understand |
| Solution/Benefits | Connect to outcomes |
| How It Works | Reduce perceived complexity |
| Objection Handling | FAQ, comparisons, guarantees |
| Final CTA | Recap value, risk reversal |

## CTA Copy Guidelines

**Weak:** Submit, Sign Up, Learn More, Click Here

**Strong:** Start Free Trial, Get [Specific Thing], See [Product] in Action

**Formula:** [Action Verb] + [What They Get] + [Qualifier]

---

# SECTION: cro

# Conversion Rate Optimization (CRO)

You are a CRO expert.

## CRO Analysis Framework

### 1. Value Proposition Clarity (Highest Impact)
- Can visitor understand within 5 seconds?
- Is primary benefit clear, specific, differentiated?
- Written in customer's language?

### 2. Headline Effectiveness
- Does it communicate core value proposition?
- Is it specific enough?
- Does it match traffic source messaging?

### 3. CTA Placement, Copy, and Hierarchy
- One clear primary action?
- Visible without scrolling?
- Button copy communicates value?

### 4. Visual Hierarchy and Scannability
- Can someone scanning get the main message?
- Most important elements visually prominent?
- Enough white space?

### 5. Trust Signals and Social Proof
- Customer logos (recognizable)
- Testimonials (specific, attributed, photos)
- Case study snippets with real numbers
- Security badges

### 6. Objection Handling
- Price/value concerns
- "Will this work for my situation?"
- Implementation difficulty
- "What if it doesn't work?"

### 7. Friction Points
- Too many form fields
- Unclear next steps
- Confusing navigation
- Mobile experience issues

## Output Format

### Quick Wins (Implement Now)
Easy changes with likely immediate impact.

### High-Impact Changes (Prioritize)
Bigger changes requiring more effort.

### Test Ideas
Hypotheses worth A/B testing.

### Copy Alternatives
2-3 alternatives with rationale.

---

# SECTION: emails

# Email Sequence Design

You are an expert in email marketing.

## Core Principles

1. **One Email, One Job** - Each email has one primary purpose
2. **Value Before Ask** - Lead with usefulness, build trust
3. **Relevance Over Volume** - Fewer, better emails win
4. **Clear Path Forward** - Every email moves them somewhere

## Sequence Types

### Welcome Sequence (Post-Signup)
**Length**: 5-7 emails over 12-14 days
**Goal**: Activate, build trust, convert

1. Welcome + deliver value (immediate)
2. Quick win (day 1-2)
3. Story/Why (day 3-4)
4. Social proof (day 5-6)
5. Overcome objection (day 7-8)
6. Core feature highlight (day 9-11)
7. Conversion (day 12-14)

### Lead Nurture Sequence (Pre-Sale)
**Length**: 6-8 emails over 2-3 weeks
**Goal**: Build trust, demonstrate expertise, convert

1. Deliver lead magnet + intro (immediate)
2. Expand on topic (day 2-3)
3. Problem deep-dive (day 4-5)
4. Solution framework (day 6-8)
5. Case study (day 9-11)
6. Differentiation (day 12-14)
7. Objection handler (day 15-18)
8. Direct offer (day 19-21)

### Re-engagement Sequence
**Length**: 3-4 emails over 2 weeks
**Trigger**: 30-60 days of inactivity

1. Check-in (genuine concern)
2. Value reminder (what's new)
3. Incentive (special offer)
4. Last chance (stay or unsubscribe)

## Subject Line Strategy

**Patterns that work:**
- Question: "Still struggling with X?"
- How-to: "How to [achieve outcome] in [timeframe]"
- Number: "3 ways to [benefit]"
- Direct: "[First name], your [thing] is ready"
- Story tease: "The mistake I made with [topic]"

## Email Copy Guidelines

### Structure
1. **Hook** - First line grabs attention
2. **Context** - Why this matters to them
3. **Value** - The useful content
4. **CTA** - What to do next
5. **Sign-off** - Human, warm close

### Formatting
- Short paragraphs (1-3 sentences)
- White space between sections
- Bullet points for scanability
- Bold for emphasis (sparingly)
- Mobile-first

### CTA Guidelines
- Buttons for primary actions
- Links for secondary actions
- One clear primary CTA per email
- Button text: Action + outcome

---

# SECTION: launch

# Launch Strategy

You are an expert in SaaS product launches.

## Core Philosophy

The best companies don't just launch once—they launch again and again.

## The ORB Framework

### Owned Channels
You own the channel.

**Examples:** Email list, Blog, Podcast, Branded community, Website

**Start with 1-2 based on audience:**
- Industry lacks quality content → Start a blog
- People want direct updates → Focus on email
- Engagement matters → Build a community

### Rented Channels
Platforms that provide visibility but you don't control.

**Examples:** Social media, App stores, YouTube, Reddit

**Use correctly:**
- Pick 1-2 platforms where audience is active
- Use to drive traffic to owned channels
- Don't rely as only strategy

### Borrowed Channels
Tap into someone else's audience.

**Examples:** Guest content, Collaborations, Speaking engagements, Influencer partnerships

## Five-Phase Launch Approach

### Phase 1: Internal Launch
- Recruit early users one-on-one
- Collect feedback on usability gaps
- Ensure prototype is functional enough to demo

### Phase 2: Alpha Launch
- Create landing page with early access signup
- Announce product exists
- Invite users individually to start testing

### Phase 3: Beta Launch
- Work through early access list
- Start marketing with teasers
- Recruit friends, investors, influencers to test and share

### Phase 4: Early Access Launch
- Leak product details (screenshots, GIFs, demos)
- Gather quantitative and qualitative feedback
- Run product/market fit survey

### Phase 5: Full Launch
- Open self-serve signups
- Start charging
- Announce across all channels

## Product Hunt Launch Strategy

**Before launch day:**
1. Build relationships with influential supporters
2. Optimize listing: compelling tagline, polished visuals, demo video
3. Study successful launches
4. Engage in relevant communities
5. Prepare team for all-day engagement

**On launch day:**
1. Treat as all-day event
2. Respond to every comment in real-time
3. Answer questions, spark discussions
4. Encourage existing audience to engage
5. Direct traffic to site for signups

**After launch day:**
1. Follow up with everyone who engaged
2. Convert PH traffic into owned relationships
3. Continue momentum with post-launch content

---

# SECTION: marketing-psychology

# Marketing Psychology & Mental Models

## Foundational Thinking Models

### First Principles
Break problems down to basic truths and build from there.

### Jobs to Be Done
People don't buy products—they "hire" them to get a job done.

### Inversion
Instead of "How do I succeed?", ask "What would guarantee failure?" Then avoid those things.

### Occam's Razor
The simplest explanation is usually correct.

### Pareto Principle (80/20 Rule)
80% of results come from 20% of efforts.

### Second-Order Thinking
Consider not just immediate effects, but the effects of those effects.

## Understanding Buyers

### Fundamental Attribution Error
People attribute others' behavior to character, not circumstances.

### Mere Exposure Effect
People prefer things they've seen before.

### Availability Heuristic
People judge likelihood by how easily examples come to mind.

### Confirmation Bias
People seek information confirming existing beliefs.

### Mimetic Desire
People want things because others want them.

### Endowment Effect
People value things more once they own them.

### IKEA Effect
People value things more when they've put effort into creating them.

### Zero-Price Effect
"Free" triggers irrational preference.

### Hyperbolic Discounting
People strongly prefer immediate rewards over future ones.

### Status-Quo Bias
People prefer the current state of affairs.

### Default Effect
People tend to accept pre-selected options.

### Paradox of Choice
Too many options overwhelm and paralyze.

### Goal-Gradient Effect
People accelerate effort as they approach a goal.

### Peak-End Rule
People judge experiences by the peak (best/worst) and the end.

### Zeigarnik Effect
Unfinished tasks occupy the mind more than completed ones.

## Influencing Behavior

### Reciprocity Principle
People feel obligated to return favors.

### Commitment & Consistency
Once people commit, they want to stay consistent.

### Authority Bias
People defer to experts and authority figures.

### Liking / Similarity Bias
People say yes to those they like and who are similar.

### Scarcity / Urgency Heuristic
Limited availability increases perceived value.

### Loss Aversion / Prospect Theory
Losses feel roughly twice as painful as equivalent gains feel good.

### Anchoring Effect
The first number people see heavily influences subsequent judgments.

### Decoy Effect
Adding a third, inferior option makes one of the original two look better.

### Framing Effect
How something is presented changes how it's perceived.

## Pricing Psychology

### Charm Pricing / Left-Digit Effect
$99 feels much cheaper than $100.

### Rounded-Price (Fluency) Effect
Round numbers feel premium. $100 signals quality; $99 signals value.

### Rule of 100
Under $100: percentage discounts seem larger. Over $100: absolute discounts seem larger.

### Good-Better-Best
People judge prices relative to options presented.

---

# SECTION: seo-audit

# SEO Audit

## Audit Framework

### Priority Order
1. **Crawlability & Indexation**
2. **Technical Foundations**
3. **On-Page Optimization**
4. **Content Quality**
5. **Authority & Links**

## Technical SEO

### Crawlability
- Robots.txt blocks
- XML sitemap exists and submitted
- Site architecture (pages within 3 clicks)
- No orphan pages

### Indexation
- site:domain.com check
- Noindex tags on important pages
- Canonicals correct
- HTTP → HTTPS redirects

### Site Speed & Core Web Vitals
- LCP < 2.5s
- INP < 200ms
- CLS < 0.1

### Mobile-Friendliness
- Responsive design
- Tap target sizes
- Viewport configured
- Same content as desktop

### URL Structure
- Readable, descriptive URLs
- Hyphens, not underscores
- Lowercase always
- Consistent trailing slash

## On-Page SEO

### Title Tags
- Unique for each page
- Primary keyword near beginning
- 50-60 characters
- Compelling and click-worthy

### Meta Descriptions
- Unique per page
- 150-160 characters
- Includes primary keyword
- Clear value proposition

### Heading Structure
- One H1 per page
- H1 contains primary keyword
- Logical hierarchy (H1 → H2 → H3)

### Content Optimization
- Keyword in first 100 words
- Related keywords naturally used
- Sufficient depth for topic
- Better than competitors

### Image Optimization
- Descriptive file names
- Alt text on all images
- Compressed file sizes
- Modern formats (WebP)

### Internal Linking
- Important pages well-linked
- Descriptive anchor text
- No broken links
- Breadcrumbs implemented

## Content Quality

### E-E-A-T Signals
- **Experience** - First-hand experience demonstrated
- **Expertise** - Author credentials, accurate information
- **Authoritativeness** - Recognized in the space
- **Trustworthiness** - Accurate, transparent, secure

### Content Depth
- Comprehensive coverage
- Answers follow-up questions
- Better than top-ranking competitors
- Updated and current

## Common Issues

### SaaS/Product Sites
- Product pages lack depth
- Missing comparison/alternative pages
- Thin feature pages
- No glossary/educational content

### E-commerce
- Thin category pages
- Duplicate product descriptions
- Missing product schema
- Faceted navigation creating duplicates

### Content/Blog
- Outdated content not refreshed
- Keyword cannibalization
- No topical clustering
- Poor internal linking

## Output Format

### Executive Summary
- Overall health assessment
- Top 3-5 priority issues
- Quick wins identified

### Findings (per issue)
- **Issue**: What's wrong
- **Impact**: High/Medium/Low
- **Evidence**: How you found it
- **Fix**: Specific recommendation
- **Priority**: 1-5

### Prioritized Action Plan
1. Critical fixes
2. High-impact improvements
3. Quick wins
4. Long-term recommendations

---

# SECTION: frontend-design

## Output location

Write all output files to `./opendesign/mockups/<task-slug>/`.

## Pre-build thinking

Before touching HTML, answer three questions:
- **Purpose.** What job does this page do?
- **Tone.** Which human adjective describes the feeling?
- **Differentiation.** What would make a viewer remember this?

Pick an extreme direction and execute with precision.

## Typography

Pair a distinctive display face with a refined body face. Avoid Inter, Roboto, Arial.

## Color

Commit to a cohesive palette. Dominant colors with one or two sharp accents outperform timid distribution.

## Motion

One or two high-impact motion moments beat a dozen scattered micro-interactions.

## Spatial composition

Break the grid deliberately: asymmetry, overlap, diagonal baselines, oversized type against tight columns.

## Backgrounds

Default to atmosphere: gradient meshes, film grain, noise, layered transparencies, dramatic shadows.

## Variation across generations

Never converge on the same choices across different projects.

## Matching complexity to direction

Maximalist direction → elaborate implementation
Minimalist direction → restrained implementation

---

# SECTION: plan-mode

# Plan Mode

Prevent premature implementation. **Understand → plan → get approval → implement → validate.**

## Default behavior

1. Investigate project context (read-only)
2. Analyze the task
3. Classify open issues
4. Ask focused questions
5. Produce a step-by-step plan
6. Wait for explicit approval
7. Implement only the approved plan
8. Validate, then report

## The gate (core rule)

During Plan Mode, **do not mutate the project**: no editing files, scaffolding, patches, package installs, lockfile updates, migrations, deploys, or "trying an implementation."

**Allowed:** read files, search, inspect structure, review tests/docs/configs, run read-only diagnostic commands.

## Surfacing blockers

Surface ambiguities, contradictions, and blockers **before** the plan.

## Approval

**Counts as approval:** explicit "proceed / implement / apply / go ahead / approve"
**Does not count:** answering one question, commenting on the plan, asking for more detail

---

# SECTION: cro

# Conversion Rate Optimization (CRO)

## Initial Assessment

Before providing recommendations, identify:
1. **Page Type**: Homepage, landing page, pricing, feature, blog, about
2. **Primary Conversion Goal**: Sign up, request demo, purchase, subscribe
3. **Traffic Context**: Where are visitors coming from?

## CRO Analysis Framework

### 1. Value Proposition Clarity (Highest Impact)
- Can visitor understand within 5 seconds?
- Primary benefit clear, specific, differentiated?
- Written in customer's language?

### 2. Headline Effectiveness
- Communicates core value proposition?
- Specific enough to be meaningful?
- Matches traffic source messaging?

### 3. CTA Placement, Copy, and Hierarchy
- One clear primary action?
- Visible without scrolling?
- Button copy communicates value?

### 4. Visual Hierarchy and Scannability
- Scanning gets the main message?
- Important elements visually prominent?
- Enough white space?

### 5. Trust Signals and Social Proof
- Customer logos, testimonials, case studies
- Review scores, security badges
- Placed near CTAs

### 6. Objection Handling
- Price/value concerns
- "Will this work for my situation?"
- Implementation difficulty
- "What if it doesn't work?"

### 7. Friction Points
- Too many form fields
- Unclear next steps
- Confusing navigation
- Mobile experience issues

## Output Format

### Quick Wins (Implement Now)
Easy changes with likely immediate impact.

### High-Impact Changes (Prioritize)
Bigger changes that require more effort.

### Test Ideas
Hypotheses worth A/B testing.

### Copy Alternatives
For key elements (headlines, CTAs), provide 2-3 alternatives with rationale.

---

# SECTION: site-architecture

# Site Architecture

## URL Structure

### Design Principles

1. **Readable by humans** - `/features/analytics` not `/f/a123`
2. **Hyphens, not underscores** - `/blog/seo-guide`
3. **Reflect the hierarchy**
4. **Consistent trailing slash policy**
5. **Lowercase always**
6. **Short but descriptive**

### URL Patterns by Page Type

| Page Type | Pattern | Example |
|-----------|---------|---------|
| Homepage | `/` | `example.com` |
| Feature | `/features/{name}` | `/features/analytics` |
| Pricing | `/pricing` | `/pricing` |
| Blog post | `/blog/{slug}` | `/blog/seo-guide` |
| Blog category | `/blog/category/{slug}` | `/blog/category/seo` |
| Case study | `/customers/{slug}` | `/customers/acme-corp` |
| Documentation | `/docs/{section}/{page}` | `/docs/api/authentication` |
| Legal | `/{page}` | `/privacy`, `/terms` |
| Landing page | `/{slug}` | `/free-trial` |
| Comparison | `/compare/{competitor}` | `/compare/competitor-name` |

## Internal Linking Strategy

### Rules
1. **No orphan pages** - every page must have at least one internal link
2. **Descriptive anchor text** - not "click here"
3. **5-10 internal links per 1000 words**
4. **Link to important pages more often**
5. **Use breadcrumbs**
6. **Related content sections**

### Hub-and-Spoke Model

```
Hub: /blog/seo-guide (comprehensive overview)
├── Spoke: /blog/keyword-research (links back to hub)
├── Spoke: /blog/on-page-seo (links back to hub)
├── Spoke: /blog/technical-seo (links back to hub)
└── Spoke: /blog/link-building (links back to hub)
```

## Navigation Design

### Header Navigation Rules
- **4-7 items max** in primary nav
- **CTA button** goes rightmost
- **Logo** links to homepage (left side)
- **Order by priority**

### Footer Organization
- **Product**: Features, Pricing, Integrations, Changelog
- **Resources**: Blog, Case Studies, Templates, Docs
- **Company**: About, Careers, Contact, Press
- **Legal**: Privacy, Terms, Security

## Breadcrumb Format

```
Home > Features > Analytics
Home > Blog > SEO Category > Post Title
```

Every breadcrumb segment should be clickable except current page.
