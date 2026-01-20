# Zalo Trigger

Lắng nghe sự kiện đến trên Zalo cá nhân (multiple users).

### Credentials account

- **Zalo Credentials hoặc Select a custom credentials ID**: dùng credential hoặc session đã lưu để đăng nhập Zalo

### Parameters
- **Trigger On (bắt buộc)**: Các sự kiện muốn lắng nghe
- **Auto Restart (Hours)**: Tự động khởi động lại kết nối sau mỗi x giờ giúp ổn định (0=tắt, không khởi động lại workflow/n8n)
- **Media Debounce**: Gộp nhiều ảnh/video gửi cùng lúc thành 1 sự kiện (chờ tối đa 10s, không khả dụng với Execute test)
- **Use Filtered Output**: Chuẩn hóa kết quả trong `filter` để dễ dùng
- **Filtering Thread IDs**: Lọc theo thread ID (không khả dụng với Execute test)
- **Allowed Thread IDs**: Chỉ lắng nghe tin nhắn từ các thread ID này (phân cách bằng dấu phẩy). Để trống = lắng nghe tất cả
- **Blocked Thread IDs**: Bỏ qua tin nhắn từ các thread ID này (phân cách bằng dấu phẩy)
- **Filtering Keyword**: Lọc tin nhắn theo từ khóa (không khả dụng với Execute test)
- **Listen Only Keywords**: Chỉ lắng nghe tin nhắn chứa ít nhất một trong các từ khóa này (phân cách bằng dấu phẩy, bỏ qua từ khóa 1 ký tự)
- **Ignore Keywords**: Bỏ qua tin nhắn chứa bất kỳ từ khóa nào trong danh sách này (phân cách bằng dấu phẩy, bỏ qua từ khóa 1 ký tự)
- **Continue On Login Fail**: Tiếp tục active workflow khi có 1 Zalo Trigger lỗi
- **Telegram Bot Token**: Bot token để thông báo khi trigger lỗi (để trống nếu credential đã có)
- **Telegram Chat ID**: ID nhóm chat để thông báo khi trigger lỗi (để trống nếu credential đã có)
- **Self Listen (bắt buộc)**: Lắng nghe các sự kiện do chính bạn thực hiện
- **Self Messages Only**: Khi Self Listen chỉ nhận sự kiện User/Group Message (không khả dụng với Execute test)

### Trigger On gồm các sự kiện

- User Messages
- Group Messages
- Group Event
- Friend Event
- Undo
- Typing
- Reaction
- Seen Message

### Lưu ý

- Không thể có 2 trigger cho cùng 1 account.
- Đây không phải API chính thức của Zalo nên có thể mất một vài gói tin.
- Khi bật Media Debounce, output `filter` sẽ có `msgType`, `href_photo`, `href_video`.
- Có cơ chế tự ổn định và kết nối lại để hạn chế mất kết nối.
- Có thể dùng Telegram Bot Token để nhận QR và cảnh báo lỗi.

### Hướng dẫn

1. Chọn đúng Trigger On cần lắng nghe.
2. Cấu hình các tuỳ chọn lọc/điều kiện nếu cần.
3. Test trigger với dữ liệu mẫu để kiểm tra output.
