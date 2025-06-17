# 📚 潛在狄利克雷分配（Latent Dirichlet Allocation, LDA）

本專案為《多變量分析課程》期末報告，探討 **LDA 模型的理論基礎與實務應用**，包含數學推導與資料分析兩個部分。

---

## 🔬 專案內容

### 1️⃣ 理論探討

- 介紹 LDA 模型的基本概念與生成過程
- 推導 Dirichlet 分配與模型後驗機率
- 使用 **Variational Inference**（變異數推論）與 **Gibbs Sampling** 進行模型估計
- 討論 ELBO、KL Divergence、Perplexity 等模型評估指標

### 2️⃣ 實務應用

#### 📄 BBC 新聞資料分析

- 收集 64 篇 BBC 新聞，涵蓋 8 個主題：
  - Sport、Business、Technology、Game、Travel、Music、Science、Political
- 文字前處理：
  - 斷詞、詞形還原（Lemmatization）、去除停用詞（Stopwords Filtering）
- LDA 主題建模分析
- 透過 **Perplexity Scree Plot** 及 **t-SNE 視覺化** 協助選擇適當的主題數

#### 💼 求職資料分析

- 蒐集約 80,000 筆職缺資料（來源：104、1111、MeetJob）
- 使用 **NER 技術** 萃取 skill tags 作為主題模型輸入
- 比較多種主題建模方法：
  - LDA
  - BerTopic
  - GPT-3.5-turbo 輔助分群

---

## 🛠 使用工具

- **程式語言**: Python
- **套件**: 
  - `gensim`、`scikit-learn`、`pandas`、`matplotlib`、`seaborn`、`t-SNE`
- **NLP 前處理**: 
  - Lemmatization、POS Tagging、Stopwords Removal

---

## 📖 參考文獻

- Blei, D.M., Ng, A.Y., & Jordan, M.I. (2003). *Latent Dirichlet Allocation*. Journal of Machine Learning Research, 3, 993–1022.
- [BBC News](https://www.bbc.com/news)
