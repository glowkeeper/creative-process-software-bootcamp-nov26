# Creative Process Software Development Bootcamp

Welcome to the Software Development Bootcamp.

Across eight weeks, you will develop an individual prototype. You will plan,
build, test, improve and present your work while learning the foundations of
modern web development.

MarBelle, Co-Founder and Editor-in-Chief of [Directors
Notes](https://directorsnotes.com/), will introduce the client context in Week 1
and return for the Week 8 prototype presentations.
Your work may inspire ideas for the publication, but you are creating an
independent learning prototype rather than production software for its live
website.

> My goal isn't to build software with AI. My goal is to become a software
> developer who knows how to use AI well.

## Your Project

You choose one of two routes:

- **A Directors Notes brief.** Choose one of the ten supplied [prototype
  briefs](docs/weeks/week-01/project-briefs.md). Your project remains closely
  connected to that brief throughout the bootcamp. Learners on a Directors
  Notes brief receive a £100 participation payment.
- **A project of your own.** Discuss your idea with the lead tutor in Week 1.
  Do not start building until it has been agreed and scoped. You present to
  MarBelle in Week 8 like everyone else, but the £100 participation payment is
  for the Directors Notes briefs only.

Several learners may choose the same brief. Every response remains individual:
you will create your own repository, Project board, design, code and Week 8
presentation.

Begin with your **Starting Point**, the smallest meaningful prototype.
**Possible Directions** are optional ideas for later, after your current
prototype works and you can explain it.

## Your Eight-Week Journey

| Week | Focus |
| --- | --- |
| 1 | Choose a brief or agree your own project, and establish your development workflow |
| 2 | Create the first visible interface with HTML and CSS |
| 3 | Add meaningful behaviour with JavaScript and the DOM |
| 4 | Begin a staged migration using React components and props |
| 5 | Read, review and restore important behaviour in React |
| 6 | Make an appropriate part of the application remember information |
| 7 | Build, debug, simplify and stabilise your prototype |
| 8 | Deploy and rehearse in the morning, then present to MarBelle |

The course gives you more independence over time. A small prototype you
understand is more valuable than a larger application you cannot explain.

## Shared Reference Application

From Week 2, the tutor will demonstrate weekly concepts through a Short Film
Programme Builder. It explores how someone might assemble a screening programme
within a running-time limit.

The reference application demonstrates development patterns without solving
your project for you. You will decide how each useful pattern applies to your
own prototype.

Reference states and later course materials will be added to this repository
week by week as they are delivered.

## Course Materials

Each week's slides, worksheet and resources are in [`docs/weeks`](docs/weeks/),
in a folder for that week, such as `docs/weeks/week-01`. Reference application
states are in [`src`](src/), organised the same way. Folders appear as each week
is delivered.

## Your Individual Repository

This cohort repository contains shared course material. Your prototype belongs
in a separate repository under your own GitHub account.

Your individual repository should contain:

- Your README
- Your source code
- Your project history
- A link to your GitHub Project board
- Evidence of your decisions and progress

Create small commits with messages that explain what changed. Push regularly so
GitHub contains a recoverable history of your work.

Plan your work with GitHub issues and your Project board. The issue templates in
this repository's [`.github/ISSUE_TEMPLATE`](.github/ISSUE_TEMPLATE/) folder
show a useful structure: a short **Why** and a **Done when** checklist, so that
anyone could tell whether the issue is finished. To use them, copy that folder
into your own repository. [Working With AI](#working-with-ai) shows how to
use an issue to direct an assistant.

## Content and Data Boundary

Do not copy Directors Notes photographs, film stills, videos, logos, article
text or archive records into your repository or deployed prototype.

The course provides a wholly fictional film archive, available in
[`datasets/fictional-film-archive`](datasets/fictional-film-archive/) from
Week 2, so that you can use as much or as little of it as your project needs. You may adapt, commit and publish that teaching data and
artwork. You may also use your own
writing or artwork, abstract placeholders, HTML and CSS visual treatments, or
openly licensed assets with the required attribution. Record the source and
licence of anything created by someone else. If you are working on your own
project, you must own the content you publish or have permission to use it.

The original Directors Notes project pack is private client reference material
and will not be distributed through this repository.

## Working With AI

AI is part of software development now. You may build without it, use it to
learn and check your work, or use it to help you build. All three are
legitimate, and every outcome in this course can be achieved without it.

Whichever route you take, you remain the developer. Before keeping any code,
make sure you can:

- Read it
- Explain it
- Test it
- Change it
- Take responsibility for it

Never paste private client material, credentials or personal information into
an AI service. The Week 1 slides introduce the shared agreement, and Week 2
practises it.

### Start With an Issue

Whether or not you use AI, the most useful habit is to decide what you are
doing before you do it. Write a small GitHub issue first, using the templates in
[`.github/ISSUE_TEMPLATE`](.github/ISSUE_TEMPLATE/): a short **Why** and a
**Done when** checklist. If you cannot say how you would know the issue is
finished, it is not ready to work on.

If you use an AI assistant to help you build, the issue is how you direct it.
Give it the issue, not a vague wish:

1. **Write the issue.** One small task you can finish and test in a sitting.
2. **Give the assistant its context.** An [`AGENTS.md`](AGENTS.md) file tells an
   assistant what the project is and how to work on it. This repository has one,
   and you can adapt it for your own repository.
3. **Ask for a plan first.** Read it, and change it, before any code is written.
4. **Ask for one small change at a time.**
5. **Read the change, run it and test it** against the **Done when** list.
6. **Commit when it works**, naming the issue in the message, then move the card
   on your Project board.

If you build without AI, the same issue is your plan, and steps 4 to 6 are your
own work. Either way, you decide what is done.

From Week 2 the tutor demonstrates this workflow using the issues in this
repository.
