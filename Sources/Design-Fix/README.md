# Design Fix

## Overview

This category has been renamed from *Feet Fix*, because there are still a lot of other glyph quality problems in the mainline Source Han Sans/Noto Sans CJK font, for which my fixes from [All Traditional](../All-Traditional/README.md) can be put here, so basically now it contains a lot more design fixes (other than feet removal) that can potentially work for the mainline font, in other words, it is now a more generalised bug fix repository. The rename also enables Source Han Serif/Noto Serif CJK fixes to be put here in the future.

This category contains any "UD (Universal Design)"-style fixes that could potentially improve glyph quality in the typeface. However, Adobe does not see this as a high-priority issue, hence why this repository exists.

Besides fixing the feet issue in some components, it also hosts fixes of outline bugs (strokes poking out unexpectedly; while v2.005 fixes a good amount of glyphs, there are still a lot of them), and also proportion adjustments of existing characters, which could potentially work across different locales (while prioritising JP-style design); with one adjusted glyph, it can save some glyph space if it is to be implemented in the mainline font.

It may also host JP-style redesigns of existing characters which are not part of the Adobe-Japan1 character set (for which the [Missing JP glyphs](../Missing-JP-Glyphs/README.md) repository will cover that), as they are intended to replace the CN glyphs (and to a lesser extent Iwata-designed extended JP glyphs) which are poorly designed, and the glyph shapes can potentially qualify for the mainline font. However, the redesigns may not suit some people especially if they prefer the CN designs.

The locales follow that of Source Han Sans (with KR, CN, TW and HK having a dot suffix, while JP doesn't), so if there are any glyphs with custom orthography, the fixes would already have been applied anyway. Besides the suffix in the glyph names, the glyph list table will indicate the AI0-SourceHanSans glyph name my fixes are intended to replace.

### Guideline for whether feet should be included in components

For any "feet" in 口, 山 and similar components (let's say A) placed on top, if there is any component at the bottom, the feet may be removed (or only the right side, depending on where it’s placed). If the B component is on the right side, while A is on the left, and the strokes of B can get in the way of A, only the right feet may be removed in A.

## List of glyphs available

- [Sans](glyphlist-design-fix-sans.md)

## Changelog

- [Sans](changelog-design-fix-sans.md)

## PDF Preview

A visual representation of the glyph edits is available in PDF format, in ExtraLight, Regular and Heavy weights.

- [Sans](Sans/Preview/)
