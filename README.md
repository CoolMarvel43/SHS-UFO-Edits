# Source Han Sans/Serif UFO Edits

## About
This is a quick-and-dirty repository to store my edits to [Source Han Sans](https://github.com/adobe-fonts/source-han-sans) and [Serif](https://github.com/adobe-fonts/source-han-serif) (思源黑體/思源宋體). They are provided in UFO and glyphspackage formats, the former for which can be read by most font editors and the latter specifically for [Glyphs for Mac](https://glyphsapp.com/). The sources are overlapped, which is suitable for variable fonts, and available in two masters, ExtraLight and Heavy.

In addition, for convenience purposes, the OTF and TTF file formats will be provided, with all weights provided, overlaps removed and no hinting, but will only contain modified glyphs. They are not full fonts so they are unsuitable as to be used as standalone fonts. Feel free to integrate them into your forks as you please. You will need to use a font editor to access the unencoded glyphs (those appended with a dot suffix like ".MN", ".CL1", ".inherited", etc.).

Unfortunately to do so, the sources will now include two additional characters which I do not include in their glyph lists: .notdef and space (taken straight from Source Han Sans/Serif). This is required for Adobe-Identity-0 to work correctly when exporting OTF and TTF file formats, so please ignore these two characters if you work with the source files.

This repository is divided into folder categories of orthography formats, followed by typeface style.

Further plans may include (but production and release date undetermined):
- Expansion of old traditional Classic forms to fully cover most common Traditional Chinese character lists. This will continue in 2025 and beyond.
- Modern TC forms (but not adopting handwritten forms like LiHei Pro and the Chiron HK series). There will be two versions:
	- A version that preserves some traditional orthography forms (like the 示 and 羽 components), similar to the unfinished Taipei Sans TC beta and some old commercial fonts. Glyph reference will roughly follow that of LXGW XiHei MN.
	- A version that is mostly based on the glyph shapes of IBM Plex Sans TC and v2 of the TW version of ButTaiwan's Gen fonts (which has since been separated into classic TC and modern TW versions). It aims to satisfy the needs of people who are much more used to the handwritten forms of modern Chinese fonts. The designs aim to match the Adobe-designed JP glyphs rather than use the CN-style designs of Changzhou SinoType wherever possible.
- CN-style orthography for Japanese kanji (up to Adobe-Japan1-3 coverage), which aims to look similar to Kyōkasho forms that are seen in commercial Japanese fonts that are intended for the educational market (but will not follow those forms).
- An alternate JP-style orthography for Simplified Chinese hanzi while closely following Mainland Chinese glyph standards.
	- For example, the first stroke in 宀 is a vertical stroke, similar to JP forms, not a drop according to handwritten 新字形 rules. However, 纟 will follow forms similar to commercial fonts like LiHei Pro (seen in the 糹 radical), and the first stroke of some components, like 言 and 户 (except for 所), will have a vertical stroke.
- A CSV file containing remaps to CIDs and to point to modified glyphs for each orthography folder. This can be one step closer to producing a full Source Han Sans derivative with customised remapped and modified glyphs. Some code points are taken from different orthography folders, and will be noted as such.

Regarding the versions, since 2025, my edits are based on Source Han Sans v2.005 and Source Han Serif v2.003. If a new version is released, any glyphs added from that version will be noted down as such.

The sources will be updated with new glyphs and adjustments periodically. They will be noted in their respective changelogs.

## Regarding the font name

The naming of the source files will temporarily be called "WIPSHDC" (an unoriginal acronym I have to make up), followed by the category (like "Kana" or "All-Traditional" as mentioned above), and then either "Sans" or "Serif" as the suffix. A better name will be decided in the near future.

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

## Issues

Any design problems or suggestions, or any ideas to improve the presentation or organisation of this repository, you can do so [here](https://github.com/CoolMarvel43/SHS-UFO-Edits/issues).

## Special Thanks to:
* ChiuMing-Neko for the [ChiuKong Gothic project (秋空黑體)](https://github.com/ChiuMing-Neko/ChiuKongGothic).
* NightFurySL2001 for providing some support.
* ButTaiwan for [GenYoGothic (源樣黑體)](https://github.com/ButTaiwan/genyog-font), for which I recreated the き and さ kana designs to work with variable format.
* Tamcy for providing the sources to the [Chiron HK](https://github.com/chiron-fonts/chiron-hei-hk-gf) [font series](https://github.com/chiron-fonts/chiron-sung-hk-gf) for Google Fonts.
* Ichitenfont for the [Inherited Glyph reference](https://github.com/ichitenfont/inheritedglyphs).
* GuiWonder for his project to quickly create an alternate traditional orthography for Source Han Sans/Serif under the name [Shanggu](https://github.com/GuiWonder/Shanggu). My plan is to improve the quality of their glyphs.