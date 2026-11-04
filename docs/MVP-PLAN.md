# Gen Boserydhek — CV website MVP plan

Status: proposed delivery plan; implementation has not started.
Prepared: 04/11/2026. Time zone: Europe/London.
Initial product version: **0.0.0 (Alpha)**; machine-readable version: **0.0.0-alpha**.
Repository: https://github.com/Codewave-Studio-UK/bosrydhek-resume
Working branch: **dev**. Production branch: **main**.

## 1. Product goal and success

Create a two-page personal CV website that lets a prospective client or reviewer understand Gen's current capabilities, experience and interests, inspect an honest project summary, and make contact.

The primary audience is people considering Gen for generalist AI contract work: response review, research, factual accuracy checking, written feedback and related tasks. AI-assisted development / vibe coding is secondary. The site is a general CV.

Success at launch means that visitors can find the relevant skills, understand the early-stage experience and send an email; both pages pass the release checks below. Job offers, platform acceptance and a particular volume of enquiries are not promised outcomes.

Official DataAnnotation generalist descriptions emphasise reading, writing, evaluating responses and explaining judgements. Outlier describes related tasks including prompts, rubrics and ranking answers. These inform content emphasis, not claims about Gen's qualifications or eligibility. Individual opportunities have different requirements. [S3–S4]

## 2. Verified inputs and current state

### User-confirmed content

- Public name: **Gen Boserydhek**.
- Supplied pronunciation: **gh-EN boss-RITH-ek**.
- Public location: **Westcountry, United Kingdom**. No exact town or home address supplied.
- Public contact address: **ascent.asian9180@eagereverest.com**. Use this address for visible text, mail links and copy actions.
- Primary interest: generalist freelance and contract work, including work through AI training platforms. Secondary interest: vibe coding.
- Developing Codewave Studio as an early-stage AI-native website and application development venture.
- Learning through independent research, planning, documentation and AI-assisted development.
- Terry is a private work-in-progress project for AI-assisted research, product requirements and technical specification writing.
- The supplied tool list is practical familiarity, with differing experience levels. It does not establish expert proficiency or credentials.
- Profile links will be added in the next MVP version.
- Projects are private WIP; the user plans to create public practice examples later.

Treat the supplied CV as autobiographical information provided by Gen, not independently verified employment evidence. Preserve its cautious descriptions of developing skills.

### Directly inspected on 04/11/2026

- The organisation repository is public and accessible through GitHub.
- The default branch is dev.
- dev and main both exist and initially pointed to c691ff60da86503a5a756ea59142a6c0ae20d316.
- The repository initially contained only a short README.
- Both branches were reported as unprotected.
- Netlify exposes the Codewave Studio team, slug codewavestudiohq, on a Free plan.
- Both a resume-name search and an unfiltered project list returned no projects through the connected Netlify account. This does not establish whether an unfinished setup wizard, a different account or an otherwise inaccessible project exists.

### Source limitations

The shared ChatGPT link returned a metadata-only page, without the conversation. The pasted CV is sufficient to plan this MVP. The exact practice-project suggestions in the earlier chat have not been retrieved; the proposals in section 11 are new suggestions.

The founder start date is unknown. Omit the date in the MVP. Do not publish a placeholder or infer a date from repository activity.

## 3. Scope and content

Two primary pages, with the same simple navigation: **CV · Projects · Email Gen**.

| Page | URL | Content |
| --- | --- | --- |
| CV | / | Name, generalist-first headline, short introduction, work sought, skills, independent experience, tools, ongoing learning and contact |
| Projects | /projects/ | Terry's purpose, private/in-development status, Gen's current planning/documentation contribution, developing skills and contact |

The CV page should read like a person describing their work. A possible opening, derived from the supplied draft:

> I'm building Codewave Studio and developing my skills in AI-assisted research, product planning and digital workflows. I'm looking for generalist contract work involving AI response review, research and clear written feedback. Alongside this, I'm learning to build websites and apps with AI tools.

Suggested headline: **AI Generalist | AI-Native Founder**. Product-building detail belongs in the body so the first impression matches the main work sought.

Keep skills and tools easy to scan. Use plain lists and brief explanations of practical use. Do not use proficiency percentages, star ratings, invented work outcomes or years-of-experience counters.

For Terry, publish only the high-level summary already supplied in the CV. State **Independent project — private, in development**. Describe research, requirements and documentation work. Do not imply that a working product, paying customers or measured outcomes exist. No private screenshots, client material, specifications or source excerpts.

A useful Projects page can start with one real project. Practice samples enter the page only after Gen has created and reviewed them.

Contact is a visible email address and a mailto link. Optional copy-to-clipboard supplements the link. A contact form is outside this initial scope. No phone number or profile-link placeholders.

MVP includes a clean browser-print layout for the CV. A downloadable PDF is a later deliverable unless specifically requested; no inactive download button.

## 4. Visual direction and interaction

### Direction: a warm, contemporary CV

Use a warm off-white surface, dark readable text and a restrained deep green accent. Final colours must pass measured contrast checks. A clear typographic hierarchy, deliberate spacing and fine dividers give the site its character.

Use a readable single-column layout on phones. On wider screens, a quiet secondary column can hold contact and compact facts, with the main reading column kept comfortable. Suggested prose width: about 60–70 characters, adjusted through visual testing.

Use **DM Sans from Google Fonts**, with a system sans-serif fallback. One font family keeps the system coherent. Google's description identifies DM Sans as intended for smaller text sizes. Self-host a small WOFF2 subset and retain its licence. This satisfies the Google Fonts requirement while avoiding a runtime font request to Google. [S7–S9]

Design references:
- Dribbble resume-website and resume-portfolio collections: inspect hierarchy and compact presentation.
- Behance resume-website collection, including its personal CV examples: inspect information order and spacing.
- Awwwards typography collection: requested reference; the primary page timed out during research and still needs direct visual review.
- One Page Love's personal/CV examples: an additional reference for small interaction details.

These are inspiration sources, not evidence of recruiting effectiveness. Take principles from them and create an original composition. Do not reproduce artwork or copy. Avoid developer-specific presentation cues that distract from generalist work.

### Typography and vertical rhythm

Widths below are proposed starting breakpoints, to be checked against actual content. Device names are shorthand; viewport width drives the layout.

| Viewport width | Base font at a default 16px browser setting | Base line height | Relative root setting |
| --- | --- | --- | --- |
| Below 768px | 14px = 1rem | 22px; ratio 22/14, approximately 1.5714 | 87.5% |
| 768px–1439px | 16px = 1rem | 26px; ratio 26/16 = 1.625 | 100% |
| 1440px and above | 18px = 1rem | 30px; ratio 30/18, approximately 1.6667 | 112.5% |

Use the exact line-height ratios, rather than the rounded 1.57 or 1.66 values, when matching 22px and 30px. Percentage root sizes retain scaling relative to the visitor's default font setting.

Use a Major Third ratio of **1.250** for the type scale: 1, 1.25, 1.5625, 1.953125 and 2.44140625rem. Choose an appropriate step per heading and viewport; do not force long names or headings into a single line.

Base spacing on the current body line-height: 0.5, 1, 1.5, 2 and 3 line-height units. Give headings suitable line heights and space them to rejoin the rhythm. Borders and visual details may need optical adjustment.

The requested 14px mobile base still needs real-phone readability and enlargement checks. Pixel size alone does not establish accessibility. Test text resizing, browser zoom and spacing overrides. [S6]

### Motion and the two small surprises

1. An accessible “How to say my name” control reveals the user-supplied pronunciation. It works by keyboard and touch. No synthesised pronunciation or invented recording.
2. A subtle contact-link underline and optional copy confirmation add a small responsive detail.

Use short transitions, approximately 120–220ms as a project design choice. If a light entrance effect is useful, run it once and keep the content visible without JavaScript. Essential information must never depend on completing an animation.

Respect prefers-reduced-motion. Keep decorative movement off in that mode. No autoplay audio, looping visual effects, scroll hijacking or motion library.

## 5. Technical approach

Use buildless semantic HTML, modern CSS and a small progressively enhanced JavaScript file. This is proportionate to two public content pages with simple interactions. No runtime framework, server functions, accounts, CMS or database are required by the agreed scope.

Proposed structure:

- site/index.html — CV.
- site/projects/index.html — Projects.
- site/404.html — useful error response, outside the two-page content/navigation structure.
- site/assets/css/site.css — shared design system, responsive layout and print rules.
- site/assets/js/site.js — optional pronunciation/copy enhancements.
- site/assets/fonts/ — self-hosted Google Fonts WOFF2 and licence.
- netlify.toml — publication directory, appropriate headers and preview behaviour.
- VERSION, CHANGELOG.md, README.md and AGENTS.md — version, change history, setup and focused coding/content rules.
- docs/ — plan, content decisions and verification evidence.

Main content, navigation and email contact must work without JavaScript. Use native HTML controls where suitable. A custom 404 must return the correct status; no blanket single-page-app rewrite.

Keep deployment state and secrets out of Git. Add .netlify to .gitignore when linking Netlify; also ignore local environment files. Do not store the private email address or confidential project material anywhere in repository content or generated output.

Add page titles, descriptions, a favicon and verified public metadata. Canonical URLs and any production sitemap must use the actual final production address. Do not invent profile links or employment metadata.

## 6. Agile workflow, branches and versioning

Use a lightweight agile workflow with a prioritised backlog, one goal per sprint, small demonstrable increments, review and adaptation. This is a solo-with-AI adaptation. Four hours is the user's chosen sprint timebox; the official Scrum Guide defines sprints as one month or less and does not prescribe this project's branch model. [S1–S2]

### Branch policy

- All MVP work integrates on dev.
- Small feature/fix branches may branch from dev where useful; their pull requests target dev.
- main receives a release through a dev-to-main pull request only after the release gates pass.
- Do not merge unfinished application code into main to make deployment easier.
- Each change has a focused commit and relevant verification. Do not force-push shared branches.
- GitHub checks should run on pull requests and on dev/main changes. Use available repository rules to prevent bypassing release checks; verify the current account/plan capability before claiming enforcement.
- Preserve the existing default branch unless there is a concrete reason to change it.

No branch-protection change is claimed as completed by this plan.

### Version policy

Display the initial version as **0.0.0 (Alpha)** and store **0.0.0-alpha** as the SemVer-compatible value. The alpha label is significant; 0.y.z indicates initial development. Versioning describes accepted releases, not elapsed sprints or commit counts. [S5]

| Stage | Example version | Gate |
| --- | --- | --- |
| Initial runnable alpha | 0.0.0-alpha | Functional foundation on dev |
| Further alpha iterations | 0.0.0-alpha.1, 0.0.0-alpha.2 | Accepted fixes or improvements |
| Feature-complete review | 0.1.0-beta.1 | Full MVP scope available for review |
| Release candidate if useful | 1.0.0-rc.1 | Release checks passed, final review pending |
| First stable production release | 1.0.0 | All release gates passed |

These are project release conventions. SemVer does not prescribe a sprint-to-version mapping. Tag only an actual accepted release, record its commit and changes, and never move a published version tag to different contents.

For this website, document the stable public surface as the two page routes, content accessibility and contact actions. After 1.0.0, use patch releases for corrections, minor releases for compatible features and major releases for deliberately incompatible public behaviour.

### Four-hour sprint structure

Each sprint totals 240 minutes:
- 10 minutes: select the goal and acceptance criteria.
- 180 minutes: implement and verify small changes continuously.
- 30 minutes: complete the sprint's focused QA.
- 15 minutes: review the working increment.
- 5 minutes: record lessons and adjust the backlog.

Do not lower quality or claim completion to fit the timebox. Carry incomplete work forward. Time estimates are planning assumptions, not guaranteed delivery times; no start times or calendar dates are booked.

## 7. Proposed delivery backlog

Three four-hour sprints are the initial forecast: **12 hours of delivery capacity**, subject to learning and integration access.

| Sprint | Goal | Main backlog items | Demonstrable result |
| --- | --- | --- | --- |
| 1 — Foundation | An honest, usable CV and Projects structure on dev | CV-01 content editing; CV-02 Terry summary; CV-03 semantic pages, navigation, contact and print baseline; CV-04 version and project rules | Both pages readable on mobile and desktop, no placeholders, initial 0.0.0-alpha |
| 2 — Presentation | Complete the visual design and small interactions | CV-05 font, type scale and rhythm; CV-06 responsive layout and contrast; CV-07 pronunciation/copy enhancements and reduced motion; CV-08 Netlify dev preview when the project is identified | Feature-complete review build; beta only if accepted |
| 3 — Release | Establish evidence of stability and prepare production | CV-09 accessibility/content checks; CV-10 performance/behaviour checks; CV-11 deployment configuration, release notes and dev-to-main review; CV-12 verify production | Stable release only when gates pass; otherwise remain on dev |

MVP priorities:
- Must: truthful CV, accurate Terry status, both pages, masked email, responsive typography, Google Fonts, keyboard access, reduced motion, lightweight delivery, dev/main separation and verification evidence.
- Should: pronunciation reveal, email-copy enhancement, print layout and small visual refinements.
- Later: profile links, completed public practice samples, a downloadable PDF, custom-domain refinements and additional projects.

If time is constrained, defer an optional interaction before sacrificing content, accessibility or release checks.

## 8. Netlify setup and deployment

### Current setup gap

No projects are visible through the connected Netlify account. Identify the user's in-progress project by its dashboard URL or site ID before creating another one. Do not treat an empty project list as permission to duplicate a project being created elsewhere.

The available Netlify management tools can inspect teams/projects and create an empty project, but they do not expose a repository-link or production/branch-build-settings write operation. Those settings need an authorised supported configuration route or a short dashboard handoff. Do not claim Git continuous deployment is linked merely because a project was created.

### Intended configuration

| Setting | Value |
| --- | --- |
| Team | Codewave Studio / codewavestudiohq |
| Git provider | GitHub |
| Repository | Codewave-Studio-UK/bosrydhek-resume |
| Production branch | main — explicitly set; GitHub currently defaults to dev |
| Development branch deploy | dev |
| Publish directory | site |
| Build command | None for the buildless site |
| Runtime functions / database | None |
| Production audience | Public once the stable CV is ready |
| Initial domain | Verified Netlify-provided address unless an existing custom domain is supplied |

Netlify's development context name does not by itself enable Git branch deployments. Enable dev explicitly in the project's branch/deploy settings. Keep production tied to main. Confirm current visibility and any initial-build behaviour before connecting the repository; do not publish alpha work on the production address. [S10–S12]

Add noindex response headers to development/preview output and verify them. Noindex is an indexing request, not access control. Treat shareable previews as potentially public unless effective access protection has been verified. Never put private WIP material in them.

The current credit-based Free plan includes 300 credits/month. Production deploys consume 15 credits; bandwidth and requests also consume credits, and sites pause when the allowance is exhausted. Preview/branch deployments have no deployment credit charge, but their traffic can still consume credits. Legacy plans can differ; use the actual team's billing context. Batch accepted production changes and review actual usage. Do not upgrade a plan or enable paid add-ons as part of this MVP. [S13–S15]

Deployment verification must identify the branch, commit SHA, final URL and successful deploy state. Smoke-test the CV, direct /projects/ navigation, unknown-route response, email link, assets and relevant headers.

If a published change is faulty, fix or revert the source commit and let the pipeline deploy the correction. A failed unpublished deployment does not replace the previous live version.

### Later repository transfer

When the user transfers the repository to their personal account, recheck GitHub app and Netlify integration access, repository URLs, branch/deployment settings and automatic deployment. Verify a new dev deployment. Do not assume redirects alone preserve integration permissions. A transfer is outside this MVP's current actions.

## 9. Quality targets and release gates

The following are **targets and acceptance criteria**, not measured results. No application has been implemented or tested yet.

### Content and function

- Name, pronunciation, location and masked email match the supplied information.
- No invented education, employment, certificates, clients, results, platform experience or start dates.
- Terry is clearly private and in development.
- No public claim of completed practice projects.
- No real private email address, confidential material, placeholder tokens, dummy links or inactive actions in files, metadata or output.
- Both page routes and a useful 404 work by direct URL.
- Main reading/navigation/contact experience works without JavaScript.
- Copy feedback, if included, is announced accessibly and failure leaves the email link usable.
- CV prints in a sensible reading order.

### Accessibility and responsive behaviour

Target WCAG 2.2 AA for applicable criteria; do not claim certification from an automated score. [S6]

- Semantic landmarks, logical headings, descriptive links and current-page indication.
- Visible keyboard focus, skip link, keyboard/touch operation and no focus traps.
- Minimum 4.5:1 contrast for normal text; assess applicable large-text and UI contrast criteria.
- Aim for 44px interactive targets as a project usability choice, with adequate spacing.
- Check 200% text resizing, 400% browser zoom/reflow, text-spacing overrides and reduced motion.
- Check widths including 320, 375, 390, 768, 1024, 1440 and 1920px, plus landscape.
- Check long headings, font failure, mail-link wrapping and large user-default fonts.
- Run automated accessibility checks and manual keyboard/screen-reader smoke checks where tools allow. Record the actual browsers, devices and assistive technologies tested; report missing coverage.

### Performance

Project budgets per page on a cold cache:
- Initial compressed transfer: at most **200kB**, including fonts and page assets.
- Compressed JavaScript: at most **10kB**.
- Compressed CSS: at most **20kB**.
- Fonts: at most **80kB** in the initial transfer.
- No large hero image, video or runtime UI library.

Record compressed network bytes; do not compare these budgets to uncompressed file sizes.

Aim for LCP at most 2.5 seconds, INP at most 200ms and CLS at most 0.1, the current Core Web Vitals good thresholds. Field assessment uses the 75th percentile of real visits. A new, low-traffic site may lack field data. Lab results do not establish a field INP pass. [S16]

Before release, take three cold-load runs per page on a documented mobile/4G test profile and inspect representative interactions. Record device/CPU/network settings, tool versions and variation. Use a Lighthouse mobile performance score of at least 95 as an investigation target, alongside actual metrics and visual checks; a score alone is insufficient. Use TBT as a lab indicator where appropriate, not as a renamed INP result.

5G support follows from the same lightweight, responsive experience; actual mobile network conditions vary. Verify failure behaviour as well as a fast connection.

### Security, privacy and deployment

- HTTPS and appropriate security headers; test a restrictive content security policy against actual assets and interactions.
- No secrets, private contact address or confidential project material in repository/output.
- Self-host the selected Google Fonts files with licence retained.
- No optional analytics, advertising, tracking pixels, third-party embeds or site-set storage in the initial scope.
- Review the final deployment's actual requests, cookies and storage before deciding whether consent controls are needed.
- Provide a concise, accurate privacy explanation within the two-page layout as applicable, covering hosting/request logging and email contact using verified provider practices. Do not claim that a static site processes no personal data.
- Apply current ICO guidance, including the 29/04/2026 storage/access guidance. Reassess if features or tracking change. [S17–S18]
- Successful dev deployment and recorded checks against the release commit.
- No unresolved critical/high-impact content, accessibility, security or functional defects.
- Final review against the user's requirements; then the dev-to-main release pull request can be merged.
- Confirm the production deploy and smoke tests before calling the release complete.

## 10. Challenge-and-verification loop

For each material choice:
1. Identify the requirement, assumption and source.
2. Challenge the choice with a relevant failure case.
3. Verify against authoritative guidance or a representative test.
4. Revise the design/code and recheck only the affected areas.
5. Record the evidence, remaining limitation and acceptance decision.

| Assumption or risk | Challenge | Planned response |
| --- | --- | --- |
| Strong visuals help the purpose | They may obscure skills or suggest a developer portfolio | Lead with generalist work and readable CV content; treat aesthetic effectiveness as a hypothesis |
| Early-stage experience is sufficient to describe | Overstatement could undermine credibility | Use the supplied experience and project status; omit unsupported dates and outcomes |
| Four hours will fit the work | Integration or QA can exceed the estimate | Fixed timebox, adjustable scope, no reduced quality |
| 14px mobile text is readable | Small text, zoom or long copy can fail for visitors | Test actual content, enlargement and device layouts |
| Google Fonts require external calls | Added requests and unnecessary data disclosure | Use licensed self-hosted font files and verify network requests |
| A preview is private | Links or indexing may expose it | Use only public CV content; verify visibility and noindex behaviour |
| A Lighthouse result proves performance | Lab/field and devices can differ | Record the test profile and limits; do not invent field measurements |
| Existing Netlify setup is accessible | The connection returns no projects | Identify the correct project before creating/linking |
| main equals stable | Branch name does not establish quality | Require the documented release checks and review |
| A static site has no privacy obligations | Hosting and email may involve personal data | Verify actual processing and provide proportionate information |

## 11. Future practice samples

These are optional new suggestions, not work Gen has completed and not a reconstruction of the inaccessible chat:

1. **AI response comparison:** compare two answers using an explicit rubric for instruction-following, accuracy, clarity and usefulness; explain the judgement.
2. **Small fact-checking exercise:** check a limited set of public factual claims, show primary sources, dates, corrections and unresolved uncertainty.
3. **Prompt-and-response improvement:** show an initial task, shortcomings, a revised prompt/answer and what changed, with a short evaluation.

Use self-created tasks and public material. Do not publish confidential assessments or platform tasks. Publish samples only after the underlying work exists and Gen has reviewed it.

## 12. Decisions still open

- Netlify project dashboard URL or site ID, if the project has already been created. If setup is unfinished, identify that state before making an empty project.
- Founder start month/year: optional; omitted until supplied.
- Profile links: explicitly deferred to the next version.
- Exact projects suggested in the original chat: not retrieved; not needed to launch the honest MVP.
- Final design and wording remain reviewable during the planned iterations.

## 13. Evidence register

Sources checked on 04/11/2026. Prefer current official documentation. Use 2026 updates where relevant; publication in 2026 alone does not supersede a current authoritative standard. Do not describe older or undated pages as 2026 publications.

| ID | Source | Use / publication note |
| --- | --- | --- |
| S1 | https://agilemanifesto.org/principles.html | Original agile principles: working increments, simplicity, feedback |
| S2 | https://scrumguides.org/download and https://scrumguides.org/scrum-guide.html | Official current guide listed as November 2020; sprint framework, not a mandated four-hour method |
| S3 | https://www.dataannotation.tech/job-board/generalist | Official current role description; content emphasis only; no pay/eligibility promise |
| S4 | https://outlier.ai/ | Official task descriptions; no claim Gen meets every role requirement |
| S5 | https://semver.org/ | Semantic Versioning 2.0.0; pre-release syntax and initial development |
| S6 | https://www.w3.org/TR/WCAG22/ | W3C Recommendation dated 12/12/2024; applicable accessibility criteria |
| S7 | https://github.com/google/fonts/blob/main/ofl/dmsans/DESCRIPTION.en_us.html | Official DM Sans description |
| S8 | https://github.com/google/fonts/blob/main/README.md | Official font repository and self-hosting route |
| S9 | https://web.dev/learn/performance/optimize-web-fonts | Primary browser-performance guidance on web fonts |
| S10 | https://docs.netlify.com/build/git-workflows/overview/ | Git integration |
| S11 | https://docs.netlify.com/build/configure-builds/file-based-configuration/ | File-based configuration; production branch is configured in project settings |
| S12 | Netlify connected deployment guidance, retrieved 04/11/2026 | Branch-deploy setup, visibility, noindex caveats and fix-forward process |
| S13 | https://www.netlify.com/pricing/ | Current published Free allowance; verify actual account plan |
| S14 | https://www.netlify.com/changelog/2026-04-14-pricing-updates-april-2026/ | 14/04/2026 official metering update |
| S15 | https://docs.netlify.com/manage/accounts-and-billing/billing/billing-for-credit-based-plans/how-credits-work/ | Credit consumption, preview distinctions and site pausing |
| S16 | https://web.dev/articles/vitals | Primary thresholds and distinction between lab/field measurements; last updated 31/10/2024 |
| S17 | https://ico.org.uk/for-organisations/direct-marketing-and-privacy-and-electronic-communications/guidance-on-the-use-of-storage-and-access-technologies/ | Official guidance update 29/04/2026 verified through indexed content; direct full-page fetch returned 403 |
| S18 | https://www.scl.org/ico-publishes-final-storage-and-access-technologies-guidance/ | Society for Computers & Law, 01/05/2026; independent corroboration of the ICO update |
| D1 | https://dribbble.com/tags/resume-website and https://dribbble.com/search/resume-portfolio | Primary inspiration collections; no hiring-effectiveness inference |
| D2 | https://www.behance.net/search/projects/resume%20website?locale=en_US | Primary inspiration collection; no asset/copy reuse |
| D3 | https://www.awwwards.com/websites/typography/ | Requested inspiration reference; primary-page fetch timed out, visual review pending |
| D4 | https://onepagelove.com/jonathan-moore | Personal/CV interaction reference published 13/05/2026; use small details proportionately |
