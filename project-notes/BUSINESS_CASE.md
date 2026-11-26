## 1. The idea
**Who is my customer?** My customer is a student or job seeker preparing for a competitive hiring process in investment banking, consulting, accounting, engineering, computer science or software engineering. The person I had in mind when I built Up Next was a second-year student who knows what internship they want but has never gone through recruiting for it before.

**What problem do they have, and how do they solve it today?** A lot of students don’t realize how early recruiting starts. Some finance applications open over a year before the position begins. A student could be planning to work next summer and miss the application before they even think to look. Getting an interview brings another challenge. Some hiring processes involve as many as eight interviews, and the technical and behavioural rounds take different kinds of preparation.

Right now, a student might check a company’s careers page for dates, ask an upper-year student what came up and search online for practice questions. They still have to put those pieces together and decide what to work on this week. That’s hard to do the first time, especially if they don’t know anyone who has interviewed for the role.

**What does Up Next do?** It builds a week-by-week plan around the role a student wants and the time they have. They can see when applications might open, practise for a specific interview round and do a mock interview. They can also tell the site which topics they struggle with and come back to those questions. The dashboard links to early-career pages so students can check whether an application has actually opened.

**How would it make money?** I would charge **$20 a month** for personalized preparation and mock interviews. The prices shown on the prototype are examples. A student might subscribe for the three months leading up to interviews and cancel once they accept an offer. I’d need to bring in a new class of applicants each year. I might eventually add mentorship with upper-year students. For now, the subscription is how I would make money.

## 2. Where IT creates value
**Which parts of the value chain does Up Next change?** The first is planning. On the prototype, entering “Investment Banking Analyst” for a May 2028 start gives an estimated application opening of February 2027. That’s 15 months before the internship. Seeing those dates together explains why a student might want to start networking this semester. Once they find the actual opening date, they can enter it and reschedule the work they have left.

The second is how students practise. Someone preparing for a banking interview might feel comfortable explaining financial statements but get stuck walking through a discounted cash flow valuation. They can flag that topic and take a three-question diagnostic. The site uses their role, interview round and missed answers to guide the next practice session. That’s **differentiation** because two students applying for the same job can spend their time on different questions.

Technology also changes how I could reach students. A finance club or co-op office could share one link with a whole class. Each student could build a different plan without someone at the club writing each one by hand. That gives me a **distribution channel** and keeps the cost of serving one more student low.

## 3. Network effects
**Is it a one-sided or two-sided market?** Up Next is **one-sided**. Students and job seekers are the people using it. The same student can read about interview topics before their interview and contribute a report afterward. Employers don’t need to join or post jobs for that exchange to work.

**Where does the extra value come from?** One person can use the planner and mock interviews on their own. The network effect comes from applicants sharing what happened afterward. If several students who went through a banking technical round mention valuation multiples, next year’s applicants have a reason to give that topic more practice time. What matters is how many people contribute recent reports for that role. Ten students visiting the homepage would leave the next applicant with the same information they had before.

**How would I solve the empty-network problem?** I’d start with investment banking internships at my university. The first students could use the planner and question bank immediately. To get the first reports, I’d ask upper-year students through a campus finance club to tick the topics they remember from their most recent interview. I’d keep reporting free, including for students who already have an offer. Ten reports about the same type of role would give the next applicant more to work with than one report in each of ten fields.

**Where does the prototype show this?** Under **What came up?**, an applicant can enter “Investment Banking Analyst,” choose “Technical” and select “Discounted cash flow.” Submitting one fictional report took that topic from zero mentions to one. The count stays in that browser today. A shared database would let another student see the updated count from their own laptop.

## 4. Can it be copied?
**What is valuable, rare, hard to imitate and well-organized?** I think anyone in my class could rebuild a similar-looking website in about a week. The weekly plan is valuable because it helps a student decide how to spend the few evenings they have before an interview. A competitor could offer a checklist and a question bank fairly quickly. What I think could become rare is a history of what applicants actually experienced in a particular role and round across several recruiting seasons.

An upper-year student might remember getting a valuation question in their final round. That’s useful advice. It would be more useful to know whether applicants also saw valuation in the first technical round and whether it came up again the following year. Building that history takes students who are willing to come back after their interviews, including those who didn’t get the job.

To make the reports useful, I’d organize them by role, interview round and recruiting season. I’d count “DCF” and “discounted cash flow” under one topic and check for duplicate reports. I’d also show how many people contributed. If a topic came up twice, a student should be able to tell whether that means two out of three applicants or two out of thirty.

**What would a competitor with a bigger budget need, and how long would it take?** A bigger company could hire developers, write more questions and promote its website faster than I could. A week is my estimate for copying the visible features. A competitor collecting fresh reports from scratch would need two recruiting cycles before it could compare one year with another. It could catch up sooner if it already had campus partnerships or could get reliable reports from past applicants. That’s why I’d put time into relationships with student clubs early on.

**Which advantages get stronger over time?** The biggest one is the data, as long as students keep contributing and the reports stay current. There is also a **switching cost** for each student. By week six, they might have finished half their checklist, saved practice notes and figured out which questions still give them trouble. Starting over somewhere else would mean rebuilding that history. That gives them a reason to stay through their interview process.

## 5. Cloud and operations
**What would it take to run Up Next for real?** GitHub Pages hosts the website today. Progress and interview reports are saved in the browser, so a student who switches from a laptop to a phone starts with a separate history.

**Which cloud services would I buy, and what are the risks?** I’d use a managed platform (**PaaS**) to run the app, with sign-in and a database for saved plans and shared topic counts. I’d buy subscription billing software (**SaaS**) to handle payments and cancellations. Renting virtual servers directly (**IaaS**) would leave me responsible for updates and monitoring, which would be more work than I’d need at launch.

I’d still need to control who can see private notes, review flagged reports and answer billing questions. If the host went down the night before an interview, students could lose access to their plans when they needed them most. I’d let them download a copy. I’d also keep backups, test that I could restore them and set spending alerts in case hosting costs rose.

## 6. Risks and ethics
**What could go wrong, and what would I do about it?** One risk is that a student trusts an estimated application date and misses the opening. I’d clearly label estimates, direct students to the employer’s official posting and let them replace an estimate with a confirmed date. Helping students avoid missed opportunities is one of the main reasons I built Up Next.

Privacy matters even with anonymous reports. At a small firm, naming the interviewer, office or exact interview date could give away who applied. I’d ask for broad topics, keep practice notes private and review custom entries for identifying details. I’d only show group results once several different students had contributed.

Reports from one club could also give a misleading picture of what everyone gets asked. I’d show the recruiting season and number of reports behind each topic and invite students from other schools as the service grows. Students could then judge how much weight to give a topic when deciding what to practise.

Price also affects who can use the service. A student with few industry connections might benefit the most and still find $20 a month expensive. I’d keep the basic recruiting timeline and topic reporting free, with the subscription covering personalized preparation.
