# Old Traditional

### Note: As of September 2025, this folder as it is has been deprecated.

*Although the original aim of this folder will continue, there are bigger priorities to change CN glyphs for commonly used characters to JP-style and to make modern orthographies for Traditional Chinese while keeping elements of Kangxi-style (or JP-style) printed forms. In other words, there will be new naming for this folder and almost all of the glyphs inside, as they will be sorted into new different folders as appropriate. They will not be removed from the repository, only organised, with the exception of a few minor “bugfix” glyphs, because Adobe has since fixed them in the main source for Sans v2.005.*

*Therefore, this part of the orthography may instead be called Retro Phototype Traditional once organisation is complete.*

### Overview

This category consists of Chinese characters as they appeared in the 1970s and 1980s during the phototypesetting era, particularly in Taiwan and Hong Kong.

They are called by several names including **traditional orthography**, **old forms**, **old character shape** (Simplified Chinese: 旧字形; Traditional Chinese: 舊字形), **inherited glyphs** (Simplified Chinese: 传承字形; Traditional Chinese: 傳承字形), **kyūjitai** (Japanese: 旧字体/舊字體) and so on.

As everybody knows, the glyph shapes are derived from the Japanese and Korean versions of Source Han Sans and Serif (or Noto Sans/Serif CJK), unlike the official Chinese versions which follow their respective handwritten government orthography (Chinese: 楷化, 新字形).

Right now, they mostly contain glyphs that I'm 100% sure will never make it into the main Adobe/Google fonts due to their glyph policy.

### Glyph policy

Regarding Inherited Glyphs, I believe it was created to standardise on the many different old forms throughout Chinese history. This will not be the main scope here as the plan is to recreate the forms seen in 1970s and 1980s newspapers and other media, which may not be deemed correct in the Inherited Glyphs standard. Regardless, many glyphs can be useful for the project.

### Restoring v1 JP glyphs

Because Adobe is not giving the project some love recently with the exception of a few external requirements deemed bare minimum, I have manually re-created and released most of the v1 JP sources (Sans only for now) to make them work with variable fonts.

For Sans, the sources cover GB 2312, Tongyong, iiCore, Big5 (both L1 and L2), HKSCS and Suppchara, with the exception of some characters that were already "restored" (like 95% close to the original v1 JP sources) in the Chiukong Gothic font.

The restored sources may not be 100% accurate to the original v1 JP source, and some of the characters are also improved upon by fixing outline bugs or improving proportions, as noted in the glyph lists.

For Serif, the v1 JP glyphs covering Big5 Level 1 will be restored and released in the future. However, Chiukong Mincho is also expected to be released in the near future, so not much work will be done here as Sans is currently of priority. I might, however, consider improving any glyphs being done on the other project.

### Chiukong Gothic

Some glyphs are taken from [Chiukong Gothic](https://github.com/ChiuMing-Neko/ChiuKongGothic), and some of those imported glyphs are improved on to make them more JP-like. They will be noted in the glyph lists below.

### Chiron Hei/Sung HK

Some glyphs are also taken from [Chiron Hei HK](https://github.com/chiron-fonts/chiron-hei-hk-gf) and [Chiron Sung HK](https://github.com/chiron-fonts/chiron-sung-hk-gf), because of the author's efforts to beautify some Chinese glyphs and adopt some JP forms for aesthetic use. However, the font series is intended to emulate glyph shapes similar to Monotype HK, therefore still falling under modern handwriting standards (although not the official educational forms). Because of this, any glyphs used are modified to old-traditional forms.

### Future updates in Source Han Sans

Regarding a potential major update to Source Han Sans in the future, it is possible that some JP forms as seen in v2 (e.g. 立, 豆, 子, 戶, 人, 夕, etc.) might be unified to the CN forms. If such a scenario happens, the sources will retain the v2 JP-style aesthetics rather than adopt the new unified forms.

## Glyph naming

To avoid confusion, the production names of the glyphs do not follow what is in the [AI0-SourceHanSans](https://github.com/adobe-fonts/source-han-sans/blob/release/Resources/AI0-SourceHanSans) or [AI0-SourceHanSerif](https://github.com/adobe-fonts/source-han-serif/blob/release/Resources/AI0-SourceHanSerif) files.

Here are a list of glyph suffixes. Taiwan will be the default glyph shape, so generally there is no suffix. The suffixes are also prepended by a period rather than dashes.

- uniXXXX<span>.</span>JP - Japanese glyph shape (according to their interpretation of the so-called Kangxi Dictionary forms)
- uniXXXX<span>.</span>HK - Hong Kong glyph shape
- uniXXXX<span>.</span>HK2 - Alternate Hong Kong glyph shape
- uniXXXX<span>.</span>inherited - Glyph shapes that follow the [Inherited Glyph standard](https://github.com/ichitenfont/inheritedglyphs) and may not appear in old prints.
- uniXXXX<span>.</span>altpr - Alternate print form (Unicode example, 卽 as an alternate print form for 即) which is also commonplace in some old typefaces.
- uniXXXX<span>.</span>noaxe - (Serif only) An alternate form which does not include the decorative axe in strokes like 乀. Inherited Glyphs adopts this standard by default, but in old media, this is less commonly seen.

## List of glyphs available

- [Sans](glyphlist-old-traditional-sans.md)
- [Serif](glyphlist-old-traditional-serif.md)

## Changelog

- [Sans](changelog-old-traditional-sans.md)
- [Serif](changelog-old-traditional-serif.md)

## PDF Preview

A visual representation of the glyph edits is available in PDF format, in ExtraLight, Regular and Heavy weights.

- [Sans](Sans/Preview)
- [Serif](Serif/Preview)