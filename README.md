# Covid-Data-Analysis
# 🧪 COVID-19 死亡風險分析與預測模型

本專案旨在分析 COVID-19 病患的基本資料與慢性病情況，找出與死亡風險顯著相關的變數，並建立預測模型。專案中整合了邏輯回歸、PCA、隨機森林、XGBoost 等方法，並利用 SMOTE 處理資料不平衡問題，以提升模型對死亡樣本的識別能力。

---

## 📌 專案目標
- 透過統計與機器學習方法，找出影響病患死亡的重要因素
- 建構準確的死亡風險預測模型
- 練習資料處理、特徵選擇、模型建立與資料不平衡處理的全流程實作

---

## 🔧 使用技術與方法

| 類別 | 方法/工具 |
|------|-----------|
| 資料處理 | pandas, sklearn.preprocessing |
| 統計分析 | Logistic Regression, Cramér’s V |
| 降維視覺化 | PCA（主成分分析） |
| 機器學習 | Random Forest, XGBoost |
| 不平衡資料處理 | SMOTE（Synthetic Minority Oversampling Technique） |
| 評估指標 | Accuracy, Recall, Precision, F1-score, Confusion Matrix |

---

## 📊 分析流程與亮點摘要

1. **資料清理與描述統計**：處理缺失值、類別轉換，進行變數分佈與死亡率分析。
2. **邏輯回歸模型**：檢驗如年齡、住院、糖尿病等變數與死亡風險的關聯性。
3. **主成分分析（PCA）**：
   - 前 5 個主成分解釋 88% 變異
   - 可視化區分死亡與存活族群
4. **初步模型評估**：
   - 使用 Random Forest 與 XGBoost 預測死亡風險
   - 雖然整體準確率高，但死亡樣本召回率偏低（約 18%）
5. **使用 Cramér’s V 選擇重要變數**：篩選出與死亡風險最相關的變數如住院、肺炎、COPD 等
6. **SMOTE 平衡資料**：提升死亡樣本召回率至 95%，但 precision 降至 34%，反映 recall-precision 的取捨

---
