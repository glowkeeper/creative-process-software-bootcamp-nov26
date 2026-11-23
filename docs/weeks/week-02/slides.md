---
marp: true
paginate: true
footer: Week 2
---

# Software Development Bootcamp

## Week 2

Creating the Interface

Dr Steve Huckle

steve@huckle.studio

---

# Today, your project becomes visible

- Learn the jobs of HTML and CSS
- Build a static Short Film Programme Builder together
- Create one interface for your prototype
- Explain the structure and styling you chose

---

# Two applications still have different jobs

```text
Short Film Programme Builder
Shared example we build together

Your prototype
Your response to one brief or your own agreed idea
```

---

<!-- _class: recap section-slide -->

# Review

## Where your project stands after Week 1

---

# Week 1 established your project's direction

```text
You decided                    You created
brief and intended visitor     repository and README
Starting Point                 Project board and first issues
```

## Today, turn that direction into a visible interface

---

<!-- _class: mentimeter-slide -->

# What have you decided to create during the bootcamp?

## Mentimeter Activity

---

<!-- _class: mentimeter-slide -->

# What would you change first?

## Mentimeter Activity

---

<!-- _class: big-idea -->

# Big Idea

## Create something people can see and use

---

# A web interface has two foundations

```text
HTML                         CSS
structure and meaning   +    presentation

              = interface
```

---

# HTML describes the content

```html
<article>
  <h2>The Quiet Cartographer</h2>
  <p>A mapmaker records disappearing paths...</p>
</article>
```

- Elements are written with tags
- Nesting expresses relationships
- Semantic elements communicate meaning

---

<!-- _class: mentimeter-slide -->

# Where is the `<article>`?

## Mentimeter Activity

---

# Attributes add information

```html
<section aria-labelledby="films-heading">
  <h2 id="films-heading">Choose from six films</h2>
</section>
```

```text
attribute name="attribute value"
```

---

# CSS selects HTML and changes its presentation

```css
.film-card {
  padding: 1rem;
  background-color: white;
}
```

```text
selector        property     value
.film-card      padding      1rem
```

---

# CSS has three simple ways to select HTML

```css
button { }          /* every button element */

.film-card { }      /* reusable class */

#films-heading { }  /* one unique ID */
```

---

# Spacing happens around the content

```text
+----------------------+
|        margin        |
|  +----------------+  |
|  |     border     |  |
|  |  +----------+  |  |
|  |  | padding  |  |  |
|  |  | content  |  |  |
|  |  +----------+  |  |
|  +----------------+  |
+----------------------+
```

---

<!-- _class: section-slide -->

# Guided Build

## Short Film Programme Builder

---

# Part 1 · Meet the scaffold

```text
starter/
├── index.html
└── styles/
    └── style.css
```

1. Open `index.html` in VS Code
2. Open it in the browser
3. Edit, save and refresh

---

# The document already has foundations

```html
<!doctype html>
<html lang="en">
<head>
  <meta charset="utf-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <title>Short Film Programme Builder</title>
</head>
<body>

</body>
</html>
```

---

# Part 2 · Structure the page

```html
<body>
  <header></header>

  <main>
    <section></section>
  </main>

  <footer></footer>
</body>
```

---

# Part 3 · Introduce the programme

```html
<header class="site-header">
  <p class="eyebrow">Creative Processes Cinema</p>
  <h1>Short Film Programme Builder</h1>
  <p>Explore six fictional films and imagine a programme...</p>
</header>
```

---

# Give the collection a purpose

```html
<section aria-labelledby="films-heading">
  <div class="section-heading">
    <div>
      <p class="eyebrow">Stage 1 archive</p>
      <h2 id="films-heading">Choose from six short films</h2>
    </div>
    <p>Target running time: 30-45 minutes</p>
  </div>
</section>
```

---

# Part 4 · Build one film card

```html
<article class="film-card">
  <p class="film-meta">Documentary · Ireland · 2023</p>
  <h3>The Quiet Cartographer</h3>
  <p>A mapmaker records disappearing paths along a changing coastline.</p>
  <button type="button">Add to programme</button>
</article>
```

---

# Part 5 · Create the collection

One card pattern + different content = a collection

```text
The Quiet Cartographer     Borrowed Weather
Soft Machines              A Song for the Underpass
Tuesday's Orbit            Salt Library
```

## All six cards are prepared, so we can move on to styling

---

# Part 6 · Connect the stylesheet

```html
<link rel="stylesheet" href="styles/style.css">
```

```text
HTML asks the browser to load the CSS file
```

---

# Give repeated decisions a name

```css
:root {
  --background: #f1eee8;
  --surface: #fffdf8;
  --text: #20201d;
  --muted: #66635d;
  --border: #d8d2c8;
  --accent: #b33a2f;
}
```

---

# Establish the page before styling details

```css
* { box-sizing: border-box; }

body {
  margin: 0;
  font-family: Arial, sans-serif;
  line-height: 1.5;
  color: var(--text);
  background-color: var(--background);
}
```

---

# Control width and spacing once

```css
.site-header,
main,
footer {
  width: min(1100px, calc(100% - 2rem));
  margin: 0 auto;
}
```

---

# Part 7 · Style the film card

```css
.film-card {
  min-height: 300px;
  padding: 1.25rem;
  border: 1px solid var(--border);
  border-radius: 0.5rem;
  background-color: var(--surface);
}
```

---

# Interfaces should respond visibly

```css
.film-card button:hover {
  background-color: var(--accent-dark);
}

.film-card button:focus-visible {
  outline: 3px solid var(--text);
  outline-offset: 3px;
}
```

---

# Part 8 · Arrange repeated items with Grid

```css
.film-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
  gap: 1rem;
}
```

---

# Test the narrow layout

```css
@media (max-width: 650px) {
  .section-heading {
    align-items: flex-start;
    flex-direction: column;
  }
}
```

Resize the browser and inspect what changes.

---

# Part 9 · Review what we built

- meaningful HTML structure
- element, class and ID selectors
- CSS properties and values
- content, padding, border and margin
- a responsive collection
- visible hover and keyboard focus

---

# Complete is today's successful outcome

- Six fictional films
- Clear hierarchy
- Responsive card layout
- Consistent visual system
- Buttons that are visible but do not work yet

---

# Showcase changes the visual direction

It still uses only HTML and CSS.

- Stronger art direction
- CSS-only abstract film artwork
- Runtime labels
- Empty programme summary
- Additional responsive polish

---

<!-- _class: section-slide -->

# Developer Studio

## Build one interface for your prototype

---

# Keep the Starting Point narrow

Choose the single most important view or moment:

- What must the visitor understand first?
- What content pattern repeats?
- Which HTML describes that content honestly?
- Which visual choices support its purpose?

The full fictional film archive is in the cohort repository if you want more
than six films. Copy only the records your interface needs.

---

# Your Week 2 minimum outcome

- One meaningful `index.html`
- One linked external stylesheet
- Clear structure and hierarchy
- A reusable class where appropriate
- A layout that works when narrow
- Fictional, self-created, placeholder or permitted assets only
- A clear Git commit

---

# Start with an issue

```text
Issue      Why, and a Done when checklist
Context    AGENTS.md says how to work here
Plan       read it before any code is written
Change     one small step
Check      run it, test it, read what changed
Commit     name the issue, move the card
```

## With AI or without, the issue is your plan

---

# Working well with AI

- Say what you are building, and for whom
- Share the smallest relevant code and the exact problem
- Ask for a plan before code
- Ask for one small change at a time
- Read the change before you accept it
- Run it and test it in the browser
- Commit when it works

---

# Working well without AI

The same habits apply:

- Break the problem down
- Read the error message properly
- Inspect the page with Developer Tools
- Check the documentation and your notes
- Change one thing at a time
- Ask a person: the tutor, the support assistant, a peer

---

# AI is often wrong, and sounds sure

It can:

- Misread your Starting Point
- Invent properties and attributes
- Add layout you did not ask for
- Ignore accessibility
- Make the page more complicated than it needs to be

Check with the browser, Developer Tools and the documentation.

---

# Check before you keep it

1. Can I read it?
2. What does each line do?
3. Does it fit my Starting Point, or expand it?
4. Have I run it?
5. Could I change it, or remove it?

---

<!-- _class: reflection section-slide -->

# Reflection

## Look back at today

---

<!-- _class: mentimeter-slide -->

# Where is the `<article>`?

## Mentimeter Activity

---

# What you imagined and what we built

```text
This morning: What would you change first?
Today:        What did we actually change?
```

## Which of your ideas became part of the page?

---

<!-- _class: mentimeter-slide -->

# What can a visitor understand from your interface?

## Mentimeter Activity

---

# Week 3 asks the next question

## How can the page respond when somebody uses it?

```text
Week 2: visible structure and presentation
Week 3: behaviour and interaction
```

---

# Week 2 complete

## You turned a planned Starting Point into a visible interface

- HTML gave the content structure and meaning
- CSS gave it hierarchy, layout and presentation
- Your visitor can now understand what the interface is for

---

# Thank you

Dr Steve Huckle

steve@huckle.studio
