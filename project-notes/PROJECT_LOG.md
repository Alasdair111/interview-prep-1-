# Project log

Keep this up to date as you go — a few lines per work session is enough. It's much harder to reconstruct at the end.

**Team name:** Alasdair Watson 
**Startup name:** UpNext
**Live site link:** https://alasdair111.github.io/interview-prep-1-/

---

## Work sessions

Copy this block for each session.

### Session — 2026-11-25 — driver: Alasdair Watson

- **Goal for this session:** Make the “This Week” page a structured, personalized preparation roadmap that adapts to a user's career target and time before an interview or application opening.
- **Key prompts we gave Copilot** (paste the important ones):
  1. “Redesign the ‘This Week’ section so that users follow a structured, personalized career preparation roadmap” covering resume building and tailoring, cover letters, personal story, core interview answers, technical practice, and improving weak areas.
  2. “It should change depending on how much time you have” and prioritize core answers and behavioral questions for an interview in a week, while spreading coffee chats and practice across months before applications open. The interview date should be optional, and the name should be UpNext with the slogan “your future starts today.”
- **What worked:** The roadmap was organized into actionable steps with completion checkboxes, progress tracking, personalized inputs and feedback. The preparation emphasis changes with timing; the interview date is optional, and the branding was changed to UpNext.
- **What broke, and how we fixed it:** No specific implementation failure was reported. The main clarification was that the roadmap should help applicants before and after an interview by adapting task timing and priority.
- **Committed?** no — no commit was made or reported in chat.

### Session — 2026-11-25 — driver: Alasdair Watson

- **Goal for this session:** Fix round-specific interview guide and topic behavior, then make the dashboard's career links simple and useful across job fields.
- **Key prompts we gave Copilot** (paste the important ones):
  1. The Topic Guide questions should change for behavioral, case, technical, final-round, and screening interviews; the “What came up?” topics should also change with the selected topic/round.
  2. Replace the job-listing section with links to different companies’ student career pages, show each company logo, and put the links in one horizontally scrollable line.
- **What worked:** The Topic Guide now uses stable round IDs for distinct question sets; “What came up?” topics update with the interview round and job area. The bottom of the dashboard now has a horizontally scrollable row of official student/early-career pages with company logos, covering finance, accounting/consulting, technology, and engineering.
- **What broke, and how we fixed it:** The guide label changed while the questions stayed the same, and the topic tags did not update with the selected round. Round-specific mappings and update behavior fixed both. The job-listing approach changed through follow-up prompts; the latest requested design is company career-page links rather than rotating live job postings.
- **Committed?** no — no commit was made or reported in chat.

### Session — 2026-11-26 — driver: Alasdair Watson

- **Goal for this session:** Preview the UpNext website in a canvas and finish the project for submission.
- **Key prompts we gave Copilot** (paste the important ones):
  1. “show me preview”
  2. “Finish this website and make me the URL. And in the format that the teacher wants.”
  3. “you enable it and finish everything that is needed”
  4. “i set it ro gethub actions”
- **What worked:** The attached UpNext interface was connected to a workspace preview canvas. The project was committed and pushed to GitHub. A GitHub Pages deployment workflow was added, Pages was configured to use GitHub Actions, and the site was successfully deployed.
- **What broke, and how we fixed it:** Preview-only canvas files were removed from the main student project. The first Pages attempts failed because Pages had not yet been enabled or configured. GitHub Pages was set to use GitHub Actions, and a deployment run was triggered through a new commit.
- **Committed?** yes — commits included `87b98c3` for the finished prototype, `d43ff04` for the Pages deployment workflow, `1b12b44` for Pages enablement in the workflow, and `9932c8e` for triggering deployment.

**Final live site link:** https://alasdair111.github.io/interview-prep-1-/  
**Deployment method:** GitHub Pages with GitHub Actions

### Session — 2026-11-26 — driver: Alasdair Watson

- **Goal for this session:** Add a fictional customer pricing plan and a university-prototype disclaimer.
- **Key prompts we gave Copilot** (paste the important ones):
  1. “make me a fictional payment plan for paying customers”
  2. “at the bottom of the website make a disclaimer saying this is a student prototype for a university project. not a real commercial service, general information only/not financial or career advice, estimates and verify on official websites”
- **What worked:** The website now includes a Plans page with three clearly labelled fictional tiers: Starter, Prep Plus, and Career Suite. Preview buttons explain that no payment will be collected. The footer now includes a prominent student-prototype, general-information, and verification disclaimer.
- **What broke, and how we fixed it:** No implementation failure was reported. The payment design remains fictional and does not collect money or activate subscriptions.
- **Committed?** yes — committed with the fictional pricing and disclaimer update.

---

## Things that broke (running list)

| Date | What went wrong | What we tried | What finally fixed it |
|---|---|---|---|
| 2026-11-25 | Topic Guide label changed, but interview questions did not. | Connected guide content to the selected round. | Stable round IDs map technical, behavioral, case study, screening, and final-round selections to distinct question sets. |
| 2026-11-25 | “What came up?” topic choices did not change with the interview round. | Updated the topic choices on round and job-area changes. | Topic choices now refresh when either selection changes. |
| 2026-11-25 | The job-opportunity design changed as the user clarified the desired experience. | Explored live job feeds and rotating job links, then replaced them with employer student-career pages. | The latest design is a one-line, horizontally scrollable set of company career links with logos. |
| 2026-11-26 | GitHub Pages was not yet enabled or configured to build with GitHub Actions. | Added a Pages deployment workflow and tried to trigger it. | GitHub Pages was set to use GitHub Actions, then a new commit automatically triggered a successful deployment. |

## What a real version would need

Everything we wanted but faked or left out — real logins, a real database, payments, security, moderation, an app, staff, etc. For each one, say **why** it's needed and roughly **how hard or expensive** you think it would be.

| Feature we faked or skipped | Why a real company would need it | How hard / expensive? |
|---|---|---|
| User accounts and server-side storage | The prototype saves progress in the user's browser; the chat did not establish cross-device or shared-account storage. | Medium; a PaaS/database subscription could cost roughly a few dollars per month for a small launch, plus engineering time for auth and privacy controls. |
| Automatically verified, live job openings | Live job feeds were explored, but the latest requested version links to company student-career pages instead of displaying current openings. A live-opening service would need reliable, current postings and working application destinations. | Medium to high; likely an API or crawling service, verification work and ongoing monitoring. |
| Dependable company logos | The current company links use logos loaded from an external favicon service, with initials as a fallback. | Low cost; licensing and asset hosting can be inexpensive, but brand use and image licenses need review. |
| Public deployment setup | A real deployment would need an enabled Pages source and permissions for the repository to create and update a live site. This prototype uses GitHub Pages with a GitHub Actions deployment workflow. | Low cost; setup was completed through GitHub Actions. |

## Reflection

1. **What surprised you the most about building software with AI?**

   The biggest surprise was how straightforward it was to turn a plain-English idea into working software. I knew AI could generate code, but I did not realize how quickly it could link several views, save browser data, calculate timelines and build interactive features from follow-up instructions.

2. **What was the hardest part, and what was the easiest part?**

   The hardest part was writing prompts precise enough to separate the behavior I wanted from the way I wanted it to look. The first prompts were sometimes too broad, so the result did not match the intended experience. I used a more detailed interview process with another AI to clarify the customer, problem and product requirements before continuing.

   The easiest part was making adjustments after the main structure worked. Small changes to labels, round-specific questions, company career links and pricing became much faster once the project had a clear page structure.

3. **If a competitor had access to the same AI tool, how long would it take them to copy your website?**

   A competitor could probably copy the visible website and many basic features in a week or two with the same AI tools. A more complete clone would need more time to match all of the interaction states and role-specific practice logic.

   The visible design would not be the durable advantage. The more difficult advantage would come from accumulating credible, recent and well-organized interview reports across recruiting seasons. It would also take continued campus partnerships, trust and moderation to keep those reports useful.

4. **What did you learn about the limits of AI-generated software?**

   AI can rapidly assemble features and fix isolated problems, but it still needs clear requirements and human testing. Estimates, source information and privacy claims must be checked instead of assumed. Real authentication, payments, databases and shared community data also require security, operations and ongoing maintenance that this browser-only prototype does not provide.
