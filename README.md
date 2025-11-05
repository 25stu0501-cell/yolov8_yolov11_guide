# yolov8_yolov11_guide
# 🦾 YOLOv11 사용법 및 YOLOv8 비교 정리

이 문서는 **Ultralytics YOLOv11** 모델의 사용법을 정리하고,  
이전 버전인 **YOLOv8**과의 차이점을 한눈에 비교할 수 있도록 구성되었습니다.  

---

## 🚀 YOLOv11 설치 및 기본 사용법

```bash
# 1️⃣ YOLOv11 설치
pip install ultralytics

# 2️⃣ 사전 학습된 모델 불러오기 및 예측 실행
yolo predict model=yolo11n.pt source='image.jpg'
