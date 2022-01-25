# public_ocr


Pytorch를 사용한 공공행정문서 OCR 실행 코드
## Pipeline


![image](https://user-images.githubusercontent.com/46219219/150891274-467d1d04-d53b-47ce-88f5-52d1abe523bd.png)

## Requirments
- Cython
- matplotlib>=3.2.2
- numpy>=1.18.5
- opencv-python>=4.1.2
- pillow
- PyYAML>=5.3
- scipy>=1.4.1
- tensorboard>=2.2
- torch>=1.6.0
- torchvision>=0.7.0
- tqdm>=4.41.0
- lmdb
- nltk
- natsort

## Pretrained
|모델|링크|
|------|---|
|detection|[pretrained](https://o365hansung-my.sharepoint.com/:f:/g/personal/gs3071_hansung_edu/EtufZdMj9hpLmAnCHh0ixaoBoG7mg6fevtvETi_jMBdm_g?e=cIgwTg)|
|recogntion|[pretrained](https://o365hansung-my.sharepoint.com/:f:/g/personal/gs3071_hansung_edu/Em0UPM2e_m9KmwQEbLeSeJ8BEWI43ewudS6sKgoMAf46Lg?e=nDWQRI)|


## How to use
1. weight 파일에 pretrained 모델 다운
2. img 폴더 안에 OCR할 파일 첨부
3. main.py 실행
4. log_result.txt에 OCR 내용 저장됨

## Result
Text detection 결과
![1](https://user-images.githubusercontent.com/46219219/150907618-905fb374-33d5-421e-86be-23f76a668c06.jpg)

Text Recognition 결과

                    
미검증 교육혁신을 념어 미래교육으로 경상남도교육청 하동도서관  경남교육 수신 내부결재 (경유) 제목 [2020-11-201 세입세출외현금수입일계」 세입세출외현금 수입일계는 아래와 같습니다. 1. 수납일자 :2020-11-20 2. 수납건수: 3. 수납금액 85,000원 붙임 세입세출외현금 수입일계. 끝. 2020 11.21. ★행정실장 민재선 관장 노광석 협조자 경상남도교육청 하동도서관 시행 ) 접수 ( ) -3647 우 52332 경상남도 하동군 하동읍 경서대로 80(하동읍) / http:/hdiib.gnae.go.kr 전화 884-7985 /전송 055-882-5958 / 부분공개(6) 물길과 물길과 미래의 갖을 멸치는 행복도서관

score : 0.8901


## To-Do List


- [ ] try-except를 통해 오류 발생시 프로그램 멈춤 현상 방지
- [ ] 안쓰이는 파일 제거
- [ ] json 출력
- [ ] 내용 첨부
- [ ] 리팩터링
- [ ] 로그 파일 출력 내용 수정
- [ ] README.md 내용 추가

## Reference


- [Yolov5](https://github.com/ultralytics/yolov5)
- [deep-text-recognition-benchmark](https://github.com/clovaai/deep-text-recognition-benchmark)
- [aihub-공공행정문서OCR](https://aihub.or.kr/aidata/30724)
