# St Helens Rovers Football Club

The club website: a home page covering who we are, our teams, our history,
links to fixtures and league tables, the latest news, and how to get in touch,
plus a separate news page.

You do not need to know how to build websites to keep it up to date. Changing
the site means typing over the words in a file, the same way you would edit a
document. Nothing to install, and no way to break it that a quick undo will not
fix.

## Making changes

Double-click `index.html` to open it in your browser; that is what visitors
see. Open the same file in any text editor (TextEdit, Notepad, or the free
[VS Code](https://code.visualstudio.com/)) to change it.

Search the file for `EDIT ME` and you will land on each part meant to be
changed. Those notes never show up on the page.

| What you want to change          | File         | Search for                       |
| -------------------------------- | ------------ | -------------------------------- |
| Club name and tagline           | `index.html` | `EDIT ME: club name`             |
| About the club                   | `index.html` | `EDIT ME: about the club`        |
| Teams                            | `index.html` | `EDIT ME: your teams`            |
| History                          | `index.html` | `EDIT ME: club history`          |
| Fixtures and tables links        | `index.html` | `EDIT ME: fixture and table`     |
| Latest news headlines            | `index.html` | `EDIT ME: the three newest`      |
| Contact details                  | `index.html` | `EDIT ME: contact details`       |
| News stories                     | `news.html`  | `EDIT ME: news stories`          |
| Club colours, fonts, spacing     | `styles.css` | the block at the top             |
| Crest                            | `assets/crest.svg` |                            |

Change the words between the tags, not the tags themselves. To add another
team, history milestone, or link, copy one whole block from `<li>` to `</li>`,
paste it below, and edit the copy.

### Adding a news story

1. In `news.html`, copy a whole `<article>` block and paste it at the top of
   the list, so the newest story comes first.
2. Give it a new `id` (for example `id="derby-day"`), and update the date and
   the `aria-labelledby` and title `id` to match.
3. In `index.html`, update the "Latest news" list so its three headlines point
   at the newest stories, for example `news.html#derby-day`.

### Fixtures and tables

Each link in "Fixtures & tables" currently points at the FA Full-Time home
page. Find each team's own page on [FA Full-Time](https://fulltime.thefa.com/)
(or your league's website), copy its address, and paste it in place of
`https://fulltime.thefa.com/` for that team.

### The crest

`assets/crest.svg` is a simple placeholder shield. To use the real crest, put
the image in the `assets` folder and change `assets/crest.svg` in both
`index.html` and `news.html` to the new file's name.

## Publishing

Drag this folder onto [app.netlify.com/drop](https://app.netlify.com/drop), or
push changes to the connected repository, and the site updates.

## What's in here

```
index.html      the home page: about, teams, history, fixtures, contact
news.html       the news page
styles.css      how it looks: colours, fonts, spacing
script.js       the light/dark switch and the copy-link button
assets/         the club crest
favicon.svg     the small icon in the browser tab
```
