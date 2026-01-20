# Send Message

Gửi tin nhắn (user).

`Message → Send Message`

### Conversation

- **Thread ID (bắt buộc)**: ID của người dùng hoặc nhóm chat.

### Message

- **Message**: nội dung tin nhắn văn bản (tuỳ chọn).
  - **Reply To Message ID**: ID tin nhắn cần trả lời (tuỳ chọn).
  - **Sticker ID**: ID sticker để gửi (tuỳ chọn).

### Attachment

- **Attachment Type**: chọn cách gửi file.
  - **Binary Property Name(s)**: tên binary property (có thể nhiều, cách nhau bằng dấu phẩy).
  - **File Path(s)**: đường dẫn file (có thể nhiều, cách nhau bằng dấu phẩy).
  - **Attachment URL(s)**: URL file (có thể nhiều, cách nhau bằng dấu phẩy).

### Options

- **Is Single User**: dùng userId khi chat 1-1 (không khả dụng do mã hoá đầu cuối).

### Hướng dẫn

1. Chọn đúng resource và operation.
2. Nhập các trường cần thiết theo mô tả.
3. Test node với dữ liệu mẫu để kiểm tra output.
