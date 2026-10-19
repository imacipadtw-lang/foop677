# 土城國小英文700單字 聽力闖關遊戲

每一關一個英語聽力遊戲，對應學校自編的「英文700單字」句型。

| 關卡 | 主題 | 遊戲 |
|---|---|---|
| 第3關 | No. 46–66 身體部位與狀態 | [健康小隊長 Health Hero](level03/) |
| 五年級 | 單元課文（Sunday、science / art / PE class、ice hockey） | [麻糬養成闖關 Pet Pal English](pet5/) |
| 五年級 | 單元課文（Where are you from? / museum / boat / How do you go to school?） | [麻糬去旅行 Pet Pal Trip](pet5u2/) |

## 第3關 玩法
1. 走到頭上有「!」的同學旁邊，聽他用英文說哪裡不舒服（預設無字幕）。
2. 帶他到能幫忙的地方：健康中心、飲水機、餐廳、洗手台、衛生紙、置物櫃、休息區、操場。
3. 去健康中心時，要在人體圖上點出痛的部位。
4. 每輪 10 位同學，最後是「護理師的考驗」。

操作：方向鍵／WASD，或在畫面上按住想去的地方。支援電腦、平板、手機。

## 技術說明
- 單一 HTML 檔，語音已內嵌，不需要伺服器。
- 3D 畫面使用 three.js r128（cdnjs）；裝置不支援 WebGL 時自動改用 2D 地圖。
- 學習紀錄只存在各自裝置的瀏覽器（localStorage）。

## 語音來源與授權
- 第 47–66 句：ElevenLabs（[elevenlabs.io](https://elevenlabs.io)）Alice 語音產生。依 ElevenLabs 條款，免費方案產生的內容不得商業使用，非商業分享時須標註 ElevenLabs。
- 第 46 句：開源 Kokoro 語音模型合成（`bf_alice` 聲音）。
- 本專案僅供教學、非商業使用。

## 五年級 麻糬養成闖關（pet5/）
- 網址（teachers 站，已開 Pages，密碼 0686）：https://imacipadtw-lang.github.io/teachers/workbook/pet5/
- 本倉庫的 GitHub Pages 尚未開啟；開啟後也可用 https://imacipadtw-lang.github.io/foop677/pet5/
- 玩法：聽英文選圖卡、排句子（點選或拖曳）、選回應、情境對話；答對得到能量，餵寵物「麻糬」長大、布置小屋、換造型。
- 以 iPad 橫式為主；直式會提示把 iPad 橫過來（也可選擇先用直式玩）。
- 進度只存在各自裝置的瀏覽器（localStorage）；無法儲存時會提示，遊戲仍可進行。
- 發音：教材有 `audio=` 錄音檔時優先播放，否則使用裝置內建英語語音（只朗讀英文）。
- 老師設定（首頁 →「老師設定」）：可貼入／修改教材、檢查格式、預覽題目、調整題數、複製學生版連結或下載學生版檔案、重設進度。
- 示範教材核對說明：原文撇號統一為「'」；「Does she have science class on Monday?」未交代 she 是誰，改用「星期一＋自然課」圖卡出題；課文開頭是 Sunday，後面卻問 PE class today，遊戲不出需要判斷星期幾的題目。

## 五年級 麻糬去旅行（pet5u2/）
- 網址（teachers 站，已開 Pages，密碼 0686）：https://imacipadtw-lang.github.io/teachers/workbook/pet5u2/
- 與 pet5 相同玩法與老師設定，進度分開儲存。
- 教材核對：原文「He is ...」句子不完整，未出題；原文未標說話者，暫以中文角色標示；「I go to school on foot. He goes to school by car.」拆成兩句練習 on foot / by car。

## 語音（pet5、pet5u2 共用做法）
- 每句英文都用開源 Kokoro 神經語音模型預先錄好（真人感語音，不是裝置的機器人聲），以 MP3 嵌在 index.html 內，離線也能播。
- 角色配不同聲音：男孩（Teddy、Edison、Rocky）、女孩（Amber、Girl、Mia）；每句有慢、中、正常三種語速。
- 老師用「老師設定」加入新句子時，沒有預錄的句子會自動改用裝置語音；要補錄可依 tts/gen.py 的流程重新產生。
- 寵物體型隨成長值連續變大（25 cm → 70 cm），不只換裝。
- 新題型「聽對話，解問題」：聽完一問一答，依中文問題選出答案圖卡（素養導向的理解題）。
