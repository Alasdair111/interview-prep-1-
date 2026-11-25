# Project log

Keep this up to date as you go — a few lines per work session is enough. It's much harder to reconstruct at the end.

**Team name:** Not provided in chat
**Startup name:** UpNext
**Live site link:** Preview at http://localhost:8000 (local preview; no public site link provided)

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

---

## Things that broke (running list)

| Date | What went wrong | What we tried | What finally fixed it |
|---|---|---|---|
| 2026-11-25 | Topic Guide label changed, but interview questions did not. | Connected guide content to the selected round. | Stable round IDs map technical, behavioral, case study, screening, and final-round selections to distinct question sets. |
| 2026-11-25 | “What came up?” topic choices did not change with the interview round. | Updated the topic choices on round and job-area changes. | Topic choices now refresh when either selection changes. |
| 2026-11-25 | The job-opportunity design changed as the user clarified the desired experience. | Explored live job feeds and rotating job links, then replaced them with employer student-career pages. | The latest design is a one-line, horizontally scrollable set of company career links with logos. |

## What a real version would need

Everything we wanted but faked or left out — real logins, a real database, payments, security, moderation, an app, staff, etc. For each one, say **why** it's needed and roughly **how hard or expensive** you think it would be.

| Feature we faked or skipped | Why a real company would need it | How hard / expensive? |
|---|---|---|
| User accounts and server-side storage | The prototype saves progress in the user's browser; the chat did not establish cross-device or shared-account storage. | Not estimated in chat. |
| Automatically verified, live job openings | Live job feeds were explored, but the latest requested version links to company student-career pages instead of displaying current openings. A live-opening service would need reliable, current postings and working application destinations. | Not estimated in chat. |
| Dependable company logos | The current company links use logos loaded from an external favicon service, with initials as a fallback. | Not estimated in chat. |

## Reflection (fill in at the end)

1. What surprised you most about building software with AI? Not answered in chat yet.
2. Which parts were easy, and which were hard? Why do you think that is? Not answered in chat yet.
3. If a competitor had the same AI tool, how long would it take them to copy your site? Not answered in chat yet.
