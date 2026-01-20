# Ví dụ

### Cấu hình nhanh

#### Tạo credential
- Vào **Credentials** trong n8n.
- Chọn loại credential phù hợp (Zalo User, Zalo Bot, Facebook User, n8n API).
- Lưu lại.

#### Thử node đơn giản
- Kéo node bất kỳ vào workflow (tương ứng loại credentials).
- Chọn credential vừa tạo.
- Chạy thử với dữ liệu mẫu.

#### Bật trigger (nếu có)
- Node trigger cần được kích hoạt và chạy liên tục.
- Kiểm tra output theo từng sự kiện.

### Ví dụ: Zalo User (unofficial) gửi tin nhắn chăm sóc khách hàng

- Dùng `Message → Send Message` để gửi lời nhắc đơn hàng hoặc phản hồi nhanh.
- Chọn đúng `threadType` (User/Group) và nhập `threadId` từ trigger hoặc kết quả tìm kiếm.
- Nếu có đính kèm (ảnh hóa đơn/video hướng dẫn), chọn `Attachment` và nhập `Attachment: URLs` hoặc `Attachment: File Paths`.

### Ví dụ: Zalo Trigger + Message Debounce gom nhiều tin nhắn

- Zalo Trigger lắng nghe hội thoại, ví dụ khách gửi liên tục nhiều câu ngắn.
- Message Debounce gộp thành một output để xử lý AI/trả lời tự động mượt hơn.
- Đặt `Wait Time (Seconds)` phù hợp (vd 8–12s) để tránh cắt câu.

### Ví dụ: Facebook User (unofficial) gửi tin nhắn cho khách ở Messenger

- Dùng `Message → Send Message` để trả lời inbox sau khi có lead.
- Nhập `threadId` và `Message`, có thể kèm `Attachment URL(s)` nếu gửi file.
