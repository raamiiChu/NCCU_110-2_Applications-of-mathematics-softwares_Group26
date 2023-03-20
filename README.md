# NCCU_110-2_Group26_Applications-of-mathematics-softwares
國立政治大學 110學年度 第2學期 數學軟體應用 第26組期末專案  
授課教師: 蔡炎龍教授  

### 專案主題：辨識各國語言  
  輸入：單一語音檔案  
  輸出：該檔案的聲音可能為哪國語言（中、俄、西、德、阿拉伯）  
  
  ![阿拉伯語辨識結果](https://user-images.githubusercontent.com/87169493/226276376-bef8d265-4388-4491-8e35-9dfa49ff2058.png)
  
  蒐集的樣本數：
  |      | train | valid | test |
  |  ----  | ----: | ----: | ----: |
  | 中文  | 22048 | 11638 | 11655 |
  | 俄羅斯文 | 15481 | 7963 | 8007 |
  | 西班牙文 | 20000 | 15089 | 15089 |
  | 德文 | 20000 | 15588 | 15588 |
  | 阿拉伯文 | 14227 | 7517 | 7622 |
  
  調整後的樣本數：
  | train | valid | test |
  | ----:  | ----:  | ----:  |
  | 20000 | 15000 | 15000 |

### 專案檔案摘要  
- Group26_audio_classification_model  
  訓練出來的模型
  
- pt  
  用於訓練的語音檔案  
  來源：[Hugging Face common_voice datasets](https://huggingface.co/datasets/common_voice)  
  官方網站：[common voice](https://commonvoice.mozilla.org/zh-TW/datasets)  
  
- 測試用  
  內含多個程式碼，用於抓取檔案、串接資料、測試輸出結果、與組員溝通等  

- 測試用錄音  
  針對 G26_gradio.ipynb 進行測試的錄音檔（[詳細測試結果及檔案來源](https://docs.google.com/spreadsheets/d/1Fv-cWO_B7givWJH-OIAWjocNSOe71Gbi/edit?usp=share_link&ouid=110248902447125902030&rtpof=true&sd=true)）  

- G26_gradio.ipynb  
  使用 gradio 呈現結果  
 
- G26_神經網路(DNN).ipynb  
  建立神經網路、訓練模型  
