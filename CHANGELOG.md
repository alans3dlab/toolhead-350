# 更新紀錄 Changelog

## 單頭方案 v0.5（2026-11-16）

- 前臉整個重畫（參數化 CAD，附 STEP 與 3MF）：稜角 5015 風扇殼（風扇從正面放入、SH-08 風扇蓋板代替原廠上蓋）、四條獨立冷卻風管 SH-13（左前、右前、左後、右後）、兩片 45 度 RGB 噴嘴燈、新的鏤空副板蓋 SH-14、照 VORON 官方比例重畫的 LOGO、蜂窩 SB2209 蓋板。取消 SH-10 相機座。

*New front: faceted 5015 shell, four separate cooling ducts, two 45-degree RGB nozzle lights, open board cover, redrawn logo, honeycomb side cover; side camera mount dropped.*

## v0.2 加厚版（2026-11-12）

- 所有列印件最薄處加厚到 2 mm 以上（平躺列印的薄板例外），孔洞完整，螺絲與熱熔螺母周圍至少 2 mm。
- 修正 v0.1 的 8 個錯誤：SB2209 排針撞脊座、線材支架兩顆螺絲裝不上、2510 風扇座螺絲頭在葉片裡、壓臂惰輪軸孔兩端盲孔、彈簧螺母埋在 PTFE 管下、板框只有 1.2 mm（螺絲柱壁 0.1 mm）、前燈板凹槽封死、冷卻件凸台與導風罩碰到排針。
- 設計變更：5015 轉 35° 並上移 3.5 mm；線材支架移到板框；壓臂後頰加 2.8 mm 環壁；2510 風扇座改 7.4 mm 框；燈窗與面框改 2.2 mm。
- 受力用 ABS 層間強度重算：脊座層間安全係數 4.2→5.3、擠出機殼 5.1→5.6、壓臂 3.9→4.2；全機 310 組零件 0 干涉；壓臂打開到 14° 不碰任何零件。
- 列印方向重新決定：支撐從 77 cm² 降到 41 cm²（不含冷卻件）；2510 風扇座翻面免支撐、紅蜥蜴座改平躺。
- BOM 變更：新增 M3 圓墊高柱 5 mm × 1（前燈板右孔）；2510 風扇前兩角改 M3×25 × 2；板框孔 2 改 M3×20 沉頭、腳座 M3×10 圓頭；取消 v0.1 線材支架那兩顆 M3。
- 已知例外：X1C 熱端座螺絲孔旁 1.61 mm；鏡頭座鏡頭窗為 U 形開口。

*thicker-wall release*

- Every printed part is at least 2 mm thick (flat-printed plates excepted), holes are complete, and there is at least 2 mm around every screw and heat-set insert.
- Fixed 8 v0.1 errors: SB2209 header hitting the spine, wire-bracket screws that could not be fitted, 2510 fan-seat screw heads inside the blades, idler-arm shaft hole blind at both ends, spring nut buried under the PTFE tube, 1.2 mm board frame (0.1 mm screw-post wall), sealed front-light board pocket, and the duct boss and shroud touching header pins.
- Design changes: 5015 turned to 35° and raised 3.5 mm; wire bracket moved to the board frame; 2.8 mm ring wall on the idler arm; 2510 fan seat now a 7.4 mm frame; light window and mask now 2.2 mm.
- Strength recomputed with ABS layer-to-layer strength: spine layer safety factor 4.2→5.3, extruder body 5.1→5.6, idler arm 3.9→4.2; 0 clashes across 310 part pairs; the idler arm opens to 14° without touching anything.
- Print orientations reworked: supports down from 77 cm² to 41 cm² (excluding the duct); the 2510 fan seat now prints flipped with no supports, the Red Lizard carrier lies flat.
- BOM changes: add one 5 mm M3 round standoff (front-light board, right hole); 2510 fan front corners now M3×25 × 2; board frame hole 2 now M3×20 countersunk, feet M3×10 button head; the two v0.1 wire-bracket M3 screws are dropped.
- Known exceptions: 1.61 mm next to the X1C carrier screw hole; the camera mount window is a U-shaped opening.

## v0.1 測試版（2026-11-06）

- 第一次開放測試下載：16 件列印件 STL。
- 2026-11-06 撤下：試印發現多處太薄、孔位不完整，正在重新設計，新版 v0.2 審核通過後再開放下載。

*test release*

- First open-test release: 16 printed parts as STL.
- Withdrawn 2026-11-06: test prints showed thin walls and incomplete holes; the redesign is under way and v0.2 will be released after review.
