Wikitable tXpx
--------------
Named based on class="wikitable tXpx" in new mediawiki syntax (supported themes only ie. this one), wikitable tXpx starts with all tables broken apart but allows them to "grow" when the screen extends beyond a certain pixel width.

No horizontal scrolling is required.

The same link is used for both the mobile and desktop version of a wiki (different from wikipedia).

Syntax and Example
------------------
The X in tXpx stands for the desired screen width, beyond which the table will "grow" into an html table.

"Grow" support includes all vertical and horizontal resolutions listed at:

[https://en.wikipedia.org/wiki/Display_resolution](https://en.wikipedia.org/wiki/Display_resolution)

The data-x attributes need to be added manually to tables, which is more wordy than normal wiki syntax but increases readability when creating wiki tables in a text editor. Notice aTtRiBuTe1 is matched to the corresponding value on the same line below (no vertical scrolling required):

```
{| class="wikitable t480px"
! aTtRiBuTe1
! aTtRiBuTe2
|-
| data-x="aTtRiBuTe1" | vAluE1
| data-x="aTtRiBuTe2" | vAluE2
|-
| data-x="aTtRiBuTe1" | vAluE3
| data-x="aTtRiBuTe2" | vAluE4
|}
```

Install
-------
Works by piggybacking off of the Vector skin (not yet standalone).
```
cd skins/
git clone https://github.com/vaskoiii/wikitable-txpx.git
vi ../LocalSettings.php
 - wfLoadSkin('Vector');
 + $wgDefaultSkin = "vector";
 + wfLoadSkin('wikitable-txpx');
```
