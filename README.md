# AIoT Lab6 Team 2

## 在 Raspberry Pi 4 上實作 Lab2 及 Lab3


---

## 實驗步驟

1. Raspberry Pi 4 刷機
    - 到[Raspberry Pi Imager](https://www.raspberrypi.com/software/)下載匹配自己作業系統之版本
        - 開啟Raspberry Pi Imager，點選對應Raspberry Pi OS安裝之版本
            - Operating system：Raspberry Pi OS(64bits)
            - Raspberry Pi Device:Raspberry Pi 4
            - Storage: xxxx Media(MicroSD)
        - 將MicroSD卡放置到Rpi4**背面**，並接上電源線、螢幕連接線、鍵盤、滑鼠後，開機
    - 開機後，會進行一系列初始化設定（設定名稱、密碼、時區等資訊）
    - 將Rpi4連接到網際網路（建議個人熱點，較穩定）

2. Arduino IDE 安裝（可參考Lab2,3教材，此部分簡略說明）
    - 下載所需之環境
        - Environment:Arduino IDE
        - Board manger:ESP32manger
        - Library:DHT11
        - 修改對應的網路資訊（SSID、Password、ServerIP）
    - [在rpi4安裝Arduino IDE bash file SetupArduinoIDE.sh](./SetupArduinoIDE.sh)

3. 運行Flask server
    - 在終端機中執行`app.py`啟動server
    - 從Console中確認資料是否正確傳輸到rpi4之server

