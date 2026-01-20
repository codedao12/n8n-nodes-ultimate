# Zalo Bot Trigger

Nhận sự kiện webhook từ Zalo Bot.

### Credentials account

- **Zalo Bot Credential**: token và base URL của Zalo Bot API.

### Lưu ý

- Trigger tự động đăng ký lại webhook khi kích hoạt.
- Để Execute Step, hãy tạm unpublish workflow.
- Mỗi bot chỉ nên dùng một trigger để tránh xung đột webhook.

### Hướng dẫn

1. Cấu hình Zalo Bot Credential.
2. Kích hoạt workflow để webhook được đăng ký.
3. Gửi thử sự kiện để kiểm tra output.
