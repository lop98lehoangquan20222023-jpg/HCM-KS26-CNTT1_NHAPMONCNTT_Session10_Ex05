# PHẦN 1. PHÂN TÍCH HỆ THỐNG SMART-FARM
## 1. Phân tích Input / Output (Mô hình IPO)
Input (Đầu vào): Các con số do cảm biến gửi về (độ ẩm đất khô/ẩm, nhiệt độ không khí nóng/mát) và nút bấm điều khiển.

Process (Xử lý - Bộ não ESP32): Nhận số liệu từ cảm biến, so sánh với mức chuẩn (ví dụ: đất dưới 50% độ ẩm là khô) rồi quyết định có bật máy bơm hay không.

Output (Đầu ra): Bật/tắt máy bơm nước, bật quạt làm mát, hiển thị con số lên màn hình OLED.
# PHẦN 2. TRIỂN KHAI TÀI LIỆU
# 🚀 Smart-Farm: Hệ Thống Tưới Lan Tự Động
## 📋 1. Mô tả dự án
Dự án **Smart-Farm** được làm ra để giúp người nông dân chăm sóc **Trang trại Lan** dễ dàng hơn. 
---

## ⚙️ 2. Hướng dẫn cài đặt
Mở màn hình dòng lệnh (Terminal) trên máy tính điều khiển và gõ 4 câu lệnh sau:

```bash
# Bước 1: Cập nhật phần mềm hệ thống
sudo apt-get update

# Bước 2: Tải mã nguồn chương trình Smart-Farm về máy
git clone [https://github.com/smart-farm/orchid-iot-system.git](https://github.com/smart-farm/orchid-iot-system.git)

# Bước 3: Di chuyển vào thư mục dự án
cd orchid-iot-system

# Bước 4: Chạy chương trình ở chế độ tự động
python3 main.py --mode=auto
```