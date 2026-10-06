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
- **Change the words** by clicking them on the sign: the title, the label beside the second number, and the
  name at the bottom.
- **The second number** can be the latest win, how many wins, the average win, or a number you type.
- **Show only the sign** hides everything else, for a screen on the wall.
- **Copy a link to this sign** gives a link that shows the sign as it is now, read-only, to anyone.
- **Copy embed code** gives an `<iframe>` snippet that puts the sign, and nothing else, on another web page.
  Like the link, it is the sign as it was when copied: it keeps ticking at the rate, but a new win needs a new
  copy, because the wins live in the browser that entered them.

One file, `index.html`. No libraries, no server, no tracking. The wins are kept in the browser that entered
them (localStorage); a copied link carries its numbers and words in the link itself.

The dollar bills behind the lettering are public-domain photographs of a United States one-dollar bill, front
and back, from Wikimedia Commons, loaded from there when the page opens.
