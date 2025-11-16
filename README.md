# hw2_M11423042
資料探勘作業二
---

## 專案結構 <a id="structure"></a>

```text
.
├─ 資料夾(資料前處理一)/
│  ├─ adult_data_duplicate.ipynb
│  ├─ adult_test_duplicates.ipynb
│  └─ adult_data_missing_value.ipynb
├─ 資料夾(實驗一)/
│  ├─ KNN_SVR_RandomForest_XGBoost.ipynb
│  ├─ Train_Time.png
│  ├─ Predict_Time.png
│  ├─ R2.png
│  ├─ RMSE.png
│  ├─ MAPE.png
├─ 資料夾(實驗二)/
   ├─ 
   ├─ 
   ├─ 
   └─ 

```






###  資料前處理

內含三個 `.ipynb` 檔案，負責資料清理與補值處理。

| 檔名 | 功能說明 |
|------|-----------|
| **adult_data_duplicate.ipynb** | 偵測並移除訓練集中的重複筆數（僅保留一筆）。 |
| **adult_test_duplicates.ipynb** | 偵測並移除測試集中的重複筆數（僅保留一筆）。 |
| **adult_data_missing_value.ipynb** | 偵測訓練集缺失值（如 `?` 或空白），並依變數型態補植：<br>・數值型欄位 → 以中位數補值<br>・類別型欄位 → 以眾數或 `Unknown` 補值。 |

---

###  實驗一

共六個檔案，包含各演算法的預測績效以及所需要的計算時間。

####  圖像檔案
| 類別 | 檔名 | 說明 |
|------|------|------|
|比較長條圖| `Train_Time.png`, `Predict_Time.png`, `R2.png`, `RMSE.png`, `MAPE.png` | 各演算法的預測績效比較。 |

####  程式與結果檔案
| 檔名 | 功能說明 |
|------|-----------|
| **KNN_SVR_RandomForest_XGBoost.ipynb** | 使用前處理後資料集訓練並測試 *KNN、SVR、RandomForest、XGBoostT** 。 |

---

###  實驗二

共四個檔案，探討 **XGBoost** 、 **K-fold cross validation** 、 **SHAP**的實際應用

| 檔名 | 功能說明 |
|------|-----------|
| **shap_bar.png** | 各特徵對模型預測影響力的平均大小 |
| **xgboost_reduced_only.png** | 刪除三個特徵後的預測績效 |
| **xgboost_full_only.png** | 使用全部 13 個特徵時的預測績效 |
| **hw2_finalverse.ipynb** | 使用 XGBoost 演算法及 K-fold cross validation預測資料集，以及SHAP 計算特徵重要性，進行特徵欄位之重要性排名 |


---


