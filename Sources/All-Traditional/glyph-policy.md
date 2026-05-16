# Glyph Policy

The source files will strictly follow Source Separation Rule to avoid confusion, but CL forms will be the default encoded form.

In this document, any mention of locales like JP/KR/CN/TW/HK refer to the vanilla Source Han Sans/Serif (or Noto Sans/Serif CJK) font. Also, this document assumes that there will eventually be a production of final font files with custom mappings and edits.

The documentation is translated and modified from [this link](https://github.com/lxgw/LxgwXiHei/blob/main/documentation/plan.md), so credit to LXGW for creating the document.

## CL forms (Classic)
This is basically the historical forms of Chinese characters used throughout 20th century, from hot metal typesetting to phototypesetting machines. It largely follows the Kangxi Dictionary forms, but made to be more unified. Nonetheless, glyph variations are allowed as there are more than one acceptable form of some components, ideally enabled via OpenType SS or CV variants.

The JP and KR locales have largely preserved these forms. However, some characters can look a bit different from what Traditional Chinese people expect because in Japan's case, they would record with variations that are not standardised, and that those characters which are common in Chinese are not really used in the Japanese/Korean locales, hence why the Unicode J and K sources recorded their sources as they were and did not even adjust their glyphs because preserving the strokes as they were originally recorded is more important than consistency. Even with variant glyphs available, Adobe-Japan1 does not record all the historical classic forms.

There are community-led efforts to expand the forms to be better optimised for Traditional Chinese without any anomalies brought about by Japanese standards. This project's UFO edits is one of them.

Several codepoints will be unified for the sake of component consistency and historical accuracy, therefore it will not respect Source Separation Rule. It should roughly follow LXGW CL forms, with some exceptions.

Unlike existing SHS forks which understandably attempt to unify all characters whenever possible, for this project, any Simplified Chinese characters will ***not*** be subjected to this policy, with the following exceptions:
- Those under the Big5/HKSCS/Adobe-CNS1/Adobe-Japan1 character sets
- 辶 radical (will unify to ⻍ regardless of character)
- Any character that historically existed as old forms (even if partially) during the 新字形 transition period in China

They will instead use orthography as defined in [New Simplified](/../../tree/main/Sources/New-Simplified).

#### Components that will NOT be unified
- 晉／晋
	- Latter will be picked for Simplified characters
- 強／强
	- Latter will be picked for Simplified characters, otherwise any character variant will be put under CL1; used in HK phototypesetting
- 奐／奂
	- Latter will be picked for Simplified characters
- 爭／争
	- Latter will be picked for Simplified/Shinjitai characters (except for those under JIS90/04 changes)
- 吳／吴／呉
	- First one is preferred for non-separated characters
- 兗／兖
	- Former is preferred for non-separated characters
- 袞／衮
	- Former is preferred for non-separated characters
- 毀／毁
	- Former is preferred for non-separated characters
- 剎／刹, 弒／弑
	- Former is preferred for characters with this component
	- 杀 (U+6740) itself will remain unchanged *(deviation from LXGW CL)*
- 眾／衆
- 查／査
	- Former is preferred for non-separated characters
	- The latter form will be under "JP/Inherited" naming and may be available under an OpenType feature

#### Components that will be unified
- 戶／户／戸 will pick 戶
- 兌／兑 will pick 兌
- 內／内 will pick 內
- 黃／黄 will pick 黃
- 別／别 will pick 別
- 呂／吕 will pick 呂
- 麼／麽 will pick 麼
- 朮／术 will pick 朮 (except for the singular characters themselves)
- 禿／秃 will pick 禿
- 冊／册 will pick 冊
- 虛／虚 will pick 虛
- 彔／录 will pick 彔 (except for the singular characters themselves)
- 敻／夐 will pick 夐 *(deviation from LXGW CL)*
- 𥁕／昷 will pick 𥁕
- 產／産 will pick 產, same with 彥／彦
- 奧／奥 will pick 奧, same with 粵／粤
- 勻／匀 will pick 勻 (last stroke is an angled stroke, not horizontal like Inherited Glyph/TW forms)
- Between 遙/瑤/搖/謠 and 遥/瑶/摇/謡, the 䍃 component will pick the former form
- 為／爲 will pick 爲
- 俞／兪 will pick 兪
- 尚／尙 will pick 尙
- 真／眞 will pick 眞
- 青／靑 will pick 靑
- 即／卽 will pick 卽
- 既／旣 will pick 旣
- 教／敎 will pick 敎
- 告／吿 will pick 吿
- 并／幷 will pick 幷
- 郎／郞 will pick 郞
- 鄉／鄕／郷 will pick 鄕
- ⻟／⻞ will pick ⻞
	- Source Separation Rule characters 飲／飮 will be unified to the latter
- 者／者 will pick 者
	- Source Separation Rule characters 緒／緖 will be unified to the latter
- 直／直 will pick 直 (bottom-left L shape as seen in JP forms)
	- Source Separation Rule characters 值／値 will be unified to the latter
- 𦣞／𦣝 will pick 𦣝
	- Source Separation Rule characters 熙／煕 will be unified to the latter
- 单／単 will pick 单 (example: 禅, 蝉)
	- Any non-unified characters will remain as they are
	- As this is a simplified character component, New Simplified takes priority over JP forms as the simplified characters (barring being part of Big5/HKSCS) will not be subject to CL rules.
- 带／帯 will pick 带 (e.g. 滞)
	- Any non-unified characters will remain as they are
	- As this is a simplified character component, New Simplified takes priority over JP forms as the simplified characters (barring being part of Big5/HKSCS) will not be subject to CL rules.
- 戋／㦮 will pick 㦮 (e.g. 浅, 残)
	- Any non-unified characters will remain as they are (栈／桟)
	- Despite being a simplified character component, JP forms take priority over New Simplified.

#### Stroke Policy
- 匚 and 匸 will be unified to 匚
	- 匸 (TW form) is available under MN3 or inherited forms
	- The JP variant glyph of 匸 (e.g. uni5340uE0101-JP 區) that is not the TW form may be available under CL2 as an OpenType feature.
- Moon 月 and Meat ⺼ will be unified to 月
	- Boat 舟月 will still be distinguished, e.g. 朝, 潮
	- There is zero distinction between near-homoglyphs like 朏 (U+670F) and 胐 (U+80D0)
- 艹 and ⻀ will be unified to 艹 *(deviation from LXGW CL)*
- 形 follows 开 while 研 follows 幵 due to different etymology
- The middle of the 𧶠 component that is found in characters like 讀, 續 follows 四 instead of 罒
- The 㐄 component in 韋, 舛, 夅, etc. will follow JP/KR forms *(deviation from LXGW CL)*
- The top part of the 旡 component will stick out in 朁 (except for 蠶), otherwise any components with 旡 will not.
	- However, unlike the 㐄 component in 韋, 舛, 夅, the second folding stroke of 旡 will follow modern forms (e.g. the JIS2004 form of 牙).
- The characters 暗, 章, 帝, 商, 意, 龍, 親, etc. will have a vertical first stroke on 亠, not horizontal (as with Inherited Glyphs). Same with 良 (except for 食 and its corresponding left radical, which will be 亼)
	- Horizontal stroke versions will be marked under CL1. There will be an OpenType feature to enable these forms.
		- 辛, 旁, 妾 and 毅 will be marked under inherited instead, as even under classic metal type and HK phototypesetting, they have a vertical stroke. Therefore doing these forms will be of much lower priority.
- The first top stroke of the 丰 component will be a horizontal stroke (if placed on left or right on its own)
- The inner part of 害, 憲 and 砉 will be 丰, and the first stroke is bending
	- MN1 and MN2 forms are also subject to this
	- The 丯 variant will be under CL1 and is available as an OpenType feature
	- This 丰 form is more prevalent in old metal type, and it is baffling when GenKiGothic has the 丯 form for TC.
- The middle component of 契 will be 丯 and the vertical stroke is slanted like this backslash: \
- The first stroke of 邦 is horizontal, and the third is angled.
	- CL1 has a variant where the first stroke is bent, and the third is angled (similar to the JP variant glyph uni90A6uE0102-JP), and may be available as an OpenType feature.
- The inner part of 周 will use 𰀁 (or キ with not-slanted strokes, or ⧧)
- 呈, 聽, 鐵 and 望 will use 𡈼
- The middle horizontal stroke in ⺕, which is part of 刍 (e.g. 急, 煞) will cross
	- However, characters like 邹 and 趋, which are the simplified forms of the 芻 component, do not apply.
	- Also 隐 because it is not part of any Traditional Chinese character set.
	- MN forms are also subject to this
- The top of 关 is 八 (applies to 朕, 送, 掷 etc.)
	- However, it does not apply to characters like 联 and 渕 because they were simplified from/related to the 𢇇 and 𣶒 components respectively.
		- The top right of 咲 will use 八 because despite it being a variant of 㗛 (which means the rule should normally not apply), it widely existed in old prints
	- 关 will remain as it is (although redesigned to JP-style)
- When used as a standalone character, the top of 兼 will use 八
- The bottom of the component that contains 遷 and 僊 is ⺋, not 巳
	- MN forms are also subject to this
- 欠, 尔 will have the strokes connected.
- The top part of 臽 will have a hook, but not the 負 and 危 components.
- The top part of 忝 is 夭, middle stroke is longest.
- 亡 will be 匚 instead of 匸 (as seen in Japanese hyōgaiji forms) *(deviation from GenKiGothic TC)*
	- Although 匸 is more commonly seen in old type, but applied inconsistently. May be available under OpenType.
- The middle horizontal stroke of 冉 will stick out
- The inner part of 成 will use 丁 (following 成 U+2F8B2)
- The right part of 化 will cross (similar to KR/CN forms)
- 才 will follow JP form (except when placed on the right side)
- The bending stroke of 丩 will cross (similar to JP forms)
- 覆, 覈 will use 襾, otherwise no distinction between 覀 and 襾
- The top of 垔 is 西
	- MN forms are also subject to this
- The 爫 component will be ⺥
	- However, 乎, 受 and 愛 are not subject to this
		- And then again, 受 and 愛 using ⺥ might be placed under "inherited" naming and may be available as an OpenType feature
- The bottom of 冬, 寒 will be 冫 (KR form)
- The bottom right part of 於 follows ⺀ (JP form)
	- MN forms are also subject to this
- The inner part of 勺 will be 一
- 卻 and 郤 will be 谷, not 𧮫 (deviation from LXGW CL)
	- The 𧮫 variant may be available under an OpenType feature
- The bottom of 聚, 衆 is 乑, except for 眾
- The bottom right 𧘇 part of 旅, 派 is㇙ (KR form)
	- MN forms are also subject to this
- The left side of 釉 is 釆, not 采
- The centre-top part of 璺, 釁 and 爨 will be 𠮛
	- Deviation from LXGW CL which uses ⿱一コ
- The bottom of 蔑 and 篾 is 戍
	- MN forms are also subject to this
- The top of 曼, 最 and 𦐇 will be 日
	- MN1 and MN2 forms are also subject to this
	- The ⺜ variant will be under Inherited and will have an OpenType feature.
- 臾 will use 𦥑, but 裒, 舁 will use 臼
	- Deviation from LXGW CL
- The top of 函 is 丂
- The right of 虧 is 亐
- When used on its own or placed at the bottom, the bottom right part of 瓦 is ㇈, but when placed on the right, it is ⺄
- In the top right part of 延, the last stroke is ㇄
- The top right part of 将 uses the traditional form as seen in 將 (following U+2F873 将)
	- Same with 奨 and 醤 (if time permits; they're Japanese characters)
	- However, 奖 and 酱 remain as they are and will follow New Simplified orthography
- The top part of 蚩 is 䶹
- 佾 and 潸 is 月
	- MN forms are also subject to this, so a deviation from LXGW MN
- The phonetic components 攸, 敄 (such as 條, 務 respectively), will be 攵, not 夂
	- MN forms are also subject to this
	- 条 and 务 can be 攵 because the former is a Japanese Shinjitai character (for which 木 will be used) and both are part of HKSCS
- The right part of the 巩 component is ⿹㇈𠂇 (e.g. 筑, 鞏)
	- There are two variants of 巩. ⿹㇈𠂇 is horizontal stroke version seen in some, but not all old typefaces. The others show the JP/CN form of the 巩 component instead (which will be in the MN version of the font)
	- ⿹㇈乂 is the Taiwan variant. There is very little evidence of that historically appearing, other than that form appearing in 銎 in ZhaohuaMinB. May have to assign this to MN3 instead.
- The outer part of 巨 is 工
- The last stroke of 外 is a throw stroke (similar to JP forms)
- The right 和 part of 啝 is ⿰禾口 (similar to CN form) (deviation from LXGW CL)
	- MN forms are also subject to this
	- The JP ⿺禾口 form is less commonly seen, so it may be available as an OpenType feature
- The top part of 𬙙 is 罒
	- MN forms are also subject to this
	- The 四 form is under inherited and is available as an OpenType feature
	- Deviation from LXGW CL
- The bottom part of 毒 is 毋 (following JP forms where the last stroke does not stick out)
- The 㕣 component is ⿱八口; 兗 and 袞 will also be ⿱八口
- 𤰇 in 備 is ⿱艹⿸厂用, similar to JP forms
- The bottom left part of 戎 is 𠂇, horizontal stroke is an angled stroke
	- Except for 賊, which will be 十 instead
- The bottom part of 类 is 犬 (because it is part of Adobe-Japan1)
- The inner part of 壳 will have a horizontal stroke, inclusive of the base character (because it is part of Adobe-Japan1)
- The inner component of 奐 is 儿, similar to JP forms
- 令 will follow JP forms
- 豕, 冢, 蒙, 豪, 家, 㒸, etc. will follow JP forms
- The bottom-left part of 睘 and 袁 will not have a folding stroke if another component is below it, similar to JP/KR forms. If they are placed left or right, they will still have a folding stroke, similar to KR forms.
- 旃, 栴 will follow JP forms (bottom right is 円 with the horizontal stroke crossing the 冂)
- The inner top part of 風 has a bending stroke (similar to JP/CN forms)
	- MN1 and MN2 forms are also subject to this
- The bottom right of 保 is 木 (similar to JP/CN forms)
	- MN1 and MN2 forms are also subject to this
- 幾 will follow JP forms (within Jōyō kanji), but the bottom part is not 戍 (as with Hyōgaiji forms).
	- MN forms are also subject to this
- Within the left side of 卽／旣 and similar characters, the bottom left 匕 part (as seen in KR forms) will be the default encoded form (or CL1 if multiple variants exist), as per GenKiGothic TC (丹). The variant that resembles the bottom part of ⻞ (different character used to illustrate this easily) will be marked under CL2, despite it also being common and the default form for Inherited Glyphs.
	- There will be an OpenType feature that will enable users to switch to the latter form if needed.
	- This policy is a deviation from LXGW CL and is not mentioned in the original document.
- There will be decorative axe strokes in Serif, e.g. 乂义更文斉齐廴史吏父交爻丈叉
	- And then due to time constraints it may not be applicable to 又支鼓攴
- The 八 component will have the folding throw stroke 乁 on the top.
	- MN forms are also subject to this
- 主 will have a drop stroke at the top
	- Sources will use drop stroke as default encoded form
	- The version with the vertical stroke at the top was actually more common in Chinese phototypesetting fonts (and due to the influence of Kyūjitai/Hyōgaiji kanji forms from Japan), apparently this is deemed incorrect. Some earlier metal type used the drop stroke though.
	- Will enable vertical stroke variant via OpenType under CL1 (if there are no JP glyphs for characters with the 主 component)

There are also some fundamental design changes, which applies to all orthographies.
- Most CN/TW/HK glyphs, even if they technically can be used as they are, will be redesigned to use JP shapes and proportions (preferably taking from similar characters within Adobe-Japan1, which is done by Adobe. Any JP glyph outside this character set are done by Iwata instead, and may not have the same quality that Adobe has). I explain this in further detail, *post is coming soon*.
- For Sans, 立 (and similar characters with this component) has been tweaked in such a way the third bending stroke does not touch the bottom horizontal stroke, which is similar to Kozuka Gothic where this vanilla open-source typeface is based on. While the current JP form is acceptable and arguably preferred, many JP glyphs with similar components (e.g. 䒑, 豆, etc.) do not adopt such forms, probably due to time constraint. Thus the change was made to 立 for more consistency and bringing back what I believe could be the initial JP design.
	- Same with 辛 and 首
- 吳 will have the bottom 大 part connected, and the left feet in the 𠃑 stroke removed, due to UD (Universal Design) principles. Some glyphs are in the [Feet Fix](/../../tree/main/Sources/Feet-Fix) repository.
	- CL forms may or may not retain the JP Kyūjitai form where the bottom 大 part is not connected. MN forms, however, must have the part connected.

Suffix naming (if final font files are to be released in the future): TC-CL

## MN forms (Modern)
Intended for the 21st century, taking into account the presence of commercial typefaces that cater to handwriting standards and government efforts to standardise glyph shapes.

It is also intended for computer input methods where glyph ambiguity (due to CL unification) may not be allowed due to academic and technical reasons.

It will strictly follow Source Separation Rule.

MN1 will be the main documentation; any glyph policy defined under MN2 and MN3 will override that of MN1.

### Modern Forms 1 (MN1)
MN1 is considered the most traditional of the modern forms, taking into account the prevalence of Japanese typefaces (mistakenly) used in Greater China and historical commercial typefaces that retain elements of the Kangxi Dictionary forms like the 羽 and 示 radicals.

#### Example fonts that roughly follow these forms
- Founder Lantinghei TC
- LXGW XiHei/ZhiSong MN
- Taipei Sans TC Beta (unfinished)

#### Stroke Policy
- Moon 月, Meat ⺼ and Boat 舟月 will be unified to 月
	- Due to strict Source Separation rule, there will be a distinction between glyphs like 朏 (U+670F) and 胐 (U+80D0).
		- 胐 (U+670F) will force the Inherited 月 form, while 胐 (U+80D0) will use the standard 月 form.
- 屯 and 鬲 will retain JP/CL forms *(deviation from LXGW MN)*
- 全 will retain the top 入 component
- 艹 and ⻀ will remain unified to 艹 *(following LXGW MN)*
- 形 and 研 are unified to 开
	- Source Separation Rule characters remain as they are
- The middle of the 𧶠 component that is found in characters like 讀, 續 follows 罒 instead of 四
- The 㐄 component in 韋, 舛, 夅, etc. will still follow JP/KR forms (as with CL forms)
- The top of the 旡 component will not stick out under any circumstance
- 食 will retain 亼 and 飠 will follow TW/HK forms, which is ⿱亼⿸𢀳丶 *(deviation from LXGW MN)*
	- If CN-style conventions are to be considered in the future, there may be an OpenType feature (or a separate MN version) to include the Japanese Shinjitai form of 飠 (as with Chiukong Gothic MN), and even Arphic's AR HeiB5 BD (文鼎粗黑) adopt this form. However, majority of the commercial fonts follow TW/HK forms.
- The first top stroke of the 丰 component will be a bending stroke (if placed on left or right on its own)
- As with CL, the inner part of 害, 憲 and 砉 will be 丰, and the first stroke is bending
	- Deviation from LXGW MN, as the vertical stroke sticks out, but may or may not touch other components depending on circumstances
- The top left part of 契 is 丰, with the first stroke being horizontal
- The first stroke of 邦 is bent, and the next two strokes are horizontal (similar to TW forms)
- The inner part of 周 will use 土
- 聽, 鐵 will use 王, while 呈, 聖 and 望 will use 𡈼
- The top right of 望 will use 𱼀, which is uni671BuE0102-JP in Source Han Sans/Serif
- 关, 酋, 兼, 益, etc. will use 丷
- The top part of 臽 will not have a hook
- The top part of 忝 is 天, middle stroke is longest
- 亡 will be 匸 instead of 匚 (similar to JP Shinjitai/KR forms)
- The middle horizontal stroke of 冉 will not stick out
- The inner part of 成 will use ㇆ (similar to CN form)
- The right part of 化 will not cross (similar to JP form)
- 才 will follow CN form
- The bending stroke of 丩 will not cross
- There is no distinction between 覀 and 襾, however, as with CL forms, the top of 垔 is 西
- The 爫 component remains unchanged
- The bottom of 冬, 寒 will be ⺀
- The inner part of 勺 will be 丶
- The left part of 卻 and 郤 is 谷
- The bottom of 聚, 衆／眾 will be 𫡑
- The left side of 釉 will remain as 釆, not 采
- The centre-top part of 璺, 釁 and 爨 will remain 𠮛
- 臾, 裒 and 舁 will use 臼
- The top of 函 will remain as 丂
- The right of 虧 is 亏
- In the top right part of 延, the bottom part is 止 (similar to JP/TW forms)
- The top right part of 将 uses the Japanese Shinjitai form (爫)
	- Same with 奨 and 醤 (they're Japanese characters)
	- As with CL, 奖 and 酱 remain as they are and will follow New Simplified orthography
- The top part of 蚩 is 屮
- The right part of the 巩 component is 凡 (e.g. 筑, 鞏)
- The last stroke of 外 is a drop stroke (similar to TW form)
- The bottom part of 毒 is 母 (except for 纛)
- The last stroke of 毋 will stick out
- 㕣 is ⿱ㄦ口
	- Except for 柗, as it is a variant of 松
- 兗, 袞 is ⿱ハ口
- 𤰇 in 備 is ⿸𦫺用, where the horizontal stroke in 厂 crosses over, but does not follow CN forms. In fact it is closer to the JP form.
- The bottom left part of 戎 is 𠂇, and the horizontal stroke remains as it is
- The bottom part of 类 is 大 (following New Simplified conventions)
- The inner part of 壳 does not have a horizontal stroke (following CN conventions)
- 奐 will retain JP/CL forms
- 令 will follow TW/HK forms *(deviation from LXGW MN)*
- 辶 will retain two dots (⻍)
- 羽, 弱, 示 (礻) will retain KR/CL forms.
- 欠, 尔 will have the strokes separated *(deviation from LXGW MN)*
- 豕, 冢, 蒙, 豪, 家, 㒸, etc. will follow CN/TW forms, but redesigned to JP-style as seen in the right part of 像 uni50CFuE0101-JP.
- The bottom-left part of 睘 and 袁 will have a folding 𠄌 stroke, even if there's another component below it, similar to TW/HK forms
- 旃, 栴 will follow CN forms (bottom right is 丹), but redesigned to JP-style
- There are no decorative axe strokes in Serif for components like 乂义更文斉齐廴史吏父交爻丈叉, however, the 八 component will retain the folding throw stroke 乁 on the top.

Suffix naming: TC-MN1

### Modern Forms 2 (MN2)
MN2 is intended as a compromise between handwritten forms and traditional orthography forms. This is suitable for anyone who are not used to classic forms and/or might deem them weird/incorrect.

#### Example fonts that roughly follow these forms
- 華康中黑體
- IBM Plex Sans TC
- GenKiGothic TW (月)

#### Stroke Policy Differences from MN1
- 艹 and ⻀ will be separated *(deviation from LXGW MN)*
- 屯 and 鬲 will follow CN/TW forms
- The inner component of 奐 will be 人 (similar to TW/HK forms)
- 羽, 弱, 示 (礻) will follow Japanese Shinjitai/TW/HK forms, with 示 (礻) using the design of Japanese Shinjitai forms.
- The centre-top part of 璺, 釁 and 爨 is 𬼽
- The top of 函 is 了
- The bottom part of 毒 is 毋 (and the middle bending stroke will stick out)
- The left side of 釉 is 采, not 釆
- The 㐄 component in 韋, 舛, 夅, etc. will follow modern forms in the same way as 牙 and 旡

Suffix naming: TC-MN2

### Modern Forms 3 (MN3)
MN3 has some elements of Taiwan's Standard Form of National Characters, also for which the Inherited variant (i.MingVar) also adopts. However, this orthography does not adopt the former's orthography wholesale. Consider this the closest to the Taiwan standard without introducing unwanted Kaiti elements that will break the beauty of the characters.

#### Example fonts that roughly follow these forms
- 華康粗黑體
- 華康新特黑體

#### Stroke Policy Differences from MN1
- The policy will largely follow MN2, with a few changes:
	- 寺, 感 will follow TW forms, but redesigned to JP-style.
	- 艹 will follow the split form (similar to TW/HK forms)
	- The inner top part of 風 has a horizontal stroke (similar to TW/HK/Inherited forms)
	- The bottom right of 保 is ホ (similar to TW/Inherited forms)
	- The top of 曼, 最 and 𦐇 will be ⺜
	- As with CL and MN forms, the inner part of 害, 憲 is 龶, and the first stroke is bending. But the vertical stroke does not cross the bottom horizontal stroke, similar to TW forms.
	- 𤰇 in 備 follows CN form
	- The right part of the 巩 component will be ⿹㇈乂 (following TW forms)
	- If placed on the left side, 屯, 己 and any other components with 乚 as the ending stroke will become 𠄌.

Suffix naming: TC-MN3

If there are any constructive disagreements with these policies I make, feel free to make an issue, and if possible, show evidence of the glyph shape being historically used.