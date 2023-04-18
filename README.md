# 深度學習模型訓練
## YOLOV5 安裝
### Step1: 在anaconda prompt中建立一個叫yolov5的環境，並activate yolov5
![image](https://user-images.githubusercontent.com/79627981/232782139-0232bd8e-9ab8-4524-a7dd-d59f9c0bde38.png)
![image](https://user-images.githubusercontent.com/79627981/232782558-ae23a92c-e494-4ef3-b829-e0530ac5a6a3.png)
### Step2: 輸入git clone https://github.com/ultralytics/yolov5
![image](https://user-images.githubusercontent.com/79627981/232782646-148d6919-89f3-4e25-9361-c157b5160ed2.png)
### Step3: 安裝完yolov5後，至 https://pytorch.org/ 安裝PyTorch(將得到的指令輸入在anaconda prompt即可)
![image](https://user-images.githubusercontent.com/79627981/232783335-a1e5de7d-9619-4b60-932c-199ffbc60f07.png)
## 
## YOLOV5 訓練及測試
### Step1: 在anaconda promopt內輸入 pip install labelImg 安裝labelimg，並執行
![image](https://user-images.githubusercontent.com/79627981/232785308-a62050f9-4adf-4093-bdfb-fb614f42fe98.png)
### Step2: 開始對影像進行標籤
![image](https://user-images.githubusercontent.com/79627981/232785817-6fcdb5fe-7458-4de7-9329-86d134afba55.png)
![image](https://user-images.githubusercontent.com/79627981/232786720-a93d659a-cc60-44e7-8b7e-c43d61000aa9.png)
### Step3: 建立一個mydataset.yaml檔案 ，並在裡面輸入訓練集、驗證集位置、標籤種類及數量
![image](https://user-images.githubusercontent.com/79627981/232788257-e60698c2-dee7-402c-8af2-d51c2f8985a3.png)
### Step4: 在train.py中調整各個訓練所要的參數、權重檔
![image](https://user-images.githubusercontent.com/79627981/232789148-c03743c3-89a8-4243-9876-16b236235f38.png)
## 訓練結果
![image](https://user-images.githubusercontent.com/79627981/232789673-cb11b764-13aa-499b-b104-85a7242820bc.png)
![image](https://user-images.githubusercontent.com/79627981/232789807-437f7a30-059c-4a8a-a82a-eb6450d3bb94.png)
![image](https://user-images.githubusercontent.com/79627981/232789878-64dbcb9a-0663-4265-9882-5a8181c7b6aa.png)
### Step5: 在detect.py中使用訓練完的權重檔(--weights)、輸入要測試的影像位置(--source)、輸出位置(--project)
![image](https://user-images.githubusercontent.com/79627981/232790624-76c2c5de-ad53-4bbb-8a3f-6cc82124b7a3.png)
### Step6: 進行訓練
![image](https://user-images.githubusercontent.com/79627981/232791112-e54f71d9-7e00-4dbc-bc5d-519bc5d32f4e.png)
##輸出結果
![image](https://user-images.githubusercontent.com/79627981/232791568-22336ac1-8db2-46ac-a5b5-7340d3d6b59a.png)
![image](https://user-images.githubusercontent.com/79627981/232791619-3bc7a0ca-c705-42c1-96ad-910310f33fc2.png)
