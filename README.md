# Source Han Sans/Serif UFO Edits

## About
This is a quick-and-dirty repository to store my edits to [Source Han Sans](https://github.com/adobe-fonts/source-han-sans) and [Serif](https://github.com/adobe-fonts/source-han-serif) (思源黑體/思源宋體). For now, they are only provided in UFO and glyphspackage formats, the former for which can be read by most font editors and the latter specifically for [Glyphs for Mac](https://glyphsapp.com/). The sources are overlapped, which is suitable for variable fonts, and available in two masters, ExtraLight and Heavy.

For convenience purposes, the OTF and TTF file formats will be provided, with all weights provided, overlaps removed and no hinting, but will only contain modified glyphs. They are not full fonts so they are unsuitable as to be used as standalone fonts. Feel free to integrate them into your forks as you please. As of September 2025, only the Missing JP sources have those formats, and eventually they will be provided for other orthography formats.

This repository is divided into folder categories of orthography formats, followed by typeface style. For now, there is only the traditional orthography format (Simplified Chinese: 旧字形/传承字形; Traditional Chinese: 舊字形/傳承字形), the JP glyphs missing from the main font and some Japanese kana edits available. More orthography formats will follow in the near future.

Further plans may include (but production and release date undetermined):
- Modern TC forms (but not adopting handwritten forms like LiHei Pro and the Chiron HK series). There will be two versions:
	- A version that preserves some traditional orthography forms (like the 示 and 羽 components), similar to the unfinished Taipei Sans TC beta and some old commercial fonts. Glyph reference will roughly follow that of LXGW XiHei MN.
	- A version that is mostly based on the glyph shapes of IBM Plex Sans TC and v2 of the TW version of ButTaiwan's Gen fonts (which has since been separated into classic TC and modern TW versions). It aims to satisfy the needs of people who are much more used to the handwritten forms of modern Chinese fonts. The designs will match the Adobe-designed JP glyphs rather than use the CN-style designs of Changzhou SinoType.
- CN-style orthography for Japanese kanji (up to Adobe-Japan1-3 coverage), which may be similar to Kyōkasho forms that are seen in commercial Japanese fonts that are intended for the educational market (but will not follow those forms).
- JP-style orthography for Simplified Chinese hanzi while closely following Mainland Chinese glyph standards.
- A CSV file containing remaps to CIDs and to point to modified glyphs for each orthography folder. This can be one step closer to producing a full Source Han Sans derivative with customised remapped and modified glyphs.

Regarding the versions, since 2025, my edits are based on Source Han Sans v2.005 and Source Han Serif v2.003. If a new version is released, any glyphs added from that version will be noted down as such.

The sources will be updated with new glyphs and adjustments periodically. They will be noted in their respective changelogs.

## Regarding the ridiculous names

The naming of the source files will temporarily be called "WIPSHDC" (an unoriginal acronym I have to make up), followed by the category (like "Kana" or "Old-Traditional" as mentioned above), and then either "Sans" or "Serif" as the suffix. A better name will be decided in the near future.

## Quick weight setup

These tables are provided as reference to recreate the intermediate weights in the font editor of your choosing.

### Sans

Weight Name | Weight Value
-- | --
ExtraLight | 0
Light | 160
Normal | 320
Regular | 390
Medium | 560
Bold | 780
Heavy | 1000

### Serif

Weight Name | Weight Value
-- | --
ExtraLight | 0
Light | 95
Regular | 210
Medium | 360
SemiBold | 510
Bold | 730
Heavy | 1000

## Licence

As always, the sources are licensed under the SIL Open Font License.

## Special Thanks to:
* ChiuMing-Neko for the [ChiuKong Gothic project (秋空黑體)](https://github.com/ChiuMing-Neko/ChiuKongGothic).
* NightFurySL2001 for providing some support.
* ButTaiwan for [GenYoGothic (源樣黑體)](https://github.com/ButTaiwan/genyog-font), for which I recreated the き and さ kana designs to work with variable format.
* Tamcy for providing the sources to the [Chiron HK](https://github.com/chiron-fonts/chiron-hei-hk-gf) [font series](https://github.com/chiron-fonts/chiron-sung-hk-gf) for Google Fonts.
* Ichitenfont for the [Inherited Glyph reference](https://github.com/ichitenfont/inheritedglyphs).
* GuiWonder for his project to quickly create an alternate traditional orthography for Source Han Sans/Serif under the name [Shanggu](https://github.com/GuiWonder/Shanggu). My plan is to improve the quality of their glyphs.