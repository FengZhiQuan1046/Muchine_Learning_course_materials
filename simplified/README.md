# ML 課程教材

課堂重點是看懂資料、說明運算意義並檢查結果。

建議依序閱讀：

1. [NumPy](./numpy-基本功能.ipynb)：shape、取值、axis、broadcasting 與矩陣乘法；保留 softmax、Linear Layer／ReLU 的 ML 練習。
2. [pandas](./pandas-基本功能.ipynb)：讀取與檢查資料、選取、缺失值及 X／y。
3. [視覺化](./matplotlib-資料視覺化.ipynb)：按問題選圖、判讀分布與特徵關係。
4. [scikit-learn](./scikit-learn-基本功能.ipynb)：資料前處理、模型、驗證、評估與 ML 練習。
5. [PyTorch](./PyTorch-基本功能.ipynb)：Tensor、批次資料、神經網路、梯度、訓練與驗證。

學習時請確認 shape、資料對應與輸出意義。

小練習依教材順序連續編號：NumPy 1–2、pandas 3–4、Matplotlib 5–7、scikit-learn 8。

小練習 1–8 集中於 [exercises.ipynb](./exercises.ipynb)，供作答及評分使用，只包含題目、資料準備與作答區，不提供解答或預期輸出。先執行套件匯入，再依序作答；各教材原位置保留對應題目的連結。

NumPy 與 pandas 的小練習及一般練習採程式填空；請補上 `____`，保留固定測資與 print 格式。

Matplotlib 與 scikit-learn 合計約 90 分鐘的授課安排（含短問答）：

|教材|時間|課堂範圍|
|---|---|---|
|Matplotlib|35 分鐘|從單張折線圖開始，讀氣象資料圖表，完成直方圖填空、熱圖範例與填空，講解分組箱型圖練習|
|scikit-learn：機器學習流程|10 分鐘|用線性迴歸看懂 fit、predict 與 X／y 的 shape|
|scikit-learn：資料前處理|15 分鐘|Titanic 欄位、缺失值填補、類別編碼；數值縮放與 one-hot 點到為止|
|scikit-learn：模型與驗證|15 分鐘|決策樹、max_depth、訓練／驗證切分，對照兩者 accuracy 理解過度適應|
|scikit-learn：評估與討論|15 分鐘|accuracy、precision、recall 的取捨與討論|

這個時程以課前安裝完成、Titanic 資料已備妥為前提。Matplotlib 的熱圖與分組箱型圖練習都在課堂講解。scikit-learn 的交叉驗證補充概念、末尾的模型改善／更換模型練習，留作課後閱讀與實作。

在 notebook 使用的 Python 環境安裝一次即可；環境已備妥可略過：

```sh
python -m pip install numpy pandas matplotlib seaborn scikit-learn
```

PyTorch 請依作業系統及 CPU／GPU 環境參考 [官方安裝頁面](https://pytorch.org/get-started/locally/)。

從 `simplified` 目錄開啟並依序執行各 notebook。pandas 與視覺化使用隨附的 [模擬氣象資料](./data/weather_sample.csv)：12 筆教學資料，含一筆缺失氣溫，並非真實觀測。`Day` 是日期序號，`Temperature` 為攝氏氣溫，`Humidity` 為相對濕度百分比，`Weather` 為天氣類別，`Rain` 表示是否下雨（0／1）。

scikit-learn 的 Titanic 段落仍需自行下載 `train.csv`，放在 `simplified/data/`。

scikit-learn 的概念示意圖隨附於 `images/scikit-learn/`，可離線顯示；搬移 notebook 時請一併保留此目錄。這些示意圖由專案自行繪製，在專案根目錄執行 `python scripts/generate_scikit_learn_figures.py` 可重新產生。
