Wikitable tXpx
--------------
Wikis should be mobile first and then "grow" elegantly to support larger screens in terms of virtual pixels while optimizing screen space and preserving data.

Named based on class="wikitable tXpx" in new mediawiki syntax (supported themes only ie. this one), wikitable tXpx allows tables to "grow" once beyond a threshold resolution.

Consequently the same link is used for both mobile and desktop wikis (different from wikipedia)

Syntax and Example
------------------
The X in tXpx stands for the desired resolution width, beyond which the table will "grow" into an html table.

"Grow" support includes all vertical and horizontal resolutions listed at:

[https://en.wikipedia.org/wiki/Display_resolution](https://en.wikipedia.org/wiki/Display_resolution)

The data-x attributes need to be added manually to tables, which is more wordy than normal wiki syntax but increases readability when creating wiki tables in a text editor (especially with tables that have a lot of columns).

```
{| class="wikitable t480px"
! aTtRiBuTe1
! aTtRiBuTe2
|-
| data-x="aTtRiBuTe1" | vAluE1
| data-x="aTtRiBuTe2" | vAluE2
|-
| data-x="aTtRiBuTe3" | vAluE3
| data-x="aTtRiBuTe4" | vAluE4
|}
```
