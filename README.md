# 不動產實價登錄之應用—透過隨機森林進行房價預測
欲了解大台北地區租房價格行情，使用 113~114 年台北市和新北市的不動產資料，並透過隨機森林模型來預測未來租賃可能所需之價格。

## 工作描述
1. **數據處理：** 創造新特徵滿足使用需求，使用 one-hot encoding 或其他技術進行特徵轉換。針對空值進行填補或刪除，通過判斷決定異常值得留存。刪除不必要特徵，確保數據一致性。
2. **資料視覺化：** 了解各特徵分布，判斷是否有離群值或異常值，或是資料是否有線性關係。
3. **資料劃分：** 進行分層避免資料不平衡問題。
4. **模型建立：** 建立隨機森林模型解決迴歸問題。透過 RandomizedSearchCV 和 GridSearchCV 找到最佳參數。
5. **模型評估：** 使用交叉驗證和透過 R2 與 RMSE 指標來衡量模型的表現。
6. **成果展示：** 訓練好的模型可預測特地地區和類型的房價。 

## 資料來源：[內政部的不動產資料供應系統](https://plvr.land.moi.gov.tw/Login_input?authfailed=true#)
![不動產資料供應系統](photo/不動產資料供應系統.png)

## 使用技術與套件
- **數據處理：** Numpy、Pandas、SciPy
- **資料視覺化：** Matplotlib、seaborn
- **模型建立：** scikit-learn

