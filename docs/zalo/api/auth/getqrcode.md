# Get QR Code

Lấy mã QR để đăng nhập

`Login Account → Get QR Code`

### Credentials account

- **Zalo Credentials hoặc Select a custom credentials ID**: dùng credential hoặc session đã lưu để đăng nhập Zalo
- **Replace the Credential in all workflows**: Update the latest credentials for nodes currently using outdated credentials. Gợi ý: tự động sửa lại các ID credentials cũ thành mới (lưu workflow này và f5 ngay sau login)

### Conversation

- **Chat ID (bắt buộc)**: Telegram chat_id to send notifications to

### Options

- **Notifications to Telegram**: Whether to send QR code, status, error login, trigger to Telegram

### Parameters

- **Proxy**: HTTP proxy to use for Zalo API requests (proxy can only be saved once for a custom credential)
- **Bot Token (bắt buộc)**: The token for your Telegram bot

### Hướng dẫn

1. Chọn đúng resource và operation.
2. Nhập các trường cần thiết theo mô tả.
3. Test node với dữ liệu mẫu để kiểm tra output.
