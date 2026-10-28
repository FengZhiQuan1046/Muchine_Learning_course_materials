# ML 前置工具精簡版

適用於已學過 vibe coding 的學生。程式可由 AI 協助產生，課堂重點是看懂資料、說明運算意義並檢查結果。

建議依序閱讀：

1. [NumPy](./numpy-基本功能.ipynb)：shape、取值、axis、broadcasting 與矩陣乘法；保留 softmax、Linear Layer／ReLU 的 ML 練習。
2. [pandas](./pandas-基本功能.ipynb)：讀取與檢查資料、選取、缺失值及 X／y。
3. [視覺化](./matplotlib-資料視覺化.ipynb)：按問題選圖、判讀分布與特徵關係。
4. [scikit-learn](./scikit-learn-基本功能.ipynb)：保留前處理、模型、驗證、評估與 ML 練習，縮短環境介紹及存檔／載入等操作。
5. [PyTorch](./PyTorch-基本功能.ipynb)：Tensor、批次資料、神經網路、梯度、訓練與驗證。

已合併重複的索引與算術示範，省略型別範圍大全、逐行語法註解、進階線性代數 API 枚舉與繪圖外觀設定。需要個別功能時，再請 AI 協助查用；課堂仍需確認 shape、資料對應與輸出意義。

在 notebook 使用的 Python 環境安裝一次即可；環境已備妥可略過：

```sh
python -m pip install numpy pandas matplotlib seaborn scikit-learn
```

PyTorch 請依作業系統及 CPU／GPU 環境參考 [官方安裝頁面](https://pytorch.org/get-started/locally/)。

從 `simplified` 目錄開啟並依序執行各 notebook。pandas 與視覺化使用隨附的 [模擬氣象資料](./data/weather_sample.csv)：12 筆教學資料，含一筆缺失氣溫，並非真實觀測。`Day` 是日期序號，`Temperature` 為攝氏氣溫，`Humidity` 為相對濕度百分比，`Weather` 為天氣類別，`Rain` 表示是否下雨（0／1）。

scikit-learn 的 Titanic 段落仍需自行下載 `train.csv`，放在 `simplified/data/`。所有精簡調整都在本目錄，`original/` 保留原教材。
