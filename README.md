# 教育大數據專題製作
教育大數據專題製作  
姓名：呂沛修  
授課教師：蔡芸琤  

## 6/27(第三次上課)
練習 1：從 Huggingfacehub 上試著抓取模型  

這次所抓取的模型：stable-diffusion-v1-5 (text to image)  
模型測試並改變的結果(https://github.com/PeiHsiuLu/Education-folio/blob/main/big_data.ipynb)  

更改的內容：
模型原先是單一的文字生成圖片，我嘗試讓它有更多的互動性，改成讓用戶輸入文字便能生成特定的影像。

補充的資源：
langchain、tavily AI


## 6/27(第四次上課)
練習 2 ：Gimini AI  

補充資源：  
1. Gimini AI  
2. Gradio  

可以上網找影片自學(找與自己想做的專案相近的東西)  

## 課後自主學習 7/2

### Hugging face (image to image)  
[課後嘗試：Hugging face ](https://github.com/PeiHsiuLu/Education-folio/blob/main/Hugging_face_image2image.ipynb)  
所採用模型：stabilityai/stable-diffusion-xl-refiner-1.0  

## 課後自主學習 7/3  

### langchain  
1. 旨在為開發者提供一套工具和接口，以便更容易、更有效地利用大型語言模型（LLM）的開源框架
2. 主要包含的程式語言函式庫： JS,python
3. 簡單來說，就是提供一個接口，讓使用者更方便運用AI模型，可以直接使用，而不需要再額外耗時訓練


LangChain 旨在為開發者提供一套工具和接口，以便更容易、更有效地利用大型語言模型（LLM）的開源框架。它主要包含適用於 JavaScript 和 Python 的函式庫，讓開發者可以在這兩種常見的程式語言中輕鬆使用 LLM。簡單來說，LangChain 提供了一個接口，讓使用者更方便地運用預訓練的 AI 模型，可以直接使用這些模型，而不需要再額外耗時訓練。此外，LangChain 還提供了各種工具和範例來幫助開發者快速構建和部署應用程序。


## 專題製作 7/4
套用Hugging face 模型：openai/whisper-large-v3
(speech to text)  
我先將下載的影片轉為mp3音檔，再轉成文字輸出。  
[聲音轉文字](https://github.com/PeiHsiuLu/Education-folio/blob/main/Educationfolio_project.ipynb)  

# 專題製作
[專題主要的成果都放在這裡](https://github.com/SAStommy/eduAIproject/tree/main)  
呂沛修負責的部分：蒐集資料、整理正負面語氣的 label  (500筆 train, 500筆 validation)、訓練後再修正所抓取的資料   
杜洺鋒負責的部分：撰寫程式、gradio前端、Fine-tuned model  

此次做專題的心得：  
我認為收集資料最累人的部分在於要蒐集的資料數量眾多，而且考慮必須讓資料多元化，還得考慮心得評論情感的問題。此外，爬蟲可能會抓到太多重複課程的資料，可能對於 AI 的模型訓練不太有利。所以，最終只能採取人工抓取資料的手段。  

[驗證資料 validation](https://github.com/PeiHsiuLu/Education-folio/blob/main/0714_education.csv)  
[訓練資料 train](https://github.com/PeiHsiuLu/Education-folio/blob/main/0714_train.csv)  

後來我們沒有使用到驗證資料
