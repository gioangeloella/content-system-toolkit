# AI writing tool: designer feedback survey

This is a question repo for gathering structured feedback from designers using an AI writing tool.

## Purpose

Informal feedback from Slack channels and office hours gives you signals, but it's anecdotal and unevenly distributed. A structured survey supplements those signals with additional data across the team. Run it 6 to 8 weeks after launch. This gives designers enough time to form real opinions.

## What the survey data can inform

- Adjustments to the tool's instructions, training data, or prompt design
- Reduction of content-related escalations through async channels and office hours
- Actionable insights for the next phase of integrated tooling
- A case for investment or for pivoting

## Survey setup

**Platform:** Google Forms, Typeform, SurveyMonkey, or equivalent

**Time to complete:** Less than 5 minutes

**Intro paragraph (customize for your specific needs):**
"Thanks for helping us evolve [tool name]. This short survey will take less than 5 minutes and will directly shape our future writing tools and integrations."

## Questions

### Question 1: Usage frequency (gatekeeper)

**Type:** Multiple choice

On average, how often have you used [tool name] over the past 2 months?

- Multiple times a day
- Once a day
- A few times a week
- I haven't used it yet → skip to Question 9
- Prefer not to say → end survey

### Question 2: Workflow integration

**Type:** Multiple choice (scale)

Overall, how does [tool name] fit into your current design workflow?

- 1 = Disruptive (too much tool-switching)
- 2 = Somewhat disruptive (noticeable friction in my daily workflow)
- 3 = Neutral (takes some manual effort, but manageable)
- 4 = Mostly smooth (integrates well with minor friction)
- 5 = Seamless (fits perfectly into my workflow)

### Question 3: Time saved

**Type:** Multiple choice

On average, how much time do you think [tool name] saves you when drafting copy for a screen?

- It doesn't save me time or adds time
- Less than 30 minutes
- 30 to 60 minutes
- More than an hour

### Question 4: Confidence level

**Type:** Multiple choice (scale)

What's the level of confidence you feel when using [tool name]'s copy recommendations?

- 1 = Not confident at all (I rarely trust the suggestions and usually rewrite them)
- 2 = Slightly confident (I feel hesitant and frequently look for alternative options)
- 3 = Moderately confident (I trust it for simple UI elements, but question it for complex copy)
- 4 = Very confident (I trust the recommendations for almost all my UI designs)
- 5 = Completely confident (I fully trust the recommendations to be accurate and it's ready to launch)

### Question 5: Guideline inaccuracies

**Type:** Checkboxes (select all that apply)

Have you noticed [tool name] suggesting any incorrect standards or guidelines?

- CTA labels that are too long (e.g., more than 3 words)
- Punctuation errors (e.g., question marks in modal headings)
- Outdated UI terminology
- I haven't noticed any incorrect patterns
- Other: [free-form text]

Customize these options based on the most common content standards in your guidelines.

### Question 6: Most-wanted features

**Type:** Checkboxes (select up to 2)

Which of the following features would bring the most value to your day-to-day work?

- Direct integration inside your design tool (no external tool-switching)
- Ability to generate an IA blueprint for new screens to guide the design layout
- Interactive prompts to narrow down user context before generating copy
- Access to relevant user research insights or testing data to back up copy recommendations
- Built-in accessibility guidelines (e.g., helper text, alt text, screen readers)

Customize these options based on your roadmap and what's realistically buildable.

### Question 7: What designers like most

**Type:** Open text (paragraph)

What do you like most about [tool name] so far?

### Question 8: Biggest frustration

**Type:** Open text (paragraph)

What's your biggest frustration with [tool name]?

### Question 9: Final comments

**Type:** Open text (paragraph, optional)

Any final comments you'd like to share?

→ End survey for active users

### Question 10: Non-user follow-up

**Type:** Open text (paragraph)

Shown only to respondents who selected "I haven't used it yet" in Question 1.

What has kept you from using [tool name] so far, and what features or integrations would make a UX writing tool useful for your daily work?

→ End survey

## Skip logic summary

| Response | Routing |
|---|---|
| Question 1: "I haven't used it yet" | Skip to Question 9, then show Question 10 |
| Question 1: "Prefer not to say" | End survey |
| All other Question 1 responses | Continue through Questions 2 to 9 |

## Tips and tricks

- **Keep it short.** Five minutes or less. Making it longer will affect the response rate.
- **Run it at the right time.** Too early (under 4 weeks) and designers haven't formed opinions. Too late (over 12 weeks) and you've missed the window to act on early feedback.
- **Pair with usage data.** Survey responses tell you why. Usage data tells you what. Together they give you a fuller picture.
- **Share results back.** Designers who took the time to respond should see what you learned and what you're doing about it. This builds trust for the next survey.

---

*Template from the [Content System Toolkit](https://github.com/gioangeloella/content-system-toolkit). Based on a framework developed by [Giovanni Ella](https://wordli.com).*
