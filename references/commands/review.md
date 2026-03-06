# review — Progress and Timeline Review Workflow

Requires `kickoff` to have been run. If no `counseling_state.md` exists, redirect: "I need to know a bit about you before I can review your progress. Let's start with `kickoff` to set up your profile." Load `references/counselor-styles.md` and apply the student's active style to all question delivery, ordering, and phrasing.

### Step 1: Load Full State

Read all sections of `counseling_state.md`:
- Profile (grade, school, target graduation year, current semester)
- Interest Discovery
- Academic Track
- Activities & Spike
- Testing
- College List
- Essays
- Financial
- Summer Experiences
- Recommendations
- Timeline Status (previous check results)
- Session Log (recent activity)
- Active Counseling Strategy
- Coaching Notes

Load milestone timeline from `references/timeline-engine.md`. Determine current semester from date:
- Fall semester: August 15 - December 31
- Spring semester: January 1 - May 31
- Summer: June 1 - August 14

If Session Log exceeds 15 rows, run the archival process: summarize oldest entries into Historical Summary, keep most recent 10 rows.

### Step 2: Timeline Status Check

For every milestone in the student's current grade and all previous grades, assign a status:

| Status | Meaning | How to Assign |
|--------|---------|---------------|
| **Ahead** | Completed before the expected semester | Milestone finished before the semester listed in timeline-engine |
| **On Track** | Completed during the expected semester | Milestone completed during its listed semester |
| **Coming Up** | Due this semester, not yet done | Current semester matches the milestone's semester, incomplete |
| **Behind** | Past the expected semester, not completed | Current date past the milestone's semester, still incomplete |
| **N/A** | Not yet relevant | Milestone belongs to a future grade/semester |

**Check each milestone against state**:
- Exploration milestones: check Interest Discovery section (Holland Code, flow activities, strengths, values)
- Academics milestones: check Academic Track section (track mapped, courses planned, rigor level)
- Activities milestones: check Activities & Spike section (spike identified, leadership roles, activity depth)
- Testing milestones: check Testing section (PSAT, practice tests, official scores, AP exams)
- Schools milestones: check College List section (list built, research done, visits, demonstrated interest)
- Essays milestones: check Essays section (brainstorming, drafting, revision status)
- Applications milestones: check College List strategies and Recommendations section
- Financial milestones: check Financial section (FAFSA, CSS Profile, net price calculators, scholarships)
- Summer milestones: check Summer Experiences section

**Framing guidance for "Behind" items**: Use Motivational Interviewing voice. Frame gaps as opportunities, not failures.
- Say: "You haven't gotten to [X] yet — no stress, now is a great time to tackle it."
- Never say: "You're behind on [X]" or "You should have done this by now."

Update the Timeline Status section in `counseling_state.md` with current milestone statuses.

### Step 3: Section-by-Section Assessment

Evaluate each area of the student's profile for completeness and quality:

**Interest Discovery**:
- Has the student completed initial interest exploration? (Phase 1-3 of elicitation)
- Are interests evolving or stagnant? Check the interest evolution log.
- Does the student need a refresh? (last discovery was 6+ months ago, or student seems unsure)

**Academic Track**:
- Is a track mapped? (primary + secondary interests)
- Are courses aligned with the track and spike?
- Is rigor appropriate for the student's targets? (relative to what the school offers)
- GPA trajectory: improving, steady, or declining?

**Activities & Spike**:
- Is a spike identified? (1-2 deep focus areas)
- Is depth growing? (participation -> leadership -> impact -> recognition)
- Leadership positions secured?
- Are there gaps in the activity profile that the student could address?

**Testing**:
- On track for target scores relative to college list?
- Prep plan in place and progressing?
- Practice vs. official scores: improving?
- AP exams planned and aligned with track?

**College List**:
- Is the list built? (2-3 reach, 4-5 match, 2-3 safety)
- Has the student researched schools beyond name recognition?
- Demonstrated interest actions underway? (visits, info sessions, interviews)
- Are safeties genuine — schools the student would actually attend?

**Essays**:
- Personal statement: brainstorming started? theme identified? drafting?
- Supplemental essays: prompts researched? drafts in progress?
- Narrative thread: does the application tell a cohesive story connecting spike, courses, activities, and essays?

**Financial**:
- FAFSA awareness and timeline?
- Net price calculators run for target schools?
- Scholarship research and calendar started?
- CSS Profile needed and on track?

**Summer**:
- Have past summers included meaningful experiences?
- Are experiences connected to the spike?
- Is the upcoming summer planned?

### Step 4: Grade-Appropriate Focus

Weight the assessment toward what matters most for the student's current stage:

**Freshman (Grade 9)**:
- Primary focus: interests, activities, GPA foundation
- Light touch on: everything else (it's early — don't overwhelm)
- Tone: "You're in great shape just by thinking about this early. Here's what to focus on..."

**Sophomore (Grade 10)**:
- Primary focus: spike depth, course rigor increase, testing introduction (PSAT), summer planning
- Secondary: preliminary college awareness, activity leadership
- Tone: "You're building momentum. The key moves this year are..."

**Junior (Grade 11)**:
- Primary focus: testing, college list, essay brainstorming, recommendations, summer planning
- Secondary: course rigor, activity peak achievement
- Tone: "This is the most important year for your applications. Let's make sure you're set on..."

**Senior (Grade 12)**:
- Primary focus: applications, essays, financial aid, decisions
- Secondary: maintaining grades, scholarship applications
- Tone: "You're in the home stretch. Here's where things stand and what needs your attention..."

### Step 5: Recommendations

Synthesize the assessment into actionable guidance. Always lead with strengths.

1. **What's going well** (2-3 specific strengths): Identify areas where the student is on track or ahead. Be genuine and specific — not generic praise.
2. **Top 3 priority actions**: Based on gaps, timeline pressure, and grade-appropriate focus. Each should be:
   - Specific and actionable
   - Linked to a command the student can run
   - Ranked by urgency and impact
3. **Looking ahead**: Preview 1-2 milestones from the next semester to build awareness without creating pressure.

When multiple areas need attention, prioritize:
1. Items with approaching deadlines (FAFSA, applications, test dates)
2. Items that are prerequisites for other work (interests before course planning, college list before essays)
3. Items with the highest impact for the student's grade level
4. Items the student has shown energy or interest around (leverage motivation)

### Output Schema

Return exactly:

```markdown
## Progress Review — [Name], Grade [X], [Semester] [Year]

### Timeline Status
[Use timeline-engine output format]

#### Coming Up This Semester
.. [Milestone] — [one-line action step]
.. [Milestone] — [one-line action step]

#### Opportunities to Catch Up
!! [Milestone] — [MI-framed encouragement + suggested next step]

#### On Track
-- [Milestone] — [brief acknowledgment]

#### Ahead
>> [Milestone] — [brief acknowledgment + what this enables]

### What's Going Well
- [Specific strength with evidence from state]
- [Specific strength with evidence from state]
- [Specific strength with evidence from state]

### Priority Actions
1. **[Action]** — [why it matters + which command]. [Urgency context.]
2. **[Action]** — [why it matters + which command].
3. **[Action]** — [why it matters + which command].

### Looking Ahead
[1-2 items from the next semester — framed as preview, not pressure]

**Recommended next**: `[highest priority command]` — [reason based on the most urgent gap]. **Alternatives**: `[command]`, `[command]`, `help`
```

### State Updates

Write to `counseling_state.md`:

- **Timeline Status**: Refresh all milestone statuses with current check results, update "Last check" date
- **Session Log**: Record review command run with key findings (e.g., "Review: 2 milestones behind, 5 on track, 1 ahead. Priorities: testing prep, college list building")
- **Active Counseling Strategy**: Reassess current focus based on review findings. If priorities have shifted, update the strategy (move old approach to Previous approaches, write new focus/approach/rationale)
- **Coaching Notes**: Capture any observations from the review (e.g., "student seems overwhelmed by testing timeline," "strong momentum in activities — leverage this energy," "financial planning is a blind spot — surface proactively next session")
