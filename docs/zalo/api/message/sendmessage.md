# Send Message

Gửi tin nhắn bình thường (ảnh, @tag, quote).

`Message → Send Message`

### Credentials account

- **Zalo Credentials** hoặc **Select a custom credentials ID**: dùng credential hoặc session đã lưu để đăng nhập Zalo

### Conversation

- **Type**: chọn loại cuộc trò chuyện cần tương tác (người dùng hoặc nhóm)
- **Thread ID**: ID của người dùng hoặc nhóm cần thao tác

### Message

- **Message**: nội dung tin nhắn cần gửi (có thể trống để gửi Attachment)
  - **Format**: gửi tin nhắn dạng thường hoặc HTML.
    - HTML hỗ trợ: `b`, `i`, `u`, `s`, `small`, `big`, `red`, `orange`, `yellow`, `green`, `br`, `ul`, `li`.
    - Ví dụ: `Xin chào <b>Codex</b><br/>Cảm ơn!`
  - **Urgency**: mức độ khẩn cấp của tin nhắn (giao diện Web/Desktop)
  - **Send \"Typing...\" Event**: gửi trạng thái "Đang soạn tin..." trước khi gửi

### Attachment

- **Attachment**: chọn nguồn file đính kèm (Ảnh, Video, File...)
  - **Mode**: chọn loại file, Auto sẽ dựa vào đuôi file
  - **URLs**: nhập url file (url hoặc url1,url2,...). Ví dụ: `https://.../img1.jpg, https://.../img2.png`
  - **File Paths**: nhập đường dẫn file trên server (path hoặc path1,path2,...). Ví dụ: `/home/node/.n8n/files/img1.jpg`
  - **File Name**: tên file (kèm đuôi) để gửi
  - **Input Binary Field**: tên file binary của node trước

### Mentions

- **Mentions**: tag tên người dùng hoặc tag @all.
  - `@all`: tag cả nhóm.
  - `userId1,userId2`: tag từng người dùng theo userId.
  - **Position**: chọn vị trí mentions là `start` hoặc `end` (nếu tag nhiều hoặc dùng HTML nên chọn `end`).

### Reaction

- **Reaction**: thả biểu tượng cảm xúc sau khi gửi tin nhắn

### Quote

- **Quote Message**: trích dẫn tin nhắn (yêu cầu `msgId`, `cliMsgId`)

### Styles

- **Text Styles**: định dạng text với các style khác nhau (dùng HTML format sẽ dễ hơn)

### TTL

- **TTL**: 0 = vĩnh viễn, thời gian tồn tại của tin nhắn (giây)

### Hướng dẫn

1. Chọn đúng resource và operation.
2. Nhập các trường cần thiết theo mô tả.
3. Test node với dữ liệu mẫu để kiểm tra output.
