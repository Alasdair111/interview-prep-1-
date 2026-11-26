# Project log

Keep this up to date as you go — a few lines per work session is enough. It's much harder to reconstruct at the end.

**Team name:** Alasdair Watson 
**Startup name:** UpNext
**Live site link:** https://alasdair111.github.io/interview-prep-1-/

---

## Work sessions

Copy this block for each session.

### Session — 2026-11-25 — driver: not provided in chat

- **Goal for this session:** Make the “This Week” page a structured, personalized preparation roadmap that adapts to a user's career target and time before an interview or application opening.
- **Key prompts we gave Copilot** (paste the important ones):
  1. “Redesign the ‘This Week’ section so that users follow a structured, personalized career preparation roadmap” covering resume building and tailoring, cover letters, personal story, core interview answers, technical practice, and improving weak areas.
  2. “It should change depending on how much time you have” and prioritize core answers and behavioral questions for an interview in a week, while spreading coffee chats and practice across months before applications open. The interview date should be optional, and the name should be UpNext with the slogan “your future starts today.”
- **What worked:** The roadmap was organized into actionable steps with completion checkboxes, progress tracking, personalized inputs and feedback. The preparation emphasis changes with timing; the interview date is optional, and the branding was changed to UpNext.
- **What broke, and how we fixed it:** No specific failure was reported in this session. Follow-up prompts clarified the timing rules and that the app should also help people who have not yet landed an interview.
- **Committed?** no — no commit was made or reported in chat.

### Session — 2026-11-25 — driver: not provided in chat

- **Goal for this session:** Fix round-specific interview guide and topic behavior, then make the dashboard's career links simple and useful across job fields.
- **Key prompts we gave Copilot** (paste the important ones):
  1. The Topic Guide questions should change for behavioral, case, technical, final-round, and screening interviews; the “What came up?” topics should also change with the selected topic/round.
  2. Replace the job-listing section with links to different companies’ student career pages, show each company logo, and put the links in one horizontally scrollable line.
- **What worked:** The Topic Guide now uses stable round IDs for distinct question sets; “What came up?” topics update with the interview round and job area. The bottom of the dashboard now has a horizontally scrollable row of official student/early-career pages with company logos, covering finance, accounting/consulting, technology, and engineering.
- **What broke, and how we fixed it:** The guide label changed while the questions stayed the same, and the topic tags did not update with the selected round. Round-specific mappings and update behavior fixed both. The job-listing approach changed through follow-up prompts; the latest requested design is company career-page links rather than rotating live job postings.
- **Committed?** no — no commit was made or reported in chat.

### Session — 2026-11-26 — driver: not provided in chat

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

### Session — 2026-11-26 — driver: not provided in chat

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
| User accounts and server-side storage | The prototype saves progress in the user's browser; the chat did not establish cross-device or shared-account storage. | Not estimated in chat. |
| Automatically verified, live job openings | Live job feeds were explored, but the latest requested version links to company student-career pages instead of displaying current openings. A live-opening service would need reliable, current postings and working application destinations. | Not estimated in chat. |
| Dependable company logos | The current company links use logos loaded from an external favicon service, with initials as a fallback. | Not estimated in chat. |
| Public deployment setup | A real deployment would need an enabled Pages source and permissions for the repository to create and update a live site. This prototype uses GitHub Pages with a GitHub Actions deployment workflow. | Low cost; setup was completed through GitHub Actions. |

## Reflection (fill in at the end)

1. **What surprised you the most about building software with AI?**

   The biggest thing that surprised me about building software with AI was how straightforward it was. I knew AI could build websites, but I didn't realize it would be as simple as telling it what I wanted and having it do the work for me. I was pretty mind-blown by everything it was able to do, especially how easily I was able to get it to link to other companies' websites and build interactive features without having to write the code myself.

2. **What was the hardest part, and what was the easiest part?**

   I would say the hardest part was creating the right prompt to get the website exactly how I wanted it. When I first started building the website, I found that my prompts weren't specific enough, and the results weren't exactly what I was looking for.

   To fix this, I used ChatGPT to interview me. I had it ask me around 50 questions, which I answered to help build a more detailed and accurate original prompt. I think one of the biggest parts of building software with AI is having a good prompt.

   The easiest part was making fixes and adjustments once the original prompt was completed. It was extremely easy to make changes to the website. All I had to do was type what I wanted to change, and the AI would make the adjustments right away.

3. **If a competitor had access to the same AI tool, how long would it take them to copy your website?**

   I think it would take a competitor over a week to replicate my website exactly, mainly because of all the small details and features I added throughout the development process. However, because anyone can access the same AI tools, I don't think it would be extremely difficult for someone to build a similar website.

   That is why I designed certain features to help build a competitive moat. For example, users can return to the website after their interviews and input the topics and common questions they were asked. Over time, as more people use the website, this data could help future applicants prepare for similar interviews.

   Even if a competitor replicated my entire website, they would not automatically have access to the data I could collect from
