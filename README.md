# Alan's 3D Lab — Voron 350 用模組化工具頭／Modular toolhead for the Voron 350

版本 v0.2 加厚版・2026-11-12　（Version v0.2, thicker-wall release, 2026-11-12）
網頁 Page：https://www.voron.com.tw/works/toolhead

## 開放測試中 檔案免費下載・尚未經過實機驗證
這是我正在一步一步列印、組裝、改裝中的設計，先把完整模型和檔案開放出來，給想一起測試的人參考。
我自己還沒完成實機驗證，之後可能會有修正檔更新；全部組裝好之後，會補上實機照片。

## 下載須知
這是測試分享，不保證能直接用；請自行評估、自負列印與使用風險。發現問題歡迎回報，修正後會在更新紀錄寫清楚改了什麼。
回報問題：LINE https://line.me/ti/p/gBlruyjDjE

## 授權
設計：Alan（Alan's 3D Lab）。授權 CC BY-NC-SA 4.0：可以自由修改，但要註明作者、不能商用，改了也要用同樣方式分享。Voron 標誌屬於 Voron Design，本設計不是 Voron 官方出品。
CC BY-NC-SA 4.0 授權說明：https://creativecommons.org/licenses/by-nc-sa/4.0/deed.zh-hant
授權條款全文：https://creativecommons.org/licenses/by-nc-sa/4.0/legalcode

## 怎麼印 STL/ 裡的檔已經轉成列印方向、底面貼床（z = 0），直接切片。材料 ABS（或 ASA），牆加厚後建議 100% 牆或高填充。每件需要的支撐面積在 parts.csv。
四種熱端座（蚊子、龍、紅蜥蜴、X1C）依你的熱端選一個印，所以一套實際要印 13 件。heatmaps/ 是每件的壁厚熱圖（紅色＝薄於 2 mm）。

## v0.2 改了什麼
・所有列印件最薄處加厚到 2 mm 以上（平躺列印的薄板例外），孔洞完整，螺絲與熱熔螺母周圍至少 2 mm。
・修正 v0.1 的 8 個錯誤：SB2209 排針撞脊座、線材支架兩顆螺絲裝不上、2510 風扇座螺絲頭在葉片裡、壓臂惰輪軸孔兩端盲孔、彈簧螺母埋在 PTFE 管下、板框只有 1.2 mm（螺絲柱壁 0.1 mm）、前燈板凹槽封死、冷卻件凸台與導風罩碰到排針。
・設計變更：5015 轉 35° 並上移 3.5 mm；線材支架移到板框；壓臂後頰加 2.8 mm 環壁；2510 風扇座改 7.4 mm 框；燈窗與面框改 2.2 mm。
・受力用 ABS 層間強度重算：脊座層間安全係數 4.2→5.3、擠出機殼 5.1→5.6、壓臂 3.9→4.2；全機 310 組零件 0 干涉；壓臂打開到 14° 不碰任何零件。
・列印方向重新決定：支撐從 77 cm² 降到 41 cm²（不含冷卻件）；2510 風扇座翻面免支撐、紅蜥蜴座改平躺。
・BOM 變更：新增 M3 圓墊高柱 5 mm × 1（前燈板右孔）；2510 風扇前兩角改 M3×25 × 2；板框孔 2 改 M3×20 沉頭、腳座 M3×10 圓頭；取消 v0.1 線材支架那兩顆 M3。
・已知例外：X1C 熱端座螺絲孔旁 1.61 mm；鏡頭座鏡頭窗為 U 形開口。

------------------------------------------------------------

[Open testing] Free download. Not yet verified on a real machine.
This is a design I'm printing, assembling and modifying step by step. I'm sharing the full model and files now for anyone who wants to test it with me.
I haven't finished testing it on a real machine yet, so fixes may follow. Once everything is assembled, I'll add photos of the real build.

[Before you use these files]
This is a test share and may not work as-is. Please judge for yourself; printing and use are at your own risk. Problem reports are welcome, and every fix will be described in the changelog.
Report a problem on LINE: https://line.me/ti/p/gBlruyjDjE

[License]
Design: Alan (Alan's 3D Lab). License: CC BY-NC-SA 4.0. You may modify it freely, but you must credit the author, may not use it commercially, and must share any changes under the same license. The Voron logo belongs to Voron Design; this design is not an official Voron product.
CC BY-NC-SA 4.0 summary: https://creativecommons.org/licenses/by-nc-sa/4.0/deed.zh-hant
Full license text: https://creativecommons.org/licenses/by-nc-sa/4.0/legalcode

[How to print] The files in STL/ are already in print orientation with the bottom on the bed (z = 0); slice them as they are. ABS (or ASA); with the thicker walls, use 100% walls or high infill. parts.csv lists the support area of each part.
Pick the one hotend carrier (Mosquito, Dragon, Red Lizard or X1C) that fits your hotend, so one set is 13 printed parts. heatmaps/ holds a wall-thickness map per part (red = thinner than 2 mm).

[What changed in v0.2]
- Every printed part is at least 2 mm thick (flat-printed plates excepted), holes are complete, and there is at least 2 mm around every screw and heat-set insert.
- Fixed 8 v0.1 errors: SB2209 header hitting the spine, wire-bracket screws that could not be fitted, 2510 fan-seat screw heads inside the blades, idler-arm shaft hole blind at both ends, spring nut buried under the PTFE tube, 1.2 mm board frame (0.1 mm screw-post wall), sealed front-light board pocket, and the duct boss and shroud touching header pins.
- Design changes: 5015 turned to 35° and raised 3.5 mm; wire bracket moved to the board frame; 2.8 mm ring wall on the idler arm; 2510 fan seat now a 7.4 mm frame; light window and mask now 2.2 mm.
- Strength recomputed with ABS layer-to-layer strength: spine layer safety factor 4.2→5.3, extruder body 5.1→5.6, idler arm 3.9→4.2; 0 clashes across 310 part pairs; the idler arm opens to 14° without touching anything.
- Print orientations reworked: supports down from 77 cm² to 41 cm² (excluding the duct); the 2510 fan seat now prints flipped with no supports, the Red Lizard carrier lies flat.
- BOM changes: add one 5 mm M3 round standoff (front-light board, right hole); 2510 fan front corners now M3×25 × 2; board frame hole 2 now M3×20 countersunk, feet M3×10 button head; the two v0.1 wire-bracket M3 screws are dropped.
- Known exceptions: 1.61 mm next to the X1C carrier screw hole; the camera mount window is a U-shaped opening.

## 下載 Downloads

| 版本 | 下載 |
| --- | --- |
| v0.2 加厚版 | [整包 zip / all files](https://github.com/alans3dlab/toolhead-350/releases/download/v0.2/alans3dlab-toolhead-v0.2-stl.zip) · [逐件檔案 / individual files](https://github.com/alans3dlab/toolhead-350/releases/tag/v0.2) |
| 單頭方案 Single-head scheme（2026-11-13） | [整包 zip / all files](https://github.com/alans3dlab/toolhead-350/releases/download/single-head-20261113/SINGLE_all.zip) · [逐件檔案 / individual files](https://github.com/alans3dlab/toolhead-350/releases/tag/single-head-20261113) |

網頁 Page：https://www.voron.com.tw/works/toolhead

## 單頭方案 v0.6 Single-head scheme v0.6 (single-head-v0.6)

左燈臂、側蓋螺絲頭孔、副板蓋立柱與線口更新；取消 SH-B10。五金規格彙總含未定與待實物確認項目，詳見 manifests/single-head-v0.6/BOM.csv。

Left light arm, screw-head opening, board-cover posts and cable opening updated. Hardware statuses remain explicit.
