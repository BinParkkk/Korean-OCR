# OCR-yolov5-SwinIR-STARNet
OCR(Korean) 한국어 메뉴판 OCR
   
   

* 기존 프로젝트 이후 개선 방향

  * ~~메뉴판 디텍션 이후에 다시 다른 한글 디텍션 (2stage)~~   
     * **느린 속도 Detection 속도로 인해 가벼운 모델 사용 필요**
  * ~~세로로 되어있는 한글 Detection~~
  * 세로로 되어있는 한글 Recognition
  * 기울어진 메뉴판 인식
  * 성능 향상

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

* 간판 (weight 루트값 수정 필요)   

![화면 캡처 2022-07-01 132858](https://user-images.githubusercontent.com/106142675/176823623-75577035-8665-422f-98d6-e2c7ef6a6585.png)      ![화면 캡처 2022-07-01 132914](https://user-images.githubusercontent.com/106142675/176823644-3c561dd8-2f12-4491-becf-27a649b7b623.png)

![화면 캡처 2022-07-01 132928](https://user-images.githubusercontent.com/106142675/176823718-f1feb1e7-1b06-470a-9953-504434193c87.png)
![화면 캡처 2022-07-01 132943](https://user-images.githubusercontent.com/106142675/176823734-b1041d80-7b77-4e39-89b4-447fc23dc0f5.png)

* 메뉴판 Detection
![1](https://user-images.githubusercontent.com/106142401/191195493-8da35a6a-92ab-4041-956e-9113ccc8992c.jpg) ![11](https://user-images.githubusercontent.com/106142401/191195532-952041ff-c7b2-43dc-a06a-4f5ef7267128.jpg)   
   
![4](https://user-images.githubusercontent.com/106142401/191195583-cd74dfd8-af17-4141-aea9-f8a878f675d4.jpg) ![42](https://user-images.githubusercontent.com/106142401/191195628-c5600bcc-522a-4afd-8564-993cb006a173.jpg)

* 메뉴판 end-to-end
![3](https://user-images.githubusercontent.com/106142401/191196228-c15bc725-90e0-4c18-b6c7-4b1feada7ac9.jpg)
![458da880-d56e-4130-bdea-68d68672e9ac](https://user-images.githubusercontent.com/106142401/191196262-c6e597bd-d28f-4332-92f5-d1c8643b17d7.jpg)




Reference
---------------------------------------------------------------------
- https://github.com/jingyunliang/swinir
- https://github.com/clovaai/deep-text-recognition-benchmark
- https://github.com/aqntks/Easy-Yolo-OCR
- https://github.com/ultralytics/yolov5
