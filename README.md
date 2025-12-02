# 🌵 FF14 仙人微彩數據池

這是一個 **Final Fantasy XIV 仙人微彩 (Cactpot)** 的社群數據收集專案。

透過收集大量玩家數據，我們可以進行統計分析，找出最佳策略！

---

## 📊 這是什麼？

- **數據收集**: 收集玩家的仙人微彩遊戲記錄
- **統計分析**: 分析數字分布、獎勵規律
- **AI學習**: 訓練機器學習模型預測最佳選擇
- **社群共享**: 所有人都能受益於更大的數據樣本

---

## 🎮 配套工具

### **FF14 仙人微彩分析器**
- 智能推薦翻開位置
- 4種選線策略 (平衡/保守/激進/AI學習)
- 深度統計分析
- 機器學習預測模型
- **自動從此Repo同步數據**

> 分析器會自動讀取這個Repo的所有JSON檔案，合併成超大數據池！

---

## 📤 如何貢獻數據？

### **方法1: 網頁上傳 (最簡單)** ⭐

1. **匯出你的數據**
   - 在分析器點「📤 匯出數據」
   - 下載 JSON 檔案

2. **上傳到這個Repo**
   - 點上方 `Add file` → `Upload files`
   - 拖曳你的 JSON 檔案
   - 檔名建議: `你的遊戲ID.json` 或 `你的名字_日期.json`
   - 寫 Commit message: 例如 "Add my 50 games data"
   - 點 `Commit changes`

3. **完成！**
   - 所有使用分析器的人會自動同步你的數據
   - 樣本量增加，AI預測更準確！

---

### **方法2: Pull Request (開放貢獻)**

如果你不是Collaborator:

1. **Fork這個Repo**
   - 點右上角 `Fork` 按鈕

2. **在你的Fork中上傳JSON**
   - `Add file` → `Upload files`
   - 上傳你的數據

3. **發送Pull Request**
   - 點 `Contribute` → `Open pull request`
   - 簡短說明你的數據 (例如: "50局遊戲記錄")
   - `Create pull request`

4. **等待審核**
   - 管理員會檢查並合併

---

### **方法3: Git指令 (進階)**

```bash
# Clone這個repo
git clone https://github.com/Roromumu/cactpot-data.git
cd cactpot-data

# 複製你的JSON檔案
cp ~/Downloads/my_cactpot_data.json .

# Commit並Push
git add .
git commit -m "Add my cactpot data"
git push
```

---

## 📋 數據格式

你的JSON檔案應該是從分析器匯出的標準格式:

```json
{
  "version": "1.0",
  "exportDate": "2024-12-02T10:30:00.000Z",
  "totalGames": 50,
  "data": [
    {
      "timestamp": "2024-12-01T08:15:00.000Z",
      "fullGrid": [[3,7,2],[6,8,4],[1,9,5]],
      "selectedLine": "左斜線",
      "actualReward": 108,
      ...
    },
    ...
  ],
  "metadata": {
    "averageReward": 250,
    "highRewardCount": 8
  }
}
```

### **必要欄位:**
- ✅ `version`: 版本號
- ✅ `data`: 陣列，包含所有遊戲記錄
- ✅ 每筆記錄需有: `timestamp`, `fullGrid`, `actualReward` 等

---

## 🗂️ 檔案組織

你可以自由組織你的檔案:

```
cactpot-data/
├── player1.json
├── player2.json
├── archive/
│   ├── 2024-01.json
│   └── 2024-02.json
└── community/
    ├── alice.json
    └── bob.json
```

**分析器會自動遞迴讀取所有子資料夾的 `.json` 檔案！**

---

## 📊 目前統計

<!-- 可以手動更新這個區塊 -->

- **總貢獻者**: ? 人
- **總遊戲局數**: ? 局
- **數據更新日期**: ?

---

## 🤝 貢獻指南

### **數據品質要求:**
- ✅ 確保是完整的9格數據
- ✅ 包含實際獲得獎勵
- ✅ 時間戳記正確
- ❌ 不要上傳測試數據
- ❌ 不要上傳重複數據

### **檔案命名建議:**
- `你的ID.json` - 個人數據
- `你的ID_2024-12.json` - 月度數據
- `群組名_資料.json` - 團隊數據

### **隱私注意:**
- 數據是匿名的
- 不包含角色名或伺服器資訊
- 只有遊戲數字和結果

---

## ❓ 常見問題

### **Q: 我的數據會被怎麼使用?**
A: 純粹用於統計分析和AI訓練，完全匿名，不涉及個人資訊。

### **Q: 我可以刪除我的數據嗎?**
A: 可以！發PR刪除你的檔案，或聯繫管理員。

### **Q: 需要上傳多少數據?**
A: 任何數量都歡迎！即使只有10局也很有價值。

### **Q: 多久需要更新一次?**
A: 隨意！累積一定數量後再上傳即可。

### **Q: 上傳後多久生效?**
A: 立即生效！所有使用分析器的人打開頁面時會自動同步。

### **Q: 我發現別人的數據有問題怎麼辦?**
A: 發Issue或PR修正，維護數據品質是大家的責任。

---

## 🔗 相關連結

- **分析器網址**: [待補充]
- **問題回報**: [Issues](https://github.com/Roromumu/cactpot-data/issues)
- **討論區**: [Discussions](https://github.com/Roromumu/cactpot-data/discussions)

---

## 📜 授權

此專案數據採用 **CC0 1.0 (公眾領域)** 授權。

任何人都可以自由使用、修改、分發這些數據。

---

## 🎉 特別感謝

感謝所有貢獻數據的玩家！

你們的數據讓社群的AI越來越聰明！ 🤖✨

---

## 💬 聯絡方式

有任何問題或建議？

- 發 Issue
- 開 Discussion  
- 或直接PR

讓我們一起建立最強的仙人微彩數據池！ 🌵🎰💰
