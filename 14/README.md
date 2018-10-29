評估模型
==
為了決定一個分類模型是否準確地捕捉了模式，我們必須評估該模型。評估的結果對於決定模型是多麼值得信賴以及我們如何使用它是非常重要。評估也可以是一個有效的工具，用於指導我們在未來改進模型。

- 測試集
1. 注意少數標籤的數量
對於有少量平衡的標籤和一個多樣化的測試集的分類任務，只要100個評估實例就可以進行有意義的評估。
但是，如果一個分類任務有大量的標籤或包括非常罕見的標籤，那麼選擇的測試集的大小就要保證出現次數最少的標籤至少出現50次。

2. 確保測試集獨立
如果測試集中出現來自於訓練集的資料，將高估模型的精度

3. 注意樣本多樣性
測試集與訓練集的數據越相似輸出的精度就越可能被高估，也許模型只適合使用在這種類型的資料，例如評估東方股市指標的模型使用西方股市資料測試精度往往降低，因為訓練模型時就沒碰過西方數據

- 準確度
解釋一個分類器的準確性得分，考慮測試集中單個類標籤的頻率是很重要的。
我們在以色列判斷阿明95%是猶太人比起在美國判斷阿明95%是猶太人，一樣是95%但積極程度是不一樣的

- 精確度和召回率