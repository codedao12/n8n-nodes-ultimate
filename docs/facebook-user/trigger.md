# Facebook User Trigger

Lắng nghe tin nhắn Messenger và thông báo Facebook cá nhân.

### Credentials account

- **Facebook User API Credential**: dùng để đăng nhập tài khoản Facebook.

### Messenger Events

- **Trigger On**: chọn các sự kiện cần lắng nghe (Message, Reply, Typing, Read Receipt, Unsend, Reaction, Presence).
- **Proxy**: proxy đăng nhập nếu cần (nên trùng với proxy đã dùng để lấy cookies).
- **Self Listen**: lắng nghe sự kiện do chính bạn thực hiện.
- **Auto Mark Read**: tự động đánh dấu đã đọc (khuyến nghị tắt khi test).
- **Reconnect Base Delay (s)**: thời gian chờ trước khi thử reconnect.
- **Auto Restart (h)**: tự kết nối lại nếu quá lâu không có event (0 = tắt).
- **Max Relogin Per Hour**: giới hạn số lần relogin để tránh checkpoint.

### Notifications

- **📣 Enable Notifications**: bật lắng nghe thông báo.
- **📢 Ignore Types**: bỏ qua một số loại thông báo.
- **📢 Interval (m)**: chu kỳ kiểm tra thông báo.
- **📢 Count**: số lượng thông báo tối đa cần lấy.
- **📢 Lookback Minutes**: lấy thông báo trong X phút gần nhất.
- **📢 Filter Tokens (comma separated)**: tuỳ chỉnh filter token (tuỳ chọn).
- **📢 Doc ID (Optional)**: tuỳ chọn doc id (để trống dùng mặc định).

### Lưu ý

- Chat 1-1 mã hoá đầu cuối có thể không nhận đủ sự kiện.
- Hạn chế spam để tránh checkpoint.
- Trigger có 2 output: `messenger` và `notification` để tách luồng xử lý.

### Hướng dẫn

1. Chọn Trigger On và cấu hình tuỳ chọn cần thiết.
2. Kích hoạt workflow để bắt đầu lắng nghe.
3. Gửi thử tin nhắn/notification để kiểm tra output.
