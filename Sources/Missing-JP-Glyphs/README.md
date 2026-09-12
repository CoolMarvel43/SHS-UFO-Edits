# Missing JP glyphs

## Overview

_While this description is mainly about Source Han Sans, the same can be said for Source Han Serif._

Source Han Sans, being a pan-CJK font, fulfils an objective for a seemingly consistent sans-serif font with different glyph shapes for different locales.

However, it comes with an aesthetic cost: Some of the Adobe-Japan1 Han glyphs look ugly.

This is because of several reasons:
* The CN glyphs are the only glyphs for the JP and KR locales. The problem is that the design of some of the CN glyphs, initially done by Changzhou Sinotype, is drastically different to that of the JP glyphs and Kozuka Gothic (or Kozuka Mincho for Serif). The CN glyphs were also, according to a person formerly involved in the main project, done in haste, therefore their quality is relatively poorer.
  * The CN design by Changzhou Sinotype (and Arphic) and JP design by Adobe (and Iwata) can look quite different in terms of component proportions, counter (中宮) and visual gravity (重心), and even in the curvature of some drop strokes (CN favours stiffer strokes like Founder’s Lantinghei, while JP favours curvier strokes). The participation of more than one type foundry, which inevitably leads to slightly different design decisions for each foundry, causes some visual inconsistency of the overall design of CJK ideographs, when comparing between characters with similar radicals and components.
  * While there was a reason for the CN glyphs being chosen over the JP glyphs (likely the CN glyphs are better for small size reading), it appears that the Adobe team had either not thoroughly checked the CN glyphs for stroke shape quality and consistency, or did not have enough time doing it. 
* The official orthography of the Chinese regions (China, Taiwan and Hong Kong) follow that of the regular script (Simplified Chinese: 楷书; Traditional Chinese: 楷書), which is basically handwriting orthography (also known as 新字形).
* Several minor design differences (e.g. 立, 豆, 子, 戶, 人, 金, 夕, etc.) are considered regional differences. Some people feel that these are unnecessary as other similar commercial Chinese typefaces adopt JP-style designs (especially the 人 and 金 components) without a problem.
* And because of these, a lot of similar-looking JP glyphs (both within and outside of Adobe-Japan1) are sacrificed in favour of CN-style 新字形 design when having to squeeze as many characters as possible within the 65,535 glyph limit.

There will be a blog post detailing the discrepancies between CN and JP design. It is coming soon.

This repository intends to "restore" the original Japanese design aesthetics of Source Han Sans and reduce the influence of CN-style 新字形 design, by recreating what the glyphs could have looked like if more JP glyphs were chosen instead. With that, the design for the Japanese, Korean (if Hanja is used alongside Hangul) and Traditional Chinese locales (not following official educational orthography) could be better harmonised and unified, without compromise.

It will be periodically updated with new glyphs, focusing on the commonly-used characters in Chinese and Japanese, although some rare characters can appear as well.

_Serif will follow after the most important characters in Sans are covered, probably in 2027-2028._

## List of glyphs available

- [Sans](glyphlist-missing-jp-sans.md)

## Changelog

- [Sans](changelog-missing-jp-sans.md)

## PDF Preview

A visual representation of the glyph edits is available in PDF format, in ExtraLight, Regular and Heavy weights.

- [Sans](Sans/Preview/)

***

**Note:** If Adobe releases their unreleased JP sources in the far future, this repository may be trimmed to keep just a few glyphs that is deemed unique.