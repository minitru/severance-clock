# The Increased Severance Clock

A sign of bulb digits, after the National Debt Clock that went up in New York in 1989. The big number is the
sum of the wins. Add a win ("90k", "90,000.00", "1.2m") and the clock counts up to the new total.

**Open it:** https://minitru.github.io/severance-clock/

- **Starting at** is what had been won before the clock; the wins you enter add onto it.
- **Add a win** ("Latest win") under the sign. A win can be removed again; the clock counts back down.
- **Between wins it keeps ticking, then trues up.** Set an increment rate per week (20k to start; 0 stops it). The top
  number is the recorded wins plus an estimate: the rate times the time since the last win. Entering the next
  win trues the sign up to the recorded total. The list under the sign is the record, and says how far ahead
  the sign is.
- **Change the words** in the settings: the top line, the line beside the second number, and the bottom line.
  `<i>…</i>` and `<b>…</b>` are allowed for italics and bold; nothing else is taken as HTML.
- **The second number** changes at once and blinks; it can be the latest win, how many wins, the average win, or a number you type.
- **Show only the sign** hides everything else, for a screen on the wall.
- **Copy a link to this sign** gives a link that shows the sign as it is now, read-only, to anyone.
- **Copy embed code** gives an `<iframe>` snippet that puts the sign, and nothing else, on another web page.

## Keeping it up to date: a Google Sheet

Typed-in wins live only in the browser that typed them, so a sign embedded on a website would be a snapshot.
Connect a Google Sheet and a new win is a new row; every copy of the sign, embedded ones too, follows within a
minute. The sheet is read, never written.

1. Make a Google Sheet with three columns: **Date**, **Amount**, **Note**. One row per win.
   Amounts can be `90000`, `$90,000.00` or `90k`.
2. In the sheet: **File → Share → Publish to web**, choose the sheet, publish, and copy the link.
3. On the clock, paste the link into **Google Sheet of wins**. The list fills from the sheet.
4. Set the three lines, **Starting at** and the **Increment rate** as you want them.
5. Press **Copy embed code** and paste it into the website once (below). After that, only the sheet changes.

Anyone with the published link can read the sheet, so put in it only what may be public. The Note column is
shown on the clock's own page, not on the sign.

## Putting it on a Squarespace page

Edit the page, add a block, choose **Code**, and paste the embed code with the type set to HTML. Squarespace
allows the Code block on its paid plans above the entry one. The sign takes the width of its column.

One file, `index.html`. No libraries, no server, no tracking. The wins are kept in the browser that entered
them (localStorage); a copied link carries its numbers and words in the link itself.

The dollar bills behind the lettering are public-domain photographs of a United States one-dollar bill, front
and back, from Wikimedia Commons, loaded from there when the page opens.

## Licence

MIT. See [LICENSE](LICENSE). The dollar-bill photographs are public domain and are not part of this repository.
