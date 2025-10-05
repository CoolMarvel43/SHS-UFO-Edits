# V1 Revival

## Overview

This category has been spun off from Old Traditional, which I felt is very difficult to maintain, plus changing priorities. It will primarily focus on restoring v1 JP glyphs that were removed in v2 of Source Han Sans/Serif, and if KR, CN and TW glyphs are to be included in the far future, I might consider adding a dot suffix (but the JP locale will not have a dot suffix by default).

Because Adobe does not believe that releasing every single unprocessed and overlapped sources of every single CJK glyph ever done by their own type foundry, Iwata, Changzhou Sinotype, and others, including those that did not make it into their main fonts, is in their primary interests (plus it’s complicated to compile their raw sources which can only work with their proprietary tools (like Adobe’s Type Work Bench 2) into something useable with common tools), I have manually re-created and released most of the v1 JP sources to make them work with variable fonts.

The vast majority of the restored JP sources can be used for Chinese locales (and some of them can be used for fonts that follow Simplified Chinese conventions), with some exceptions (which will be colour tagged in <span style="color:red">**red**</span>), because the forms are either completely alien to Chinese users, or they are not fully compliant with common conventions.

For Sans, the sources cover GB 2312, Tongyong, iiCore, Big5 (both L1 and L2), HKSCS and Suppchara.

The restored sources may not be 100% accurate to the original v1 JP source, and some of the characters are also improved upon by fixing outline bugs or improving proportions, as noted in the glyph lists.

For Serif, the v1 JP glyphs covering Big5 Level 1 and the jf7000 character set (base only) will be restored and released in the future. For now only a tiny amount of glyphs are available.

## List of glyphs available

- [Sans](glyphlist-v1-revival-sans.md)
- [Serif](glyphlist-v1-revival-serif.md)

## PDF Preview

A visual representation of the glyph edits is available in PDF format, in ExtraLight, Regular and Heavy weights.

- [Sans](Sans/Preview/)
- [Serif](Serif/Preview/)

Some glyphs are colour coded (which are also indicated in the source files). For more information, see the glyph list. But roughly:

<span style="color:red">**Red**</span> - Unsuitable for any Chinese locales, whether classic or modern forms. Those forms were originally made for the Japanese locale, for their own use (if they use the full 65535-glyph OTF version and pick any kanji outside the Adobe-Japan1-7 character set).
<span style="color:magenta">**Magenta**</span> - Borrowed glyphs from other Source Han forks without any modifications whatsoever. There is no guarantee that any future updates from them will be synced to this repository.

