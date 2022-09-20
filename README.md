# OCR-yolov5-SwinIR-STARNet
OCR(Korean) 한국어 메뉴판 OCR
   
   

* 기존 프로젝트 이후 개선 방향

  * ~~메뉴판 디텍션 이후에 다시 다른 한글 디텍션 (2stage)~~
  * 세로로 되어있는 한글 학습
  * 기울어진 메뉴판 인식

## Run demo

- Requirement
```
!pip install timm
```

- Run demo.py
```
!CUDA_VISIBLE_DEVICES=0 python3 demo.py --image_folder /content/OCR-yolov5-SwinIR-STARNet/img_demo
```
- Result : The result will be saved in './results'

![화면 캡처 2022-07-01 132858](https://user-images.githubusercontent.com/106142675/176823623-75577035-8665-422f-98d6-e2c7ef6a6585.png)      ![화면 캡처 2022-07-01 132914](https://user-images.githubusercontent.com/106142675/176823644-3c561dd8-2f12-4491-becf-27a649b7b623.png)

![화면 캡처 2022-07-01 132928](https://user-images.githubusercontent.com/106142675/176823718-f1feb1e7-1b06-470a-9953-504434193c87.png)
![화면 캡처 2022-07-01 132943](https://user-images.githubusercontent.com/106142675/176823734-b1041d80-7b77-4e39-89b4-447fc23dc0f5.png)

Reference
---------------------------------------------------------------------
- https://github.com/jingyunliang/swinir
- https://github.com/clovaai/deep-text-recognition-benchmark
- https://github.com/aqntks/Easy-Yolo-OCR
- https://github.com/ultralytics/yolov5
