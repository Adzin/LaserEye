# 如何用視線偵測玩pygame

### 使用的模型:

此範例所需使用的模型有:

  * `face-detection-adas-0001`
  * `head-pose-estimation-adas-0001`
  * `facial-landmarks-35-adas-0002`
  * `gaze-estimation-adas-0002`

此模型可以從 OpenVINO 中的 Open Model Zoo 找到 [Open Model Zoo](https://github.com/opencv/open_model_zoo).


## 如何執行


### 0. 必要套件
- **OpenVINO 2020.1**
  - 如果還沒安裝OpenVINO 可以參考OpenVINO官網或是到 [*Get Started*](https://software.intel.com/en-us/openvino-toolkit/documentation/get-started)中參考.  

### 1. 安裝相關套件  
此遊戲需要:
- `numpy`
- `scipy`
- `opencv-python`
- `pygame`

### 2. 下載模型
如果要下載模型可使用OpenVINO中的下載器
``` sh
(Win10) python "%INTEL_OPENVINO_DIR%\deployment_tools\tools\model_downloader\downloader.py" --list models.lst
```

### 3. 執行程式
首先要將USB webCam安裝到電腦上，建議使用 Anaconda 開一個新環境使用

``` sh
(Win10) python gaze-estimation.py
```

## 測試環境
- Windows 10 
- Intel(r) Distribution of OpenVINO(tm) toolkit 2020.1  
- Python 3.6
