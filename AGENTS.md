# AGENTS.md

This file tells an AI coding assistant how to work in this repository. It is
also an example for you. It is short, it says what the project is, and it gives
an assistant the context a new teammate would need. Writing one for your own
project is optional.

## What this repository is

Shared material for the Creative Process Software Development Bootcamp, and the
Short Film Programme Builder, a reference application that the tutor builds in
front of the class from Week 2. It helps a visitor assemble a screening
programme within a running-time limit.

It is a teaching example, not a product. Learners build their own prototypes in
separate repositories.

## Layout

```text
docs/weeks/week-NN/                      slides, worksheet and resources
src/week-NN/starter|complete|showcase/   reference application states
datasets/fictional-film-archive/         wholly fictional teaching data
.github/ISSUE_TEMPLATE/                  templates for tasks and bugs
```

Material is added week by week, so not every folder exists yet. Put new files
inside this layout. Do not create new top-level folders.

## How to work

- Work on one GitHub issue at a time. Its **Done when** list is the finish line.
- Start with a short plan and wait for approval before changing files.
- Make one small change at a time and explain it in plain language.
- Do only what the issue asks. Do not add features, files or libraries that it
  does not mention.
- Use only the techniques the course has introduced up to the current week. For
  example, Week 2 has no JavaScript and Week 3 has no React.
- Prefer clear, explicit code a beginner can read over clever shortcuts.
- Say when you are unsure. Do not invent properties, attributes or APIs.
- Check the result in the browser and report how you checked it.
- Commit when it works, with a message that names the issue, for example
  `Lay out film cards in a responsive grid (#4)`.

## Issues

Issues use the templates in `.github/ISSUE_TEMPLATE/`: `task.md` for work to do
and `bug.md` for something that is wrong.

- When asked to write an issue, use the matching template's headings: **Why**,
  **Done when** (three to five items someone could check in the browser) and, for
  a task, **Leave for later**. Keep it small enough to finish and test in one
  sitting.
- Show the draft and wait for approval. Create the issue on GitHub only when
  asked.
- When asked to work on an issue, read it first. Use `gh issue view <number>`,
  or ask for it to be pasted. Treat **Done when** as the finish line. If the
  issue is vague or too large, say so and suggest how to split it. Do not guess.

## Running a React state

From inside the state's folder, for example `src/week-05/complete/`:

```bash
npm ci          # install exactly what package-lock.json says
npm run dev     # start the development server
npm run lint    # check the code
npm run build   # make a production build
```

## Content and data

- Use only the fictional archive, placeholder artwork and your own content.
- Never add real film stills, logos, article text or archive records.
- Never put credentials, personal information or private material in a file, a
  commit or an AI prompt.

## Quality checks

- Use semantic HTML and one `h1` per page.
- Every interactive element works with a keyboard and has a visible focus style.
- Text has enough contrast against its background.
- Pages work on a narrow phone screen without sideways scrolling.

## Whoever uses an assistant is the developer

Read every change before you keep it. Be able to explain it, test it and change
it. If you cannot, ask for a simpler version or leave it out.
