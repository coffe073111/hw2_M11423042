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
│  ├─ 
│  ├─ 
│  ├─ 
│  └─ 

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

共四個檔案，探討 **CART 決策樹** 之 **後剪枝 (Cost-Complexity Pruning)** 與模型複雜度。

| 檔名 | 功能說明 |
|------|-----------|
| **dm_post_pruning_decision_tree_finalver.ipynb** | 透過 **Grid Search** 比較不同樹深度與葉節點數的組合，並以 **Elbow Method** 尋找模型複雜度與準確率的平衡點。選出三組代表模型（Small、Medium、Large），最後於測試集進行評估。 |
| **Small_tree_d3_l16.png** | 小型模型（樹深度=3，葉節點=16）之決策樹圖。 |
| **Medium_tree_d6_l16.png** | 中型模型（樹深度=6，葉節點=16）之決策樹圖。 |
| **Large_tree_d10_l64.png** | 大型模型（樹深度=10，葉節點=64）之決策樹圖。 |

---

###  環境設定

  ● requirements：環境設定。

