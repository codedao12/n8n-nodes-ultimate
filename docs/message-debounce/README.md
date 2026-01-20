# Message Debounce

Chờ tin nhắn từ trigger, gộp lại và trả sau thời gian chờ.

### Parameters

- **Mode**: Zalo dùng key mặc định cho trigger Zalo; Custom cho phép chỉ định key/content từ JSON.
- **Wait Time (Seconds)**: thời gian chờ gom tin nhắn tiếp theo (tối đa 60s).
- **Max Batched Messages**: số tin nhắn gộp tối đa (tối đa 10).
- **Separator**: ký tự nối các tin nhắn (mặc định là xuống dòng).

### Zalo Mode

- **Ignore IsSelf**: bỏ qua tin nhắn của chính mình (tắt có thể gây vòng lặp).
- **Extract Text From Photo/Video**: gom text trong ảnh/video (nếu có) và đặt `data.content.title` = "".
- **Content Fields**: đường dẫn tới nội dung cần gom, mặc định `data.content`.

### Custom Mode

- **Key Fields**: danh sách field tạo key duy nhất, ví dụ `id,userId,type`.
- **Content Fields**: đường dẫn tới nội dung cần gom, ví dụ `data.content` hoặc `payload.text`.
- **Drop When Path is true (boolean)**: nếu path trả về `true` thì bỏ qua item (ví dụ `isSelf`).

### Lưu ý

- Node sẽ reset thời gian chờ nếu có tin mới và chỉ trả output khi hết thời gian chờ.
- Ví dụ tạo key: `id,data.uid` và lấy nội dung `data.text` từ JSON.
- Dùng được cho mọi nền tảng có trigger (không chỉ Zalo/Facebook).
