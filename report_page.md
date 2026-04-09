Họ tên: Nguyễn Văn Tiến | MSSV: 1771040025.
Mình thiết lập môi trường học phần trên Windows 10 bằng conda với Python 3.10.9.
Mình cài dependency bằng requirements.txt và xác nhận Torch version: 2.11.0+cpu.
Mình chạy check_env.py để kiểm tra import, phiên bản thư viện và lưu log ở outputs/logs/env_check.txt.
Mình chạy run_smoke_test.py với configs/smoke_test.yaml để test nhanh pipeline train.
Kết quả tạo đủ outputs/logs/smoke_test_log.txt, outputs/figures/loss_curve.png và outputs/checkpoints/smoke_model.pt.
Thiết bị chạy: CPU Ryzen 5 5625U, GPU RTX 3050 Mobile (smoke test hiện tại chạy trên CPU).
Vấn đề ban đầu là thiếu pandas, pyyaml do nhầm interpreter; đã xử lý bằng cách cài lại đúng env rồi chạy lại thành công.
