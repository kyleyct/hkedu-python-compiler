# HK Edu Python Compiler

瀏覽器內 Python 編譯器（MVP）：以 **Pyodide** 執行 Python，並支援 **NumPy**／**pandas**；可上傳 CSV 後於程式碼中以 `pd.read_csv('檔名.csv')` 讀取。

**示範：** https://kyleyct.github.io/hkedu-python-compiler/

## 功能

- 線上編輯器 + Console 輸出 + DataFrame／值預覽
- 內建示例：Hello World、NumPy、pandas
- 多檔 CSV 拖放／選擇上傳（執行環境內讀取）
- Run／Reset Runtime／Clear Output

## 使用

1. 開啟 [GitHub Pages](https://kyleyct.github.io/hkedu-python-compiler/)，或
2. 本機：

```bash
git clone https://github.com/kyleyct/hkedu-python-compiler.git
cd hkedu-python-compiler
python3 -m http.server 8080
# http://localhost:8080/
```

首次載入需下載 Pyodide 執行環境，請稍候。

## 技術

- `index.html` + `py-worker.js`
- Pyodide（WebAssembly Python）
- 靜態託管（含 `.nojekyll`）

## 授權

未於 repo 宣告授權時，使用前請先向作者確認，或自行補上合適授權。
