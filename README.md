<picture>
  <source media="(prefers-color-scheme: dark)" srcset="assets/title-dark.svg">
  <img src="assets/title-light.svg" width="100%" alt="Senior Full-Stack &amp; AI Product Engineer">
</picture>

I take work from discovery and spec to release, in TypeScript end to end. In my own products I build LLM features with validated output, traces and a person's approval.

I run [GEXP Software](https://gexpsoftware.com), a small remote studio in Costa Rica (UTC-6). 12 years on the web, remote since 2019. I work in English and Spanish.

## What I've shipped

<a href="https://picomar.com"><img src="assets/picomar.webp" width="100%" alt="Picomar home page: an aerial photo of a villa in the forest, the headline A luxury villa, looked after, and a booking search bar"></a>

**[Picomar](https://picomar.com)** is the booking platform of a 46-villa rental company, a client of my studio. Next.js 16, Postgres on Supabase with row-level security, two-way channel-manager sync and card payments. Every change has to pass lint, type checks and a suite of more than 800 test files. [Case study](https://marceloretana.com/work/picomar)

<p><a href="https://alhena.fun"><img src="assets/alhena.webp" width="50%" alt="Alhena: a card with four tasks waiting for a parent to approve"></a><a href="https://goeasy.chat/en"><img src="assets/goeasy-chat.webp" width="50%" alt="GoEasyChat: the headline Your team loses customers when only one person can answer WhatsApp, above a shared inbox"></a></p>

**[Alhena](https://alhena.fun)** is a family task board, my own product. gpt-4o-mini drafts tasks from school email and a parent approves each one. Next.js 16, Drizzle and Neon Postgres. [Case study](https://marceloretana.com/work/alhena)

**[GoEasy.Chat](https://goeasy.chat/en)** is WhatsApp support for teams, my own product. After the Paddle checkout the server creates each customer's workspace and trial, with health checks and self-repair. [Case study](https://marceloretana.com/work/goeasy-chat)

## How I build with AI

**From a school email to a task, in Alhena.** Code checks the model's reply before a parent sees a draft. Every extraction keeps its model name and trace ID, and a failed email is logged and skipped.

<picture>
  <source media="(max-width: 640px) and (prefers-color-scheme: dark)" srcset="assets/email-to-task-dark-mobile.svg">
  <source media="(max-width: 640px)" srcset="assets/email-to-task-light-mobile.svg">
  <source media="(prefers-color-scheme: dark)" srcset="assets/email-to-task-dark.svg">
  <img src="assets/email-to-task-light.svg" width="100%" alt="Example. A school email says: for Friday, bring white poster board; 4th grade, bring the flute. Code checks the model's reply: it matches the schema, Friday becomes November 27, the flute is for another grade and is filtered out, and a link that isn't in the email is dropped. The parent gets a draft to approve or discard.">
</picture>

**Code review by other models, at GEXP.** On GEXP products agents write much of the code, and the model that wrote a change never reviews it. A harness I built sends each diff or plan to two to four others, and one that fails or gets cut off is recorded with the reason.

<picture>
  <source media="(max-width: 640px) and (prefers-color-scheme: dark)" srcset="assets/review-dark-mobile.svg">
  <source media="(max-width: 640px)" srcset="assets/review-light-mobile.svg">
  <source media="(prefers-color-scheme: dark)" srcset="assets/review-dark.svg">
  <img src="assets/review-light.svg" width="100%" alt="Example. The type and risk of a change pick two to four reviewers, never the model that wrote it. Reviewer A answered with two findings, B with none, C was cut off and D hit its provider's limit; both are recorded. A person reads the answers and decides GO or NO-GO. A missing answer never counts as a yes.">
</picture>

I'm also building a terminal agent without a framework: a tool loop, an MCP server, replayable traces, and evals with held-out cases, injection and safety traps, and confidence intervals.

## Where I've worked

- **Universal Music Group**, since 2019: full-stack work on a long-running platform, with React and TypeScript front ends and Node.js services on AWS.
- **TelevisaUnivision**: the monorepo behind 10 high-traffic sites, including Univision.com and TUDN, with Next.js, Relay, GraphQL and React Native.
- **Provectus**: engineer at an AI consultancy and AWS Premier Tier partner, on work for its enterprise clients.
- **IBM**: process tools with React, Node.js and the Carbon Design System.
- **Earlier**: SixFifty, a US legal tech company, and Prodigious, on the Bank of America account.

## Open source and writing

- [chatwoot/chatwoot#13837](https://github.com/chatwoot/chatwoot/issues/13837): how Meta's WhatsApp business-scoped user IDs would break contact matching. Chatwoot's maintainers used it to track the work and closed it as completed in September 2026.
- A bilingual [blog](https://marceloretana.com/blog) and [step-by-step guides](https://marceloretana.com/learn).

## Tools

- **AI:** OpenAI API with structured outputs, Zod, tool calling, MCP, evals
- **Product:** Next.js, React Native, Node.js, GraphQL (Apollo, Relay), Postgres on Supabase, Drizzle, Prisma, Redis
- **Cloud and quality:** AWS (Lambda, S3, CloudFront, DynamoDB, SQS), Vercel, Docker, Turborepo, GitHub Actions, Vitest, Playwright

[Case studies](https://marceloretana.com/work) · [LinkedIn](https://www.linkedin.com/in/marceloretana) · [GEXP Software](https://gexpsoftware.com)
