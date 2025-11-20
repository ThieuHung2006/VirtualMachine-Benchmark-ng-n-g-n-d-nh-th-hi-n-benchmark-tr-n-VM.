# VirtualMachine-Benchmark

## Mục tiêu
Thực hiện benchmark hiệu năng CPU, RAM và ổ cứng trên môi trường ảo (VirtualBox + Ubuntu 22.04) để phân tích ảnh hưởng của các linh kiện đến hiệu năng tổng thể hệ thống.

## Công cụ sử dụng
- **OS:** Ubuntu 22.04 (trên VirtualBox)
- **CPU/RAM Benchmark:** sysbench
- **Ổ cứng Benchmark:** dd
- **Phân tích:** Ghi nhận và so sánh kết quả

## Cấu hình thử nghiệm mẫu
- CPU: 2 cores (không Hyper-Threading)
- RAM: 4 GB
- Disk: Virtual Disk 20 GB

## Hướng dẫn chạy benchmark

### CPU Benchmark
```bash
sudo apt update
sudo apt install sysbench -y
sysbench cpu --threads=2 run
