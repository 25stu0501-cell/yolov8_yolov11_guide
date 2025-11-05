# yolov8_yolov11_guide
# 🦾 YOLOv11 실습 및 정리

이 문서는 **YOLOv11(Object Detection)** 모델 실습을 위한 정리 자료입니다.  
YOLOv11은 Ultralytics에서 개발한 YOLOv8의 후속 버전으로,  
더 빠르고 정확한 객체 탐지를 제공합니다.

---

## 🚀 YOLOv11 설치 및 기본 사용법

```bash
# 1️⃣ YOLOv11 설치
pip install ultralytics

# 2️⃣ 사전 학습된 모델 불러오기 및 예측 실행
yolo predict model=yolo11n.pt source='image.jpg'
from ultralytics import YOLO

# 모델 불러오기
model = YOLO("yolo11n.pt")

# 이미지 예측
results = model("image.jpg")

# 결과 보기
results.show()

# 결과 저장
results.save("runs/detect/")
# 🦾 YOLOv11 모델 다운로드 & 성능 정리

이 문서는 Ultralytics YOLOv11 모델의 다운로드 링크와 성능 정보를 정리한 것입니다.  
모델 이름을 클릭하면 **.pt 파일이 자동으로 다운로드**됩니다.

---

## 📥 모델 다운로드

| 모델 | 크기 (픽셀) | mAP<sub>val</sub> 50–95 | 속도 (CPU ONNX) | 파라미터 (M) | FLOPs (B) | 다운로드 |
|------|-------------|--------------------|------------------|---------------|------------|-----------|
| **YOLO11n** | 640 | 39.5 | 56.1 ± 0.8ms | 2.6 | 6.5 | 🔽 [Download](https://github.com/ultralytics/assets/releases/download/v0.0.0/yolo11n.pt) |
| **YOLO11s** | 640 | 47.0 | 90.0 ± 1.2ms | 9.4 | 21.5 | 🔽 [Download](https://github.com/ultralytics/assets/releases/download/v0.0.0/yolo11s.pt) |
| **YOLO11m** | 640 | 51.5 | 183.2 ± 2.0ms | 20.1 | 68.0 | 🔽 [Download](https://github.com/ultralytics/assets/releases/download/v0.0.0/yolo11m.pt) |
| **YOLO11l** | 640 | 53.4 | 238.6 ± 1.4ms | 25.3 | 86.9 | 🔽 [Download](https://github.com/ultralytics/assets/releases/download/v0.0.0/yolo11l.pt) |
| **YOLO11x** | 640 | 54.7 | 462.8 ± 6.7ms | 56.9 | 194.9 | 🔽 [Download](https://github.com/ultralytics/assets/releases/download/v0.0.0/yolo11x.pt) |

> 💡 **링크 클릭 시** 자동으로 `.pt` 파일이 다운로드됩니다.  
> 위 링크는 Ultralytics 모델이 호스팅되는 GitHub Release 경로입니다.

---

## 🚀 설치 및 실행 예시

```bash
# 1️⃣ YOLOv11 설치
pip install ultralytics

# 2️⃣ 모델 다운로드 후 예측 실행
yolo predict model=yolo11n.pt source='image.jpg'
<img width="856" height="349" alt="image" src="https://github.com/user-attachments/assets/66087d28-773c-4bb4-9896-2b6b8f575eb2" />
