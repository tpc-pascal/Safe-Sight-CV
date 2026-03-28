# Safe-Sight-CV

<div align="center">
  <img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white" alt="python">
  <img src="https://img.shields.io/badge/PyTorch-EE4C2C?style=for-the-badge&logo=pytorch&logoColor=white" alt="pytorch">
  <img src="https://img.shields.io/badge/YOLOv5-00FFFF?style=for-the-badge&logo=ultralytics&logoColor=black" alt="yolov5">
</div>

<br />

**Safe-Sight-CV** là một giải pháp thị giác máy tính (Computer Vision) hiệu năng cao, được thiết kế để bảo vệ trẻ em khỏi các nội dung không phù hợp trên thiết bị di động. Dự án tập trung vào việc nhận diện nội dung nhạy cảm (NSFW) theo thời gian thực và xử lý trực tiếp trên thiết bị (On-device) để đảm bảo quyền riêng tư tuyệt đối.

---

## 🎉 Tác giả

[![Contributors](https://contributors-img.web.app/image?repo=tpc-pascal/Smart-Parking-System)](https://github.com/tpc-pascal/Smart-Parking-System/graphs/contributors)
<details open>
<summary><b>🔍 Các thành viên</b></summary>

| STT | Tên | MSSV | Vai trò |
|:---:|:---|:---|:---|
| 1 | Trịnh Phú Cường | 2380614500 | ... |
</details>

## 🚀 Tính năng chính

* **Nhận diện Real-time:** Tận dụng sức mạnh của YOLOv5 (Nano/Small) để đạt tốc độ xử lý tối ưu trên phần cứng di động.
* **Phân loại nội dung:** Tự động phân loại luồng hình ảnh thành `Safe` (An toàn) hoặc `Unsafe` (Nhạy cảm/NSFW).
* **Tối ưu hóa Mobile:** Quy trình chuyển đổi mô hình sang `.tflite` hỗ trợ Quantization (int8) để giảm dung lượng và tăng tốc độ.
* **Quyền riêng tư (Privacy-First):** Không truyền dữ liệu hình ảnh lên máy chủ, mọi quá trình tính toán (Inference) diễn ra 100% cục bộ.
* **Cảnh báo thông minh:** Hệ thống có khả năng kích hoạt lệnh khóa hoặc gửi thông báo khi phát hiện vi phạm.

## 🛠️ Công nghệ sử dụng

* **Model:** YOLOv5
* **Framework:** PyTorch
* **Language:** Python
* **Dataset:** COCODataSet

## 📂 Cấu trúc dự án

```text
Safe-Sight-CV/
├── data/
├── model/
│   ├── weapon-detection/
│   │   ├── result/
│   │   ├── Weapon.ipynb
│   │   ├── Weapon_detection.yaml
│   │   └── weapon-detection.pt
│   ├── MODEL.md
│   └── requirements.txt
├── .gitattributes
├── .gitignore
├── CONTRIBUTING.md
├── CREDITS.md
├── LICENSE
└── README.md
```
## 🚅 Bộ dữ liệu

Đọc thêm tại [TRAINING_DATASET.md](./data/training/TRAINING_DATASET.md) và [TESTING_DATASET.md](./data/testing/TESTING_DATASET.md)

## ✈ Hướng dẫn đóng góp

Đọc thêm tại [CONTRIBUTING.md](./CONTRIBUTING.md)

## 🙏 Nguồn tham khảo

Đọc thêm tại [CREDITS.md](./CREDITS.md)
