# Day 1 Lab

## Exercise 1

### Prompt v1

```text
I'm a podcaster and I need to create an e-mail asking for mailing list for another company
```

### Response v1

```text
You can use this email template to ask another company or partner to share your

podcast's mailing list sign-up with their audience.

Email Template

Subject: Quick collaboration idea / Share [Your Podcast Name] with your audience?

Hi [Contact Namel,

I hope you are having a great week.

I love the work you do at [Company Namel, especially your recent [mention a specific

article, product, or project].

I host [Your Podcast Name], a show where we talk about [briefly describe your podcast

topic in 5 words]. Our listeners are deeply interested in [shared niche/topic], which makes

them a great fit for your brand.

I am writing to see if you would be open to a simple cross-promotion. We are growing our

newsletter and would love to share a sign-up link with your community. In exchange, I

would love to feature [Company Namel or share your latest updates with our podcast

listeners and newsletter subscribers.

Here is the link where people can join our list: [Insert Link to Your Signup Page]

Let me know if you are open to chatting about this. I am happy to keep it simple and low-

effort for your team!

Best regards,

[Your Namel

[Your Podcast Namel

[Link to your website]

If you tell me what your podcast is about and what your partner company does, I can

customize this template to fit your exact situation.
```

### Assumption audit

| Assumption | What the response assumed and where I can see it | Was it acceptable? |
| --- | --- | --- |
| Purpose of the request | My phrase “asking for mailing list” was interpreted as asking the company to promote my own signup link: “share your podcast's mailing list sign-up with their audience.” | No. I had not clarified whether I wanted to join the company's mailing list, request a list, or promote my own. The response chose one meaning without checking. |
| Relationship with the recipient | “I love the work you do” and the reference to a recent project assume I know the company's work and can give a sincere compliment. | No. I did not provide that background, so I would need to verify or replace this part. |
| Audience overlap | “Our listeners are deeply interested in [shared niche/topic]” assumes my listeners and the company's audience share an interest. | No. I gave no information about either audience to support that claim. |
| Existing newsletter and growth goal | “We are growing our newsletter” assumes I already have a newsletter and want more subscribers. | No. I only said I was a podcaster; I did not mention a newsletter or a growth goal. |
| Offer in return | “In exchange, I would love to feature [Company Namel” assumes I am willing to offer promotion on my podcast or newsletter. | No. I did not authorize an exchange or say what I could offer. |
| Available signup page | “Here is the link where people can join our list: [Insert Link to Your Signup Page]” assumes I have a working subscription page. | No. That is a necessary detail for the proposed email, but I had not supplied it or confirmed that it exists. |
| Tone | “I hope you are having a great week” and “happy to keep it simple and low-effort” establish a friendly business tone. | Yes. It is a reasonable tone for an introductory email, although I did not specify one. |
| Format | “Email Template,” a subject line, a greeting, and a signature turn the answer into a reusable template with placeholders. | Yes. That gives me a usable email structure despite the missing names and details. |
| Length and scope | The response includes several email paragraphs plus an introduction and a final offer to customize the template. | Partly. The draft is usable, but I only asked for an email. I would remove the surrounding commentary before using it. |
| Effort required from the company | “low-effort for your team” assumes the proposed collaboration will be easy for the recipient. | No. I do not know the company's process or workload, so I cannot promise that. |

## Exercise 2

### My goal for the rewrite

For this rewrite, I use a specific version of the task: asking to join a company's press mailing list so I can receive news for my podcast. This removes the ambiguity in “asking for mailing list” without inventing a company, a contact, or an audience size.

### Prompt v2

```text
Instruction: Write an email asking a company to add me to its press mailing list so I can receive news for my podcast.

Context: The recipient is the company's press or communications team. Use professional, friendly English. I am requesting updates from the company, not access to its subscribers or promotion of my own newsletter. Do not invent audience numbers, previous contact, familiarity with the company, or an offer of coverage or cross-promotion. Use placeholders for missing names and contact details.

Input:
"""
I am a podcaster. I want to receive company news, press releases, and product announcements that I can consider for future episodes. My name, podcast name, company name, and email address have not been provided.
"""

Output format: Return only the email in plain text. Include one subject line, a greeting, two short body paragraphs, and a sign-off. Keep the entire email under 120 words. Use [Your Name], [Podcast Name], [Company Name], and [Your Email] as placeholders.
```

### Response v2

```text
Subject: Press Mailing List Request

Hello [Company Name] Press Team,

I’m a podcaster with [Podcast Name], and I’d like to receive your company news, press releases, and product announcements for consideration in future episodes. Could you please add me to your press mailing list?

My contact details are below:
[Your Name]
[Podcast Name]
[Your Email]

Thank you for your time and consideration.

Best regards,
[Your Name]
```

### Side-by-side comparison

| Point | v1 | v2 |
| --- | --- | --- |
| Main request | “share a sign-up link with your community” asks the company to promote my newsletter. | “Could you please add me to your press mailing list?” asks to receive the company's updates. |
| Recipient | “Hi [Contact Namel” leaves the recipient's role unspecified. | “Hello [Company Name] Press Team” identifies the relevant team. |
| Unsupported claims | “I love the work you do” and “Our listeners are deeply interested” add background I never supplied. | The email sticks to being a podcaster and wanting news to consider for future episodes. |
| Commitments | “In exchange, I would love to feature” offers promotion. | “for consideration in future episodes” leaves editorial decisions open. |
| Output boundaries | An introduction and an offer to customize surround the email. | The response contains only the email. |
| Remaining editing | The purpose, invented claims, and placeholders all need attention. | The placeholders still need filling, and the body needs tightening to meet the two-paragraph requirement. |

### Which block made the biggest difference?

The **Instruction** block made the biggest difference because it changed the actual request. The first output asked for newsletter promotion; the second explicitly asked to be added to the company's press mailing list, which is the task I chose for the rewrite. The Context block reinforced that boundary and excluded invented claims and offers, so I cannot attribute every improvement to Instruction alone.

### Which assumptions are resolved, and which remain open?

The revised prompt resolves the purpose, recipient's role, tone, and intended output length and structure. It also removes the need to assume an existing newsletter, a signup page, shared audiences, familiarity with the company, or a cross-promotion offer. The output no longer makes the “low-effort” promise from v1.

The actual company, contact, podcast name, and email address remain open and are represented by placeholders. I also still need to check whether the company has a press mailing list and whether it accepts requests from podcasters. The format instruction is explicit, but compliance is not perfect: the response has a request paragraph, a contact-details block, and a separate thank-you paragraph instead of exactly two short body paragraphs.

### Format ablation: full prompt

I removed only the Output format section and ran the remaining prompt in a fresh conversation.

```text
Instruction: Write an email asking a company to add me to its press mailing list so I can receive news for my podcast.

Context: The recipient is the company's press or communications team. Use professional, friendly English. I am requesting updates from the company, not access to its subscribers or promotion of my own newsletter. Do not invent audience numbers, previous contact, familiarity with the company, or an offer of coverage or cross-promotion. Use placeholders for missing names and contact details.

Input:
"""
I am a podcaster. I want to receive company news, press releases, and product announcements that I can consider for future episodes. My name, podcast name, company name, and email address have not been provided.
"""
```

### Format ablation: full response

```text
Here’s a professional, friendly version you can send:

Request to Join Press Mailing List

Dear [Press/Communications Team],

My name is [Your Name], and I host [Podcast Name]. I’m writing to ask if you could add me to your press mailing list.

I’d appreciate receiving your company news, press releases, and product announcements so I can stay informed and consider relevant updates for future podcast episodes.

Please let me know if you need any additional information from me. My email address is [Your Email Address].

Thank you for your time, and I appreciate your consideration.

Best regards,
[Your Name]
[Podcast Name]
[Your Email Address]

I can also make this shorter and more casual if you’d prefer.
```

### Manual cleanup and what the ablation shows

The ablated version keeps the correct purpose, which suggests the first three blocks are enough to communicate the request. It adds “Here’s a professional, friendly version you can send” before the email and an offer to make it shorter afterward; it also uses four body paragraphs and a different email placeholder.

Before using it, I would remove the two surrounding comments, put “Request to Join Press Mailing List” in the subject field, replace the placeholders, and combine the body into two paragraphs. This is a small editing pass rather than a complete rewrite, but it is more cleanup than v2 needs. This single comparison suggests that Output format helped control the presentation; it does not prove that every future run would behave the same way.

## Exercise 3

### Part A — Token budget

#### Longer text

I used the supplied lab documentation for Exercises 1 and 2 as my longer text. It is reproduced below so the character count can be checked against the exact material.

```text
Exercise 1 — The assumption audit (15 min)

    Write down the first prompt that comes to mind for your chosen task. Do not polish it. Label it v1.
    Run it. Paste the full output.
    Now list every assumption your prompt forced the model to guess. Aim for at least five. Use these prompts to find them:
        Who is the audience?
        How long should the answer be?
        What tone or register?
        What format — prose, bullets, table, JSON?
        What must the answer include? What must it avoid?
        What information does the model not have that it would need?
    For each assumption, write one line: what the model guessed, and whether that guess was acceptable.

What good looks like: at least five named assumptions, each tied to something concrete you can see in the output. "It was too generic" is not an assumption; "I never said the audience was non-technical, so it used jargon like idempotent" is.

Keep this list. You will use the same diagnostic habit for the rest of the course.
Exercise 2 — The four-block rewrite (20 min)

    Rewrite your v1 prompt using four explicitly labelled sections. Label it v2:

    Instruction: <what to do — concrete verb, measurable target>

    Context: <audience, purpose, constraints, what to avoid>

    Input:
    """
    <the material to act on>
    """

    Output format: <exact shape: length, structure, fields or columns>

    If one of the four sections is genuinely empty, write (none needed because ...) and justify it in one sentence. Do not leave a section blank without a reason — the most common cause of a blank section is that you forgot, not that it was unnecessary.

    Run v2. Paste the full output.

    Compare v1 and v2 side by side and answer in writing:
        Which single block made the biggest difference? How do you know?
        Which assumptions from Exercise 1 are now resolved, and which are still open?

    Run one ablation: take v2, delete only the Output format section, and run it again. Paste that output too. Note how much manual cleanup the unformatted version would need before you could use it.

What good looks like: v2 resolves at least three assumptions from your Exercise 1 list, the input is wrapped in delimiters, and your comparison names a specific block rather than saying the prompt is "better."
```

#### Full-context prompt for the estimate

This is my baseline for comparison before sending the shorter version.

```text
Using only the documentation below, explain how to run the format ablation and what to record. Answer in two sentences.

Documentation:
"""
Exercise 1 — The assumption audit (15 min)

    Write down the first prompt that comes to mind for your chosen task. Do not polish it. Label it v1.
    Run it. Paste the full output.
    Now list every assumption your prompt forced the model to guess. Aim for at least five. Use these prompts to find them:
        Who is the audience?
        How long should the answer be?
        What tone or register?
        What format — prose, bullets, table, JSON?
        What must the answer include? What must it avoid?
        What information does the model not have that it would need?
    For each assumption, write one line: what the model guessed, and whether that guess was acceptable.

What good looks like: at least five named assumptions, each tied to something concrete you can see in the output. "It was too generic" is not an assumption; "I never said the audience was non-technical, so it used jargon like idempotent" is.

Keep this list. You will use the same diagnostic habit for the rest of the course.
Exercise 2 — The four-block rewrite (20 min)

    Rewrite your v1 prompt using four explicitly labelled sections. Label it v2:

    Instruction: <what to do — concrete verb, measurable target>

    Context: <audience, purpose, constraints, what to avoid>

    Input:
    """
    <the material to act on>
    """

    Output format: <exact shape: length, structure, fields or columns>

    If one of the four sections is genuinely empty, write (none needed because ...) and justify it in one sentence. Do not leave a section blank without a reason — the most common cause of a blank section is that you forgot, not that it was unnecessary.

    Run v2. Paste the full output.

    Compare v1 and v2 side by side and answer in writing:
        Which single block made the biggest difference? How do you know?
        Which assumptions from Exercise 1 are now resolved, and which are still open?

    Run one ablation: take v2, delete only the Output format section, and run it again. Paste that output too. Note how much manual cleanup the unformatted version would need before you could use it.

What good looks like: v2 resolves at least three assumptions from your Exercise 1 list, the input is wrapped in delimiters, and your comparison names a specific block rather than saying the prompt is "better."
"""
```

#### Trimmed prompt

The question only needs the paragraph about the format ablation. I kept that paragraph and removed the assumption-audit instructions, the four-block template, and the other comparison requirements.

```text
Using only the documentation below, explain how to run the format ablation and what to record. Answer in two sentences.

Documentation:
"""
Run one ablation: take v2, delete only the Output format section, and run it again. Paste that output too. Note how much manual cleanup the unformatted version would need before you could use it.
"""
```

#### Counts and reduction

I counted characters including spaces and line breaks, excluding the Markdown code fences and any trailing newline. I divided each count by four; these are estimates, not exact tokenizer counts.

| Material | Characters | Estimated tokens (characters ÷ 4) |
| --- | ---: | ---: |
| Longer source text | 2,319 | 579.75 |
| Relevant excerpt only | 195 | 48.75 |
| Full-context prompt, including question and delimiters | 2,463 | 615.75 |
| Trimmed prompt, including question and delimiters | 339 | 84.75 |

Source-text reduction: `(2319 − 195) ÷ 2319 × 100 = 91.59%`.

Total-prompt reduction: `(2463 − 339) ÷ 2463 × 100 = 86.24%`.

The total-prompt figure is the more useful estimate of what I send because it includes the question and delimiters. The shorter version still contains every instruction needed to answer this specific question: delete only Output format, run the prompt again, paste the output, and note the manual cleanup required. I did not perform the optional exact-token comparison.

#### Full response to the trimmed prompt

After estimating the counts, I ran the trimmed prompt:

```text
Take v2, delete only the Output format section, and run it again, then paste that output too. Record how much manual cleanup the unformatted version would need before it could be used.
```

The response includes both the procedure and the observation to record, using only the relevant paragraph.

### Part B — Variability

Each repetition used a fresh conversation with the same prompt text. The creative prompt left the choice of names and presentation open; the specified prompt fixed both the answer and its format.

#### Open-ended prompt — Run 1

**Prompt:**

```text
Suggest a name for a podcast about technology.
```

**Full output:**

```text
Here are some catchy tech podcast name ideas:

Future Stack
Beyond the Code
Tech Unplugged
The Digital Edge
Next Byte
Signal & Noise
The Tech Current
Circuit Breakers
Tomorrow, Today
Code & Culture
The Innovation Loop
Byte Sized
Future Frequency
The Tech Frontier
Silicon Stories

My favorite: Future Stack — short, modern, and broad enough to cover AI, startups, gadgets, software, and emerging technology.
```

#### Open-ended prompt — Run 2

**Prompt:**

```text
Suggest a name for a podcast about technology.
```

**Full output:**

```text
Here are some catchy options:

Tech Unplugged
The Future Stack
Beyond the Screen
Circuit Breakers
Next Byte
Tech in Plain English
The Digital Frontier
Future, Now
Code & Coffee
The Tech Signal
Byte Sized
Tomorrow’s Tech
Silicon & Beyond
The Innovation Loop
Ctrl + Future

My favorite: The Tech Signal — short, memorable, and broad enough to cover AI, gadgets, startups, cybersecurity, and emerging tech.
```

#### Open-ended prompt — Run 3

**Prompt:**

```text
Suggest a name for a podcast about technology.
```

**Full output:**

```text
Here are some catchy tech podcast name ideas:

Future Wired
Tech Unpacked
The Digital Edge
Beyond the Code
Next Gen Now
Circuit Breakers
The Tech Signal
Byte by Byte
Future Stack
Silicon & Sense
The Innovation Loop
Code & Culture
Tomorrow's Tech
The Upgrade
Tech After Hours

My top 3: The Tech Signal, Beyond the Code, and The Upgrade.
```

#### Tightly specified prompt — Run 1

**Prompt:**

```text
Return only the ISO 8601 date for the first day of March 2026. No other text.
```

**Full output:**

```text
2026-03-01
```

#### Tightly specified prompt — Run 2

**Prompt:**

```text
Return only the ISO 8601 date for the first day of March 2026. No other text.
```

**Full output:**

```text
2026-03-01
```

#### Tightly specified prompt — Run 3

**Prompt:**

```text
Return only the ISO 8601 date for the first day of March 2026. No other text.
```

**Full output:**

```text
2026-03-01
```

#### Which prompt was more consistent, and why?

The tightly specified prompt returned exactly `2026-03-01` in all three runs. It names a single date, specifies ISO 8601, and excludes extra text, leaving very little room for variation.

The creative prompt produced three different lists of 15 names. Run 1 favored “Future Stack,” Run 2 favored “The Tech Signal,” and Run 3 selected three favorites instead of one; even though some names repeated, the full outputs differed. I had not fixed the number of suggestions, naming style, audience, or explanation format, so the prompt allowed many acceptable responses.

These results connect consistency to how tightly the task and output are specified, but the tasks also differ: a date has a single factual answer, while naming is subjective. Three runs illustrate the difference here; they do not establish that a constrained prompt can never vary.

## Reflection

### Which of my tasks need consistency, and which benefit from variety?

Emails requesting press-list access need consistency because the purpose, tone, and factual claims should stay stable between drafts. Brainstorming podcast names or episode titles benefits from variety because different angles give me more options to compare before I choose one.

### What habit will I apply before writing my next prompt?

Before writing my next prompt, I will list the decisions I do not want the model to guess, starting with my actual goal and the intended recipient. I will then put those decisions into the four blocks and include only the source material needed for the task.
