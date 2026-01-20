# Upload Attachment

Upload file để lấy thông tin (fileUrl, photoId, fileId...)

`Attachment → Upload Attachment`

### Credentials account

- **Zalo Credentials hoặc Select a custom credentials ID**: dùng credential hoặc session đã lưu để đăng nhập Zalo

### Conversation

- **Type**: Chọn loại cuộc trò chuyện cần tương tác (người dùng hoặc nhóm)
- **Thread ID (bắt buộc)**: ID của người dùng hoặc nhóm cần thao tác

### Attachment

- **Source Type**: loại nguồn dữ liệu
- **Upload Mode**: Auto dựa theo extension (chỉ dùng cho File Path / URL). Gợi ý: video/voice/file thường được zalo định dạng kiểu gửi tệp
- **File Name**: Nhập để phân biệt định dạng file (nếu để trống mặc định jpg, mp4)

### Options

- **Return Partial Result On Timeout**: Quá thời gian trả về kết quả tạm thay vì báo lỗi.

### Hướng dẫn

1. Chọn đúng resource và operation.
2. Nhập các trường cần thiết theo mô tả.
3. Test node với dữ liệu mẫu để kiểm tra output.
