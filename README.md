# edge-traffic — Đèn giao thông thích ứng xử lý tại biên

Mô hình IoT ngã tư 4 hướng: các máy nhúng tại mỗi hướng dùng camera đếm xe đang chờ,
gửi dữ liệu về máy mẹ để tự điều chỉnh thời gian đèn xanh.

So sánh 2 kiến trúc:
- Kiến trúc 1: Raspberry Pi tự xử lý ảnh tại chỗ (biên), chỉ gửi số xe về Jetson Nano.
- Kiến trúc 2: Raspberry Pi gửi hình về, Jetson Nano xử lý tập trung.

## Thiết bị
- 1 Jetson Nano 4 GB: máy mẹ, kiêm hướng Bắc
- 3 Raspberry Pi 3B: máy con, hướng Đông, Nam, Tây
- 4 camera, 4 cụm đèn LED đỏ/vàng/xanh

## Tiến độ
- [ ] Phần 1: Thiết lập công cụ