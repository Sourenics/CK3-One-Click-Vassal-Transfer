# Changelog

## 1.3.1

- **Fixed:** titles were still given to vassals living outside them. A recipient must now **reside** inside the title (their capital lies de jure within it) as well as hold their primary title there. A Duke of Bavaria living in Saxony no longer receives the Kingdom of Bavaria.
- The last-resort recipient is now whoever in your realm holds the most counties inside the title, not only your direct vassals. They become your direct vassal first.
- **Fixed:** noble family titles (administrative, celestial, sōryō and ritsuryō governments), nomad titles, mercenary companies and holy orders are no longer offered for granting or distribution. The exclusion button is hidden on noble family titles.

## 1.3.0

- Decisions are now hidden when they have nothing to do: no vassal to transfer, no title available to create, or no county or title left to hand out (after exclusions).
- The county grant decisions show how many new vassals they will create, with a reminder to watch your vassal limit.
- Players using French, German, Polish, Russian, Simplified Chinese, Korean or Japanese now see the English text instead of raw localization keys.
- Spanish: game concepts are now lowercased mid-sentence, as in the base game.

## 1.2.0

- **Transfer Vassals to their De Jure Liege** now lists in its Effects section every vassal that will be transferred and their new liege, before you confirm.
- Transfers are now decided all at once on the realm as it is, then applied. The result always matches the preview, and is no longer affected by the order in which vassals are processed.

## 1.1.0

- **No more bordergore when distributing titles.** Recipients are now chosen by the titles they hold, not by where they live, and their primary title must lie de jure within the title they receive. A Duke of Bavaria living in a Saxon county now receives the Kingdom of Bavaria, never the Kingdom of Saxony.
- **Cascading recipient search.** An empire goes to the holder of its capital kingdom, then of its capital duchy, then of its capital county; a kingdom to the holder of its capital duchy, then of its capital county; a duchy to the holder of its capital county. As a last resort, it goes to the vassal with the most counties in it.
- If the chosen holder is a vassal of one of your vassals, they first become your direct vassal and then receive the title.
- If no vassal qualifies, you keep the title. The Effects preview shows it before you confirm.
- Updated decision descriptions in English and Spanish.

## 1.0.0

- First public release.
- Decisions to transfer vassals to their de jure liege, grant counties to brand-new characters (your culture or local culture), create duchies, kingdoms and empires, and distribute them to the vassals who rule their de jure capitals.
- De jure vassals automatically move under the new holder when a title is distributed.
- Exclusion toggle in the title window to keep any title out of the distribution.
- Preview in the Effects section of each decision: every title that will be handed out and its recipient.
- English and Spanish localization.
