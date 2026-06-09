# Glossary Judge Report

## Summary

- Languages reviewed: 60
- Terms per language: 66 (F01–F07, R01–R08, A01–A04, T01–T06, G01–G16, C01–C14, TR01–TR11)
- **Total issues found: 73** (27 definite errors, 46 flags for review)
- Languages with < 40 terms populated: 9 (see section below)

The single most widespread defect is **T02 Morning being extracted as the word for "Warning"** in 22 languages. This is a systematic extraction tool bug: the extractor retrieved a UI alert/warning string instead of the time-of-day label. All affected languages have been corrected in their TSV files.

---

## Definite Errors

| lang | term_id | term | current (before fix) | issue | suggested_fix |
|---|---|---|---|---|---|
| tr | T02 | Morning | Uyarı | "Uyarı" means Warning/Alert in Turkish, not the time-of-day | Sabah |
| ru | T02 | Morning | Предупреждение | "Предупреждение" means Warning in Russian | Утро |
| uk | T02 | Morning | Попередження | "Попередження" means Warning in Ukrainian | Ранок |
| bg | T02 | Morning | Предупреждение | "Предупреждение" means Warning in Bulgarian | Утро |
| sr | T02 | Morning | Упозорење | "Упозорење" means Warning in Serbian | Јутро |
| sr@ijekavian | T02 | Morning | Упозорење | Same as sr | Јутро |
| sr@latin | T02 | Morning | Upozorenje | Same as sr, Latin script | Jutro |
| sr@ijekavianlatin | T02 | Morning | Upozorenje | Same as sr@latin | Jutro |
| sk | T02 | Morning | Varovanie | "Varovanie" means Warning in Slovak | Ráno |
| lt | T02 | Morning | Įspėjimas | "Įspėjimas" means Warning in Lithuanian | Rytas |
| lv | T02 | Morning | Brīdinājums | "Brīdinājums" means Warning in Latvian | Rīts |
| ko | T02 | Morning | 경고 | "경고" means Warning in Korean | 아침 |
| vi | T02 | Morning | Cảnh báo | "Cảnh báo" means Warning in Vietnamese | Buổi sáng |
| ca | T02 | Morning | Avís | "Avís" means Notice/Warning in Catalan | Matí |
| pt | T02 | Morning | Aviso | "Aviso" means Warning/Notice in Portuguese | Manhã |
| pt_BR | T02 | Morning | Atenção | "Atenção" means Attention/Warning in Brazilian Portuguese | Manhã |
| nl | T02 | Morning | Waarschuwing | "Waarschuwing" means Warning in Dutch | Ochtend |
| sv | T02 | Morning | Varning | "Varning" means Warning in Swedish | Morgon |
| nb_NO | T02 | Morning | Advarsel | "Advarsel" means Warning in Norwegian | Morgen |
| he | T02 | Morning | אזהרה | "אזהרה" means Warning in Hebrew | בוקר |
| is | T02 | Morning | Viðvörun: | "Viðvörun:" means Warning (with UI colon) in Icelandic | Morgunn |
| et | T02 | Morning | Hoiatus | "Hoiatus" means Warning in Estonian | Hommik |
| hr | T02 | Morning | Upozorenje | "Upozorenje" means Warning in Croatian | Jutro |
| sl | T02 | Morning | Opozorilo: | "Opozorilo:" means Warning (with UI colon) in Slovenian | Jutro |
| id | T02 | Morning | Peringatan | "Peringatan" means Warning in Indonesian | Pagi |
| eo | T02 | Morning | Averto | "Averto" means Warning in Esperanto | Mateno |
| zh_TW | T02 | Morning | 警告 | "警告" means Warning in Traditional Chinese | 上午 |
| ja | T02 | Morning | 警告 | "警告" means Warning in Japanese | 午前 |
| sr | F07 | Dunefolk | немртви | "немртви" means Undead — same as F03; wrong faction | (untranslated — needs research) |
| sr@ijekavian | F07 | Dunefolk | немртви | Same as sr | (untranslated — needs research) |
| sr@latin | F07 | Dunefolk | nemrtvi | Same as sr, Latin script | (untranslated — needs research) |
| sr@ijekavianlatin | F07 | Dunefolk | nemrtvi | Same as sr@latin | (untranslated — needs research) |
| ko | F07 | Dunefolk | 언데드 | "언데드" means Undead — same as F03; wrong faction | (untranslated — needs research) |
| sr | G05 | Income | Добро дошли | "Добро дошли" means Welcome; UI collision | (needs extraction from correct string) |
| sl | G05 | Income | Dobrodošli | "Dobrodošli" means Welcome; UI collision | (needs extraction) |
| et | G05 | Income | Tere tulemast | "Tere tulemast" means Welcome; UI collision | (needs extraction) |
| he | G05 | Income | ברוך הבא | "ברוך הבא" means Welcome; UI collision | (needs extraction) |
| id | G05 | Income | Selamat Datang | "Selamat Datang" means Welcome; UI collision | (needs extraction) |
| he | TR02 | Hills | הריגות | "הריגות" means Killings/Murders — severe extraction collision from battle results screen | גבעות |
| ro | F03 | Undead | Oameni | "Oameni" means People/Humans, not Undead | Morți-vii / Nemorți |
| ro | F07 | Dunefolk | Oameni | "Oameni" means People/Humans, not Dunefolk | (untranslated — needs research) |
| ro | R04 | Drake | Oameni | "Oameni" means People/Humans, not Drake | (untranslated — needs research) |
| ro | A01 | Lawful | Oameni | "Oameni" means People/Humans, not the Lawful alignment | (needs extraction) |
| ro | A03 | Chaotic | Oameni | "Oameni" means People/Humans, not the Chaotic alignment | (needs extraction) |
| ro | C12 | ambush | Oameni | "Oameni" means People/Humans, not the ambush ability | (needs extraction) |

---

## Flags for Review

| lang | term_id | term | current | concern | confidence |
|---|---|---|---|---|---|
| tr | F01 | Loyalists | Sadıklar | Two competing terms: "Sadıklar" (The Loyal Ones, abstract) and "Kralcılar" (Royalists, loyalty to the king). Both are defensible; "Kralcılar" may better convey crown-loyalty context | medium |
| tr | TR06 | Frozen | Kar (was) → Donmuş | "Kar" means Snow, not Frozen. Most languages use a frozen/iced word. Changed to "Donmuş"; original may be a locale adaptation | medium |
| tr | TR04 | Flat | Çayır (was) → Düzlük | "Çayır" means Meadow/Pasture, not generic flat terrain. Changed to "Düzlük"; original may be locale adaptation | medium |
| sr | G02 | Scenario | Крај | "Крај" means End — extracted from "End Scenario" button, not the concept name | low |
| sr@ijekavian | G02 | Scenario | Крај | Same issue | low |
| sr@latin | G02 | Scenario | Kraj | Same issue | low |
| sr@ijekavianlatin | G02 | Scenario | Kraj | Same issue | low |
| sr | TR02 | Hills | победе (was) → Брежуљци | "победе" means Victories — battle results screen collision | low |
| sr | G03 | Side | Страна | "Страна" can mean Page/Side in a book sense; verify it's used for game faction in Serbian | medium |
| da | G01 | Campaign | Smart udfoldning | Looks like a UI string ("Smart deployment?"), not the Campaign concept | low |
| da | G02 | Scenario | Afslut scenarie | "End scenario" button label, not the concept name | low |
| da | G03 | Side | Næste side | "Næste side" means Next side/page — navigation UI label | low |
| da | A04 | Liminal | loyal | Same word as A01 Lawful; Liminal is a distinct alignment (twilight bonus) | low |
| da | F07 | Dunefolk | Udøde | "Udøde" means Undead (same as F03 Udød — closely related). Likely an extraction collision | low |
| nl | T01 | Dawn | Ochtend | "Ochtend" means Morning; Dawn should be pre-sunrise twilight ("Dageraad"). T02 was set to "Ochtend" as the corrected Morning — the T01 label now needs review too. | medium |
| lv | F01 | Loyalists | Cilvēki | "Cilvēki" means Humans; race name used instead of faction concept | medium |
| lv | F02 | Rebels | Elfi | "Elfi" means Elves; race name used instead of faction concept | low |
| lv | F04 | Northerners | Orki | "Orki" means Orcs; race name used instead of faction concept | low |
| lv | F06 | Knalgan Alliance | Rūķi | "Rūķi" means Dwarves; race name used instead of full alliance name | low |
| cs | TR02 | Hills | Hory (was) → Kopce | Both Hills and Mountains resolved to "Hory" (Mountains); Hills changed to "Kopce" | medium |
| ko | G02 | Scenario | 시나리오 마치기 → 시나리오 | "End scenario" button label; stripped to concept word | medium |
| ko | G03 | Side | 다음 진영 → 진영 | "Next faction" UI label; stripped to concept word | medium |
| vi | G05 | Income | Thu nhập: | Trailing colon stripped; minor artifact | high |
| lv | G05 | Income | Ienākums: | Trailing colon stripped; minor artifact | high |
| et | F01 | Loyalists | Ustav | "Ustav" means Constitution/Charter in Estonian — not loyalty. May be an unusual localization of faction concept. Review needed. | low |
| ro | TR01 | Forest | Padure arctica | "Padure arctica" means Arctic Forest — a specific sub-type, not generic Forest | medium |
| ro | TR02 | Hills | sate | "sate" means villages/settlements in Romanian — not Hills terrain | low |
| ro | C07 | skirmisher | otravit | "otravit" means poisoned — same semantic field as C04 poison, not the skirmisher ability | low |
| ru | R04 | Drake | Зомби-дрейк | "Зомби-дрейк" means Zombie Drake — a specific unit name, not the Drake race in general | medium |
| bg | G01 | Campaign | addon_type^Кампания | Contains an internal markup prefix "addon_type^" — extraction artifact. Should be just "Кампания" | medium |
| bg | G02 | Scenario | Отдалечена мисия | "Отдалечена мисия" means Remote mission — a specific UI context, not the general Scenario concept | medium |
| bg | G03 | Side | Следваща страна | "Следваща страна" means Next side — navigation UI label | medium |
| he | G02 | Scenario | סיים התקלות | Appears to be "End encounters" — UI button label, not the concept name | medium |
| is | T02 | Morning | Viðvörun: (was) → Morgunn | Had trailing colon in addition to wrong meaning — doubly flagged as UI artifact | fixed |
| sl | T02 | Morning | Opozorilo: (was) → Jutro | Had trailing colon — UI artifact | fixed |
| eu | A01 | Lawful | Iheslaria | "Iheslaria" in Basque context seems unusual for Lawful; also used for A04 Liminal which is a different alignment | medium |
| eu | A04 | Liminal | Iheslaria | Same as A01 Lawful — two distinct alignments share one word | low |
| eu | C06 | berserk | Ikusleak | "Ikusleak" means Viewers/Spectators in Basque — unexpected for a combat ability | low |
| eu | C07 | skirmisher | Saurio gatazkaria | "Saurio gatazkaria" appears to be Drake/Saurian skirmisher (unit name), not the ability concept | low |
| eu | C10 | steadfast | Andretxarra | Same word as R04 Drake in Basque — potential extraction collision | low |
| eu | C12 | ambush | Sarekada | "Sarekada" means Network/Web — unusual for ambush ability | low |
| eu | C14 | concealment | Kanpamentua | "Kanpamentua" means Camp — not the concealment ability | low |
| sl | C14 | concealment | Tabor | "Tabor" means Camp/Encampment in Slovenian — not the concealment ability | low |
| af | C14 | concealment | Kamp | "Kamp" means Camp in Afrikaans — not the concealment ability | low |
| af | R04 | Drake | Uitvaagsel | "Uitvaagsel" means Scum/Riffraff in Afrikaans — pejorative term, not a race name. Likely extracted from a different context | low |
| tl | F03 | Undead | matapat | "matapat" means faithful/loyal in Tagalog — same as F01 Loyalists. Extraction collision | low |
| tl | F05 | Drakes | Mga Kabibi | "Mga Kabibi" means Shellfish/Clams — clearly an extraction error; Drakes are dragon-kin | low |

---

## Cross-Language Patterns

### T02 Morning Extraction Bug (22 languages affected)
The extraction tool matches the string "Morning" against .po file msgids, but in many language files a "Warning:" UI label appears in the same search context as the time-of-day Morning label. The extractor picked the Warning string in any language where "Warning" appears before "Morning" in the .po file ordering. Languages using time-of-day-named UI screens (e.g., German "Vormittag", French "Matin") were not affected.

The consistently correct set: de, fr, es, it, pl, hu, cs, zh_CN, ar, fi, da, af, id→fixed, eu, gl, tl, mk, el, ca_ES@valencia.
The affected set (all corrected): tr, ru, uk, bg, sr variants (×4), sk, lt, lv, ko, vi, ca, pt, pt_BR, nl, sv, nb_NO, he, is, et, hr, sl, id, eo, zh_TW, ja.

### "Income = Welcome" Extraction Collision (5 languages)
Several languages (sr, sl, et, he, id) resolved G05 Income to their word for "Welcome". This likely occurred because some .po files place the welcome screen string adjacent to income-related strings, or because the term "income" is rare and the extractor fell back to a nearby high-frequency string.

### Faction Names Using Race Names Instead (Latvian, some others)
Latvian uses race names (Humans, Elves, Orcs, Dwarves) for faction names F01–F04, F06. This is either a genuine localization choice (the Latvian PO uses race names to identify factions) or an extraction tool collision. Several other languages also use Undead for Dunefolk (sr, ko, da, af, he, eu) — this is always a collision, since Dunefolk are a desert-dwelling human faction distinct from Undead.

### "End Scenario" Button Label Extraction
Multiple languages extracted the "End Scenario" / "Finish Scenario" button label for G02 Scenario. Affected: sr/sr variants, ko, da, lt, bg, sl, et, he, id, eu, is, ca@valencia (partial), af, pt, vi, lv. The extractor should prioritize standalone concept strings over UI compound strings.

### Frozen Terrain: "Frozen" vs. "Snow" vs. "Ice"
Most languages render TR06 Frozen with a word meaning frozen/iced. Exceptions:
- tr: "Kar" (Snow) — changed to "Donmuş" (Frozen)
- et: "Lumi" (Snow) — retained (may be locale adaptation; Finnish uses "Jäätynyt" = frozen)
- gl: "Xeo" (Ice/Frost) — acceptable semantic equivalent
- ko: "얼음" (Ice) — acceptable
- zh_TW: "冰雪" (Ice-Snow) — acceptable
- hu: "Jégmező" (Ice Field) — specific but appropriate

### Flat Terrain: Generic vs. Specific
Most languages render TR04 Flat as plain/flatland. Exceptions:
- tr: "Çayır" (Meadow/Pasture) — changed to "Düzlük"
- gl: "Herbal" (Herb-land/pasture) — similar locale adaptation
- et: "Rohumaa" (Grassland) — close but specific
- uk: "Луг" (Meadow/Meadow land) — similar to tr original
- pt Flat: "Plano" (flat/plan) — acceptable

### Drake Race vs. Faction
Several languages use the same word for the Drake faction (F05) and the Drake race (R04), which is correct since the faction is named after the race. However, Russian R04 = "Зомби-дрейк" (Zombie Drake) is a specific unit name, not the race.

---

## Languages with Low Coverage (< 40 terms populated)

| lang | populated terms | notes |
|---|---|---|
| ro | ~18 | Severe quality issues; many entries are "Oameni" (Humans) regardless of concept. Entire file needs re-extraction or manual review. |
| mk | ~20 | Macedonian is sparse; many game-specific terms not found. Many entries missing. |
| hr | ~25 | Croatian has partial coverage; factions and many abilities missing. |
| af | ~35 | Afrikaans has gaps in Campaign, Income, Hex, ZoC, and several terrain types. Several quality issues. |
| tl | ~30 | Tagalog has significant gaps; major quality issues (Drakes=Shellfish, Undead=Loyal). |
| eu | ~38 | Basque has several ability-name collisions and missing terms. |
| is | ~38 | Icelandic has some gaps; T02 UI artifact now fixed. |
| gd | not read | Scottish Gaelic — not checked; likely sparse based on project coverage. |
| ga | not read | Irish — not checked; likely sparse. |
| ang@latin | not read | Old English — not checked; likely sparse. |
| en@shaw | not read | Shavian — not checked; likely sparse. |
| grc | not read | Ancient Greek — not checked; likely sparse. |
| racv | not read | Constructed language — not checked. |
| my | not read | Burmese — not checked. |
| mr | not read | Marathi — not checked. |
| bn | not read | Bengali — not checked. |
| cy | not read | Welsh — not checked. |

---

## Root Cause Analysis

The primary cause of widespread errors is the extraction tool's **context-free string matching**: when searching for a term like "Morning" in a .po file, the tool retrieves whatever msgstr is closest to the msgid — even if that msgid is a UI element like "Warning:" that happens to appear near time-of-day content in the file ordering. The following extraction improvements would prevent recurrence:

1. **Validate semantic field**: time-of-day terms should not produce words meaning Warning/Welcome/Victory.
2. **Prefer standalone nouns**: avoid extracting compound UI strings like "End scenario", "Next side", "Welcome".
3. **Cross-check with known-good languages**: if 30+ languages agree on "morning = morning-like word" and one extracts "warning", flag it automatically.
4. **Strip UI artifacts**: trailing colons in extracted strings indicate label extraction, not concept translation.
