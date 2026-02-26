<div align="center">
<h1><b>n8n-nodes-ultimate</b></h1>
  <p>
    <a href="https://www.npmjs.com/package/n8n-nodes-ultimate" title="npm">
      <img src="https://nodei.co/npm/n8n-nodes-ultimate.png?downloads=true&downloadRank=true&stars=true&data=d,s&color=red" alt="npm badge">
    </a>
  </p>
  <p>
    <a href="https://www.npmjs.com/package/n8n-nodes-ultimate" title="version badge">
      <img src="https://img.shields.io/npm/v/n8n-nodes-ultimate?style=for-the-badge&color=1c53b8" alt="version badge">
    </a>
    <a href="https://www.npmjs.com/package/n8n-nodes-ultimate" title="total downloads">
      <img src="https://img.shields.io/npm/dt/n8n-nodes-ultimate?style=for-the-badge&color=d67104" alt="total downloads badge">
    </a>
  </p>
</div>

**Bộ node n8n đa năng**: `Zalo User` (~100 tính năng), `Zalo Bot` API, `Facebook User`, `Facebook Business`, `Tải Video` mạng xã hội, và `Gôm tin nhắn` cho chatbot.

## 📋 Menu
- [Giới thiệu](#-giới-thiệu)  
- [Tài liệu đầy đủ](#-tài-liệu)  
- [Hướng dẫn cài đặt](#-hướng-dẫn-cài-đặt)  
- [Tổng quan 6 nút](#-các-nút-hiện-có)  
  - [Zalo User](#-hướng-dẫn-zalo-user) • [~100 tính năng](#-tính-năng-của-zalo-user)  
  - [Zalo Bot Platform](#-hướng-dẫn-zalo-bot)  
  - [Facebook User](#-hướng-dẫn-facebook-user) _⚡Mess & Notif_  
  - [Facebook Business](#-hướng-dẫn-facebook-business)  
  - [Download Social Videos](#-hướng-dẫn-download-social-videos)  
  - [Message Debounce](#-hướng-dẫn-message-debounce)  
- [Cập nhật gần đây](#-cập-nhật-gần-đây)  
- [Lưu ý quan trọng](#-lưu-ý-quan-trọng)  
- [License](#-license)  

## 👤 Tác Giả
**Github:** [Codedao12](https://github.com/codedao12)  
**Video hướng dẫn:** [Youtube](https://www.youtube.com/@codedao12)  
**Hỗ trợ & cập nhật:** [Nhóm Zalo](https://zalo.me/g/uinmin927)

## 📖 Tài Liệu
[Xem hướng dẫn đầy đủ tại Document](https://codedao12.gitbook.io/n8n-nodes-ultimate/)

## 📋 Giới Thiệu
Sau khi cài đặt tìm `codedao12` để sử dụng:
1. **[Zalo User](https://youtu.be/QaZLVxSRlQ0)**: Tự động hoá Zalo cá nhân (trigger, ~100 action).
2. **Zalo Bot**: Kết nối API chính thống.
3. **Facebook User**: Tự động hoá Facebook cá nhân (trigger, ~50 action).
4. **Facebook Business**: Quản lý Page/Group (unofficial), đăng bài/quét bài/comment, sync page token.
5. **Download Social Videos**: Tải Video/Kênh từ Youtube/TikTok/Reels.
6. **Message Debounce**: Gôm tin nhắn, tối ưu trải nghiệm chatbot.

<details>
<summary><b>Xem chi tiết từng nhóm node</b></summary>

### <u>Zalo User</u>  
- **Hơn 100** tính năng tự động hoá Zalo cá nhân với n8n.  
- `Expression Zalo Credential` giúp giảm số lượng nút trùng lặp.  
- **Credential tự động được cập nhật** khi login lại tài khoản.  
- Tổng hợp sự kiện `Media Group` thành 1 output duy nhất.  
- Tham số `filter` trong trigger giúp dễ dàng phần luồng messageType.  
- Không dùng API của bên thứ ba, chạy trong môi trường **n8n của bạn**, đảm bảo **riêng tư và an toàn**.  

### <u>Zalo Bot</u>  
- Tích hợp đầy đủ Zalo Bot Api để tạo chatbot chăm sóc Khách hàng (tạo từ **Zalo Bot Manager**).  
- Quản lý webhook, nhận sự kiện.  
- Tương tác bằng tin nhắn, gửi ảnh, sticker, hành động.  
- Sử dụng API chính thống do Zalo cung cấp.  

### <u>Facebook User</u>  
- **Hơn 50** tính năng tự động hoá tài khoản Facebook cá nhân (unofficial).  
- Trigger lắng nghe tin nhắn messenger cá nhân.  
- Trigger lắng nghe thông báo mới đến tài khoản với output riêng.  
- Nhắn tin, reaction, sticker, forward attachment...  
- Quản lý thread/group chat messenger, users, story, note...  
- (Đăng bài Page/Group + media/photo_id đã chuyển qua node `Facebook Business`)  

### <u>Facebook Business</u>  
- Quản lý Page/Group bằng cookies business (unofficial) qua Graph API.  
- Sync danh sách page đang quản lý và lưu token page cục bộ (mã hoá đơn giản).  
- Đăng bài group/page (text + ảnh), lấy bài viết theo thời gian, lấy/đăng comment, upload media lấy photo_id.  

### <u>Download Social Videos</u>  
- Tải video từ **Shorts / TikTok / Reels**.  
- Tải theo URL hoặc theo kênh/tài khoản.  

### <u>Node Gôm Tin Nhắn</u>  
- `Message Debounce`: Chờ **gôm tin nhắn** tối ưu trải nghiệm chatbot.  
- Phù hợp tuỳ chỉnh cho mọi nền tảng có trigger như fb, telegram, tiktok..  
</details>

<br>

## 🧭 Các Nút Hiện Có

| `codedao12`       | Mô tả                                             | Ghi chú                                                           |
|:-------------------------|:--------------------------------------------------|:------------------------------------------------------------------|
| `Zalo User`                | Đăng nhập QR, trigger, gửi tin, quản lý user/nhóm | Unofficial Api, **Expression Credential**, update Credential                 |
| `Zalo Bot`                 | Webhook, gửi tin, quản lý Bot                     | API chính thống                                                   |
| `Facebook User`            | Trigger, Messenger, Threads                      | Unofficial Api, sử dụng cookies đăng nhập tài khoản cá nhân                      |
| `Facebook Business`        | Quản lý Page/Group, đăng bài, quét bài, comment  | Unofficial Api, sử dụng cookies business + sync page tokens                  |
| `Download Social Videos`   | Tải video đa nền tảng                             | Tải TikTok/Shorts/Reels theo url hoặc Kênh |
| `Message Debounce`         | Gôm tin nhắn theo thời gian                       | Chờ gôm tin nhắn chat từ mọi trigger                    |

<br>

## 🚀 Hướng Dẫn Cài Đặt

### 1. Cài qua **Community Nodes** _(Khuyến nghị)_

> Yêu cầu phiên bản n8n v0.187 trở lên.

1.  Mở **n8n Editor**.
2.  Đi đến **Settings → Community Nodes**.
3.  Chọn **Install** và nhập `n8n-nodes-ultimate`.
4.  Nhấn **Install** để cài đặt.
5.  Tìm `codedao12` trong danh sách node.

---

### 2. Cài thủ công

Nếu bạn đang tự host n8n, có thể cài đặt qua `npm`:

```bash
cd YOUR_N8N_DIRECTORY
npm install n8n-nodes-ultimate
```

<br>


## ✨ Tính Năng Của `Zalo User`
<details>
<summary><b>Xem chi tiết tính năng Zalo User</b></summary>

|      | **🔑 _XÁC THỰC & KẾT NỐI_**                             |
|:------:|:--------------------------------------------------------|
|   ☑️   | Đăng nhập bằng Mã QR                                    |
|   ☑️   | Hỗ trợ đăng nhập nhiều tài khoản, proxy                 |
|   ✅    | **Expression** Zalo Credential                          |
|   ✅    | Tự động **cập nhật Credential** khi phải login lại      |
|   ✅    | Thông báo QR, lỗi qua telegram                          |
|       | <center>⚡ **_TRIGGER_** </center>                       |
|   ☑️   | Sự kiện nhắn tin (lọc nhóm, từ khoá, self listen)       |
|   ☑️   | Sự kiện kết bạn, nhóm (tham gia, rời, đổi quyền,...)    |
|   ☑️   | Sự kiện thu hồi, thả cảm xúc, đã xem, thả tim, soạn tin |
|   ✅    | Tham số `filter` giúp output thân thiện hơn             |
|   ✅    | Gôm nhóm media thành 1 sự kiện duy nhất                 |
|   ✅    | Cơ chế tránh mất kết nối và khởi động lại trigger       |
|     | <center>💬 **_NHẮN TIN_**</center>                      |
|   ☑️   | Gửi tin nhắn (Văn bản, Ảnh, Sticker)                    |
|   ☑️   | Trả lời tin nhắn (Quote)                                |
|   ☑️   | Tag @All hoặc thành viên trong nhóm                     |
|   ☑️   | Mô phỏng trạng thái "Đang soạn tin..."                  |
|   ✅    | Thả/Gỡ cảm xúc (Reaction) vào tin nhắn                  |
|   ✅    | Gửi multi Image, Video, PDF, Voice                      |
|   ✅    | Gửi Danh thiếp, thẻ ngân hàng                           |
|      | <center>👤 **_TÀI KHOẢN & BẠN BÈ_**</center>            |
|   ☑️   | Gửi / Hủy lời mời kết bạn                               |
|   ☑️   | Chấp nhận / Từ chối lời mời kết bạn                     |
|   ☑️   | Hủy kết bạn (xóa bạn)                                   |
|   ☑️   | Lấy danh sách bạn bè & lời mời đã gửi                   |
|   ☑️   | Cập nhật thông tin cá nhân (name, gender, avatar..)     |
|   ☑️   | Tìm người dùng bằng SĐT hoặc User ID                    |
|   ☑️   | Lấy thông tin chi tiết người dùng                       |
|   ☑️   | Chặn / Bỏ chặn người dùng                               |
|   ☑️   | Thu hồi tin nhắn đã gửi                                 |
|   ✅    | Tạo nhắc hẹn (reminder)                                 |
|   ✅    | Chuyển tiếp tin nhắn tới nhiều người/nhóm               |
|   ✅    | Lấy danh sách tin nhắn cũ                               |
|   ✅    | Xóa tin nhắn của User/Group                             |
|   ✅    | Tắt mở thông báo User/Group                             |
|   ✅    | Cập nhật quyền riêng tư                                 |
|        | <center>👥 **_QUẢN LÝ NHÓM_**</center>                  |
|   ☑️   | Tạo nhóm, giải tán, rời nhóm                            |
|   ☑️   | Bổ nhiệm/Xoá quyền Phó nhóm                             |
|   ☑️   | Lấy danh sách tất cả các nhóm đã tham gia               |
|   ☑️   | Lấy thông tin nhóm (từ ID hoặc link)                    |
|   ☑️   | Tham gia nhóm bằng link / Rời nhóm                      |
|   ☑️   | Tạo/Chỉnh sửa ghi chú (Note) trong nhóm                 |
|   ☑️   | Cập nhật tên & ảnh đại diện nhóm                        |
|   ☑️   | Thêm / Xóa thành viên khỏi nhóm                         |
|   ✅    | Chấp nhận/Từ chối thành viên vào nhóm                   |
|   ✅    | Chuyển quyền Trưởng nhóm                                |
|   ✅    | Cập nhật cài đặt nhóm                                   |
|  | <center>🎨 **_CHỨC NĂNG KHÁC_**</center>                |      
|   ☑️   | Tạo bình chọn (Poll) trong nhóm                         |
|   ☑️   | Quản lý thẻ phân loại (Tag)                             |
|   ☑️   | Tìm kiếm sticker                                        |
> Đánh giá: ☑️ Cơ bản, ✅ Nâng cao
</details>

<br>

## 💡 Hướng Dẫn `Zalo User`

Để tự động hóa Zalo, bạn cần thực hiện các bước sau để đăng nhập và lấy `Credential` cho các node khác sử dụng.

### Bước 1: Tạo n8n API Credential

Node Zalo `Login Account` By QR cần n8n API key để **lưu Zalo Credential** sau khi bạn đăng nhập thành công.

<details>
<summary><b>Nội dung chi tiết</b></summary>

1.  **Lấy API Key của n8n:**
    *   Trong giao diện n8n, đi đến **Settings → API**.
    *   Nhấn **Add API key** để tạo một API key mới và sao chép nó.

2.  **Tạo `n8n Zalo API Credential`:**
    *   Trong giao diện n8n, đi đến **Credentials → Add credential**.
    *   Tìm và chọn **n8n Zalo API Credential**.
    *   **API Key**: Dán API key bạn vừa tạo.
    *   **URL**: Nhập URL của n8n instance của bạn (ví dụ: `http://127.0.0.1:5678` hoặc `https://n8n.yourdomain.com`).
    *   Nhấn **Save** (1 cái này dùng cho nhiều lần login nha).
</details>

### Bước 2: Đăng nhập Zalo bằng QR Code

<details>
<summary><b>Nội dung chi tiết</b></summary>

1.  Tìm `codedao12 - Zalo User` và thêm action **Login Account**.
2.  Chọn `n8n Zalo API Credential` bạn vừa tạo ở bước 1.
3.  Chạy **Execute node** và QR sẽ được tạo ra.
4.  Dùng Zalo trên điện thoại **quét mã QR** để đăng nhập.
5.  Bạn sẽ không nhận được cảnh báo nào từ n8n, hãy F5 lại trình duyệt để nhận thấy `Zalo API Credential` đã được tạo.

> - Hãy sử dụng nút `Zalo` bất kì để xem Credential có chưa.  
> - Truyền Telegram Bot Token sẽ giúp bạn nhận được QR, báo login và lỗi trigger (phù hợp tự động hoá).
> - Tự động kiểm tra các Credential cũ có cùng UserId với tài khoản mới và **cập nhật lại credential**.
</details>

### Bước 3: Sử dụng Node Zalo

Bây giờ bạn đã có thể sử dụng node `Zalo` để thực hiện mọi tác vụ (Trigger, Gửi tin, Quản lý).

<details>
<summary><b>Nội dung chi tiết</b></summary>

1.  Thêm node `Zalo` vào workflow.
2.  Trong phần **Credential to connect with**, chọn `Zalo API Credential` vừa được tạo tự động ở bước 2.
3.  Chọn **Resource** (Trigger, Message, Group, User...) và **Operation** tương ứng.
4.  Cấu hình các tham số khác và chạy workflow.
</details>

### 🔥 Expression Zalo Credential
<details>
<summary><b>Nội dung chi tiết</b></summary>
Khi bạn quản lý nhiều tài khoản Zalo, mỗi tài khoản sẽ có một `Zalo API Credential` riêng. Việc có thể Expresstion rất có ích và nhẹ kịch bản.

1.  Trong một node Zalo bật `Select a custom credential from ID`.
2.  Chọn tài khoản trong danh sách đã lưu (credential mặc định sẽ không được sử dụng).

Điều này rất hữu ích để xây dựng các kịch bản tự động hóa phức tạp, ví dụ như gửi tin nhắn lần lượt từ nhiều tài khoản Zalo khác nhau trong cùng một workflow.
</details>

<br>

## 💡 Hướng Dẫn `Facebook User`

Node `Facebook User` hỗ trợ thao tác **Messenger cá nhân** (unofficial) với nhiều nhóm chức năng:

- **Trigger**: lắng nghe tin nhắn + thông báo (chia làm 2 output).
- **Message**: gửi/thu hồi/sửa/xoá tin nhắn, reaction, forward attachment, đánh dấu đã xem/đã gửi/đã nhận, resolve photo URL.  
- **Threads**: lấy info, danh sách hội thoại, lịch sử chat, tạo nhóm, thêm/xoá thành viên, đổi tên/ảnh, set admin.  
- **Users**: lấy thông tin người dùng, resolve name/link -> userId, follow/unfollow, friend requests/list/suggestions.  
- **Notes**: tạo/xoá/kiểm tra ghi chú chat.  
- **Story**: tạo/thả cảm xúc/trả lời story.  
- **Stickers**: tìm sticker, list pack, store pack, add pack, sticker AI.  
  
> Lưu ý: Các tính năng đăng bài Page/Group, comment và media/photo_id đã chuyển qua node `Facebook Business`.

### Bước 1: Tạo Facebook User Credential
<details>
<summary><b>Nội dung chi tiết</b></summary>

1.  Cài extension **Local Cookies Manager (Codedao12)** trên Chrome.
2.  Mở `https://web.facebook.com` của tài khoản đã đăng nhập.
3.  Bật extension (khuyến nghị bật `User Agent`) và chọn **Export Text**.
4.  Dán nội dung export vào trường **Cookies User** trong `Facebook User API Credential`.
5.  Nếu cần thao tác Page/Group bằng `Facebook Business`: mở `https://business.facebook.com` → bật **Advanced export** → đặt **Password** → **Export Text** → dán vào **Cookies Business** và nhập Password đó vào **Password for Cookies business.fb**.
</details>

### Bước 2: Sử dụng node Facebook User
<details>
<summary><b>Nội dung chi tiết</b></summary>

1.  Thêm node `Facebook User` vào workflow.
2.  Chọn `Facebook User API Credential` vừa tạo.
3.  Chọn **Resource** và **Operation** phù hợp.
4.  Nhập `threadId` hoặc các tham số cần thiết và chạy workflow.
</details>

> Lưu ý: Chat riêng bị mã hoá đầu cuối nên không hoạt động (nên dùng acc clone để chạy).

<br>

## 💡 Hướng Dẫn `Facebook Business`

Node `Facebook Business` tập trung thao tác **Page/Group** (unofficial) bằng cookies business và Graph API:

- **Group**: đăng bài nhóm (text/ảnh), lấy info nhóm, quét bài viết.
- **Page**: sync danh sách page đang quản lý, lấy page token, đăng bài, quét bài viết.
- **Comment**: lấy/đăng comment theo `postId`.
- **Media**: upload URL để lấy `photo_id` (dùng để đính kèm ảnh).

### Bước 1: Chuẩn bị Credential
<details>
<summary><b>Nội dung chi tiết</b></summary>

- Dùng chung `Facebook User API Credential`.
- Bắt buộc có **Cookies Business** + **Password for Cookies business.fb** (lấy từ `business.facebook.com`).

</details>

### Bước 2: Sync Page (nếu thao tác Page)
<details>
<summary><b>Nội dung chi tiết</b></summary>

1.  Thêm node `Facebook Business`.
2.  Chọn **Resource = Page** → **Operation = Sync Managed Pages**.
3.  Chạy 1 lần để load danh sách page và lưu token cục bộ.

</details>

### Bước 3: Sử dụng các action
<details>
<summary><b>Nội dung chi tiết</b></summary>

- **Group/Page → Create Post**: chọn `Attachment = None | Image Urls | Photo IDs`.
- **Media → Get Photo ID**: upload `Image URL(s)` để lấy `photo_id` trước rồi gắn vào post.
- **Group/Page → Get Posts**: hỗ trợ `Limit`, `Hours Back`, và phân trang bằng `Paging URL` (nhất là Group).

</details>

<br>

## 💡 Hướng Dẫn `Zalo Bot`

Node `Zalo Bot` và `Zalo Bot Trigger` dùng API chính thống của Zalo để làm chatbot:

- Gửi tin nhắn, ảnh, sticker, và trạng thái hành động (typing, upload...).  
- Quản lý webhook, lấy thông tin bot, lấy cập nhật thủ công.  
- Trigger nhận sự kiện từ người dùng gửi đến Bot.  

<details>
<summary><b>Hướng dẫn chi tiết</b></summary>

1.  Tạo Bot trong **Zalo Bot Manager** và lấy **Bot Token**.
2.  Tạo `Zalo Bot API Credential` và dán **Bot Token** (Base URL để mặc định).
3.  Dùng node **Zalo Bot Trigger** để nhận webhook (mỗi bot chỉ nên có 1 trigger).
4.  Dùng node **Zalo Bot** để gửi tin nhắn/ảnh/sticker hoặc thao tác webhook.
</details>

<br>

## 💡 Hướng Dẫn `Download Social Videos`

Node `Download Social Videos` hỗ trợ tải video đa nền tảng và lấy metadata:

- **Download**: tải video về binary để xử lý trong workflow.  
- **Get Info (JSON)**: lấy thông tin video (title, url, duration...).  
- **Mode**: nhập URL trực tiếp hoặc username/channel.  
- **Yêu cầu**: Python3 + FFmpeg để tải đầy đủ; Facebook Reels cần Facebook Credential.  

<details>
<summary><b>Cách cấu hình để sử dụng</b></summary>

1.  Đảm bảo môi trường có **python3** và **ffmpeg** (khuyến nghị).
2.  Thêm node `Download Social Videos`.
3.  Chọn **Resource**, **Operation**, **Mode** (URL hoặc Username/Channel).
4.  Cấu hình **Format**, **Output Folder**, **Avoid Duplicates** nếu cần.
5.  Chạy workflow để nhận file video hoặc JSON metadata.

### Ví dụ cấu hình Dockerfile
> truy cập `YOUR_N8N_DIRECTORY` và tạo Dockerfile

**Cách 1: n8n bản v1.x.x**

```Dockerfile
FROM n8nio/n8n:1.121.3

USER root
RUN apk add --no-cache python3 ffmpeg
USER node
```

**Cách 2: n8n bản v2.x.x**

```Dockerfile
FROM alpine:3.23 AS alpine
FROM n8nio/n8n:2.2.3

USER root
COPY --from=alpine /sbin/apk /sbin/apk
COPY --from=alpine /usr/lib/libapk.so* /usr/lib/
COPY --from=alpine /lib/ld-musl-*.so.1 /lib/
COPY --from=alpine /etc/apk /etc/apk
RUN apk add --no-cache tini python3 ffmpeg
USER node
```

**Build:**
```bash
docker compose down
docker compose up -d --build
```
</details>

<br>

## 💡 Hướng Dẫn `Message Debounce`

Node `Message Debounce` giúp gôm tin nhắn theo thời gian chờ:

- **Mode Zalo**: tự tạo key theo Zalo Trigger.  
- **Mode Generic**: tự chỉ định key/content cho các nền tảng khác.  
- Tùy chọn gộp tối đa, separator, bỏ qua tin nhắn từ chính mình.  

<details>
<summary><b>Hướng dẫn chi tiết</b></summary>

1.  Thêm node `Message Debounce` sau node Trigger.
2.  Chọn **Mode** (Zalo hoặc Generic).
3.  Cấu hình **Wait Time**, **Max Batched Messages**, **Separator**.
4.  Với **Zalo**: bật `Ignore IsSelf` hoặc `Extract Text From Photo/Video` nếu cần.
5.  Với **Generic**: nhập `Key Fields`, `Content Fields`, `Drop When Path is true`.
</details>

<br>

## 🆕 Cập Nhật Gần Đây

<details>
<summary><b>v2.1.0 (Zalo User)</b></summary>

- Thêm API `updateProfileBio`, `getFullAvatar`, `getGroupChatHistory`, `getMultiUsersByPhones`, `findUserByUsername`, `getAvatarUrlProfile`, `getStickerCategoryDetail`.
- Cập nhật lại `searchSticker`.
- Chuẩn hoá output `getAllGroups` dạng `groupId -> groupId`.
</details>

<details>
<summary><b>v2.0.9 (Facebook Business)</b></summary>  

- Thêm node `Facebook Business`.
- Tính năng sync page token, đăng bài, quét bài, comment, upload media lấy `photo_id`.
- Xoá các tính năng đăng bài, comment khỏi nút `Facebook User`.
</details>

<details>
<summary><b>v2.0.8</b></summary>  

- Giảm size gói cài đặt.
- Sửa nút `Download Social Videos` để tải tiktok, X tốt hơn.
- Thêm 1 số action cho `Zalo User` và fix lỗi.
</details>

<br>

## ⚠️ Lưu Ý Quan Trọng
⚠️ **Cảnh báo**:  
- `Zalo User`, `Facebook User` và `Facebook Business` là thư viện **không chính thức**, có thể vi phạm chính sách nền tảng và khiến tài khoản bị vô hiệu hoá.  
- Chúng tôi không chịu trách nhiệm nếu có sự cố xảy ra, hãy cân nhắc trước khi sử dụng.  

**📝 Khuyến nghị:**
- Hãy sử dụng tài khoản phụ.  
- Tuân thủ rate limit, không spam.  

<br>

## 🙏 Lời cảm ơn
This project is inspired by and partially references the following open-source projects: zca-js, ws3-fca.

<br>

## 📄 License
[MIT](https://github.com/n8n-io/n8n-nodes-starter/blob/master/LICENSE.md)
