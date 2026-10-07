# The Increased Severance Clock

A sign of bulb digits, after the National Debt Clock that went up in New York in 1989. The top number is the
total of the wins, and it keeps ticking between them. Add a win and the clock counts up to the new total.

**Open it:** https://minitru.github.io/severance-clock/

## Dan: how to run your clock

The clock reads its wins from a Google Sheet. You never edit your website again after step 3: a new win is a new
row in the sheet.

### 1. Get the sheet

The clock is already reading a sheet called **Severance Clock wins**. Ask Sean to share it with you as an
editor, and you are done with this step. It has three columns:

| Date | Amount | Note |
| --- | --- | --- |
| 2026-10-06 | 90000 | whatever helps you remember |

- **Date** is the day of the win, written like `2026-10-06` or `10/6/2026`.
- **Amount** can be `90000`, `$90,000.00` or `90k`.
- **Note** is for you. It shows in the list on the clock's own page, never on the sign.

Would you rather own the sheet? Make a Google Sheet with those three headings, press **Share**, set General
access to **Anyone with the link** as **Viewer**, copy the link, and paste it into **Google Sheet of wins** on
the clock. Then carry on from step 2.

**The sheet is public to anyone who has its link.** Put no names or details in it that you would not publish.

### 2. Set the sign up once

Open the clock and use the settings under the sign:

- **Top line, line beside the second number, bottom line:** the three lines of lettering. Wrap words in
  `<i>…</i>` for italics or `<b>…</b>` for bold.
- **Starting at:** what you had won before the first row in the sheet. The rows add onto it.
- **Increment rate, per week:** how fast the top number ticks between wins. `20k` to start; `0` stops it.
- **The second number shows:** the latest win, how many wins, the average, or a number you type.

These settings are remembered in your browser, and they travel inside the embed code in step 3.

### 3. Put it on your Squarespace site, once

1. On the clock, press **Copy embed code**.
2. In Squarespace, edit the page, add a block, and choose **Code**.
3. Paste, leave the type as HTML, and save.

The sign takes the width of its column. Squarespace offers the Code block on its paid plans above the entry
one. If you later change the lettering, the starting amount or the rate, copy the embed code again and replace
the old one; a new win never needs that.

### 4. When you win

Add a row to the sheet. Within a minute every copy of the sign counts up to the new total and the latest
recovery blinks: on the clock's page, on your site, and on any link you have sent. No reload, nothing to paste.

Made a mistake? Fix or delete the row. The sign follows.

### What the top number means

It is the recorded total (the starting amount plus the rows) plus an estimate: the weekly rate times the time
since the last win. When you add the next win, the sign **trues up** to the recorded total and starts ticking
again from there. If the estimate had run ahead of the real figure, the sign comes down to it. The clock's own
page always says, under the list, what is recorded and how far ahead the sign is running.

### Sharing it elsewhere

- **Copy a link to this sign** gives a link that opens the sign alone, read-only, and stays up to date.
- **Show only the sign** hides everything else, for a screen on the wall.
- LinkedIn and most social posts cannot embed a live page. Post the link, or a short screen recording.

### A LinkedIn banner

**Download a LinkedIn banner** saves a picture of the sign as it is right now, 1584 by 396, the size LinkedIn asks
for a profile background. On LinkedIn: open your profile, press the camera on the background, and upload the
picture. The sign sits to the right in the picture, because LinkedIn puts your photo over the lower left.

It is a still picture. LinkedIn does not play animation in a background, so the number in the banner is the number
on the day you saved it; save a new one after a win.

## Without a sheet

Clear the **Google Sheet of wins** field and the clock goes back to wins typed into **Latest win**. Those live
only in the browser that typed them, so a copied link or embed code is then a snapshot of the sign as it stood,
and has to be copied again after each win.

## How it is made

One file, `index.html`. No libraries, no server, no tracking. Settings are kept in the browser (localStorage).
The sheet is read as CSV, once when the page opens and once a minute after; it is never written to.
`embed-example.html` shows the sign inside an ordinary page.

The dollar bills behind the lettering are public-domain photographs of a United States one-dollar bill, front
and back, from Wikimedia Commons, loaded from there when the page opens.

## Licence

MIT. See [LICENSE](LICENSE). The dollar-bill photographs are public domain and are not part of this repository.
