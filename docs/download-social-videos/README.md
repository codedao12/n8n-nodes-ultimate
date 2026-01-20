# codedao12 - Download Social Videos

Tải video từ TikTok, YouTube, Facebook Reels.

### Credentials account

- **Facebook User API Credential**: cần khi tải Facebook Reels.

### Parameters

- **Resource**: nền tảng cần tải (TikTok, YouTube, Facebook...).
- **Operation**: Download hoặc Get Info (JSON).
- **Mode**: chọn nhập URL hoặc theo Username/Channel.
- **URL**: link video cần tải.
- **Username / Channel ID**: tên người dùng hoặc ID kênh để quét video mới nhất.
- **Download Playlist/Mix?**: bật để tải toàn bộ playlist/mix.
- **Max Videos (Limit)**: số lượng video tối đa.
- **Sleep (Seconds)**: thời gian nghỉ giữa các lần tải.
- **Format**: định dạng tải (Best/Medium/Low/Audio/Custom).
- **Custom Format String**: chuỗi định dạng khi chọn Custom.
- **Output Folder**: thư mục lưu file tải về.
- **Avoid Duplicate Downloads**: bỏ qua video đã tải trước đó.

### Lưu ý

- Cần cài `python3` và `ffmpeg` để tải đầy đủ nền tảng và chất lượng.
- Khi tải Reels, cần cookies nên phải cấu hình Facebook User API Credential.
- Hỗ trợ tải theo URL hoặc theo kênh/tài khoản, phù hợp Shorts/TikTok/Reels.

### Ví dụ cấu hình Dockerfile (tự host)

```dockerfile
FROM n8nio/n8n:latest

USER root
RUN apk add --no-cache python3 ffmpeg
USER node
```

### Ví dụ cấu hình Dockerfile (Debian/Ubuntu)

```dockerfile
FROM n8nio/n8n:latest

USER root
RUN apt-get update && apt-get install -y python3 ffmpeg && rm -rf /var/lib/apt/lists/*
USER node
```
