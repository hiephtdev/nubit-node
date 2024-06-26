# Hướng dẫn tạo system service duy trì Nubit light node
## System Requirements
| Component | Minimum | Recommended |
|-----------|---------|-------------|
| RAM | 2GB | 8GB |
| CPU (amd64/x86 architecture) | 1 core | 	4 core |
| Storage (SSD) | 20-40 GB | 200-300 GB |
**OS Recommended Ubuntu 22.04**

## Run Light Node
1. Run script
```bash
curl -sL1 https://nubit.sh
```
2. Đợi gen xong PUBKEY, nhấn Ctrl + C để hoàn thành node

3. Chạy lệnh bash dưới để tạo service
```bash
bash <(wget -qO- https://raw.githubusercontent.com/hiephtdev/nubit-node/main/light-node-service.sh)
```

4. Kiểm tra trang thái service -> Kết thúc
```bash
sudo systemctl status nubitlightd
```
