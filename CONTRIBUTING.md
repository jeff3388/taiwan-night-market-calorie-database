# Contributing to taiwan-night-market-calorie-database

## 資料來源要求

所有熱量數據必須來自：
- 衛福部食藥署 TFND（台灣食品成分資料庫）— 優先來源
- USDA FoodData Central（原料參考）
- 衛福部國民健康署外食熱量指南

不接受：部落格估計值、個人測量、食品廠商提供數據（利益衝突）。

## 如何提交

1. Fork 此 repository
2. 在 `data/street-food-calories.json` 新增項目
3. 填寫所有必要欄位（`calories_kcal`、`protein_g`、`fat_g`、`carbs_g`、`source`）
4. 更新 `_meta.last_updated`
5. 提交 Pull Request，說明數據來源

## 接受的貢獻

- 新增台灣各地夜市常見食物（需有 TFND 數據支持）
- 更新已有食物的更精確熱量（附新來源）
- 補充各縣市夜市特色食物（台南、高雄、台中等）
- 新增點餐調整建議（`smart-choices.json`）

## 不接受的貢獻

- 熱量「估算」（無 TFND 或 USDA 依據）
- 特定夜市攤商廣告或推薦
- 健身補充品或代餐廣告
- 宣稱某食物「有助減重」而無科學依據
- 重複內容或 SEO 填充

## 熱量分級標準

| `calorie_level` | 熱量範圍 |
|----------------|---------|
| `light` | < 250 kcal |
| `moderate` | 250–400 kcal |
| `high` | 400–600 kcal |
| `very_high` | > 600 kcal |

## 注意事項

夜市食物熱量因攤販而異，本資料庫數據為標準份量的估計值。
所有數據標示「來源：衛福部食藥署 TFND」表示基於原料成分計算，
非直接測量成品。Pull Request 需說明計算方式。

---

本資料庫以公共衛生教育為目的，不作為任何飲食計畫的唯一依據。
