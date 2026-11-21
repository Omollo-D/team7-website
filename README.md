# Team Name:

**Live site:**https://omollo-d.github.io/team7-website/

## Team

| Name           | Registration no. | GitHub username |
| -------------- | ---------------- | --------------- |
| David Ambanya  | COM/3487/26      | Omollo-D        |
| Sheilah Kerubo | COM/34 /26       | Shixkerry       |

## Who drove each part

- Part 0, 2, 4: David Ambanya
- Part 1, 3: Sheilah Kerubo

## Personalisation

- Our colours:
  Light: --color-primary: #1d4ed8;
  Light dark: --color-primary-dark: #1e3a8a;
  Dark: --color-primary: #38bdf8;
  Dark dark: --color-primary-dark: #bae6fd;

- Projects we added:
  We added two projects to script.js: a Git version-control project and a JavaScript contact-form validation project. Added the git category label and matching Git filter button in projects.html. The category and filter values match, so the existing filter logic can display the Git project.

- Extension challenge(s) completed:
  We created faq.html section with atleast 4 quizzes and save message input value

## Reflection

1. Our menu toggle is a `<button>`, so people can reach it with the keyboard and activate it with Enter or Space. A clickable `<div>` would not have those button features or announce itself as a button by default, which would make the menu harder to use for keyboard users and people using screen readers.

2. We use `defer` so the browser can keep parsing the page and run our script after the HTML is ready. Without it, the script in the `<head>` could run before the browser reaches the body, so things like the menu, theme button, or contact form might not exist yet when the script looks for them.

3. Our projects are displayed with `textContent`, which treats each title as plain text. If we used `innerHTML` for titles typed by visitors, someone could enter HTML or script-like markup that the browser might interpret instead of just showing as text.

4. Our JavaScript checks the form to help visitors fix mistakes, but it runs in their browser and could be turned off or bypassed. Once the form sends data to a server, the server must check it too because it cannot assume the browser-side checks were used.

5. Our theme choice is saved in `localStorage`, which is associated with the page's origin (its scheme, host, and port). Home and Contact on the same site share an origin, but opening a file with `file:` and using Live Server with `http:` are different origins, so the browser keeps their saved theme choices separate.

6. We copied the same header and navigation into each of our HTML pages. If we add or rename a link, we have to remember to update every page, or the menus could stop matching; a template or shared component could keep the header in one place.
