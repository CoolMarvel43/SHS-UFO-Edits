# Missing JP glyphs

## Overview

_While this description is mainly about Source Han Sans, the same can be said for Source Han Serif._

Source Han Sans, being a pan-CJK font, fulfils an objective for a seemingly consistent sans-serif font with different glyph shapes for different locales.

However, it comes with an aesthetic cost: Some of the Adobe-Japan1 glyphs look ugly.

This is because of several reasons:
* The CN glyphs are the only glyphs for the JP and KR locales. The problem is that the design of some of the CN glyphs, initially done by Changzhou Sinotype, is drastically different to that of the JP glyphs and Kozuka Gothic. The CN glyphs were also, according to a person formerly involved in the main project, done in haste, therefore their quality is relatively poorer.
* The official orthography of the Chinese regions (China, Taiwan and Hong Kong) follow that of the regular script (Simplified Chinese: 楷书; Traditional Chinese: 楷書), which is basically handwriting orthography.
* Several design differences (e.g. 立, 豆, 子, 戶, 人, 金, 夕, etc.) are considered regional differences. Some people feel that these are unnecessary as other similar commercial Chinese typefaces adopt JP-style designs (especially the 人 and 金 components) without a problem.
* And because of these, a lot of similar-looking JP glyphs (both within and outside of Adobe-Japan1) are sacrificed in favour of CN-style design when having to squeeze as many characters as possible within the 65,535 glyph limit.

This repository intends to “restore” the original Japanese design aesthetics of Source Han Sans, by recreating what they could have looked like. With these glyphs, uncompromised by CN-style design, the design for the Japanese, Korean and old Traditional Chinese locales are better harmonised and unified.

It will be periodically updated with new glyphs, focusing on the commonly-used characters in Chinese and Japanese, although some rare characters can appear as well.

_Serif is coming soon._

## List of glyphs available

- [Sans](glyphlist-missing-jp-sans.md)

## Changelog

- [Sans](changelog-missing-jp-sans.md)

## PDF Preview

A visual representation of the glyph edits is available in PDF format, in ExtraLight, Regular and Heavy weights.

- [Sans](Sans/Preview/)

***

**Note:** If Adobe releases their unreleased JP sources in the far future, this repository will be deleted.
