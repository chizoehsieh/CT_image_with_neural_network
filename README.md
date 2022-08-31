# A trial of multiple neural networks reflecting the results of COVID-19 CT image processing

## 研究背景
嚴重特殊傳染性肺炎疫情（COVID-19）在2019年末於中華人民共和國湖北省武漢市首次被發現，隨後在2020年初迅速擴散至全球多國，逐漸變成一場全球性大瘟疫。

本研究透過肺部CT影像分析是否有感染COVID-19，CT影像可用於判斷患者是否感染病毒性肺炎（COVID-19是一種由SARS-CoV-2病毒引起的病毒性肺炎）。但是CT 無法確定導致病毒性肺炎的病毒是 SARS-CoV-2 還是其他病毒。\
嚴格來說，CT 不能用於確認患者是否感染了 COVID-19。 然而在疫情爆發期間，大多數病毒性肺炎是由 SARS-CoV-2 引起的。也就是說，如果患者根據CT結果確診為病毒性肺炎，這種病毒性肺炎極有可能是COVID-19。

本研究參考"Medical Image Processing and Deep Learning to Diagnose COVID-19 with CT Images"。

## 資料集
本研究使用來自Github上的開源資料集，該數據集的實用性已得到中國武漢同濟醫院的一名高級放射科醫生的證實可用性。

資料集內包含349筆確診病患的肺部CT影像，和397筆未確診的肺部CT影像圖。\
我們先將圖片重整成224 x 224像素大小，再打亂資料順序後，以8 : 2的比例切割成訓練和測試資料集。

## 資料前處理
1. 二值化處理
2. 直方圖等化
3. 中值濾波
4. 局部拉普拉斯濾波

## 特徵擷取
1. 局部二值模式
2. 灰度共生矩陣

## 使用的深度學習模型
1. Inception V3
2. VGG-19
3. ResNet50
4. Xception
5. DenseNet169

## 結論
![image](https://user-images.githubusercontent.com/88066658/187683684-95419455-54db-4eaf-9aa0-bbd46828d9aa.png)


### 工作分配
  - **謝奇容**    影像前處理、特徵擷取、ppt製作
  - 王采筑    模型設計、文件撰寫、ppt製作



