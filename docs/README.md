# Giới thiệu
 
Bộ tài liệu này hướng dẫn sử dụng bộ node n8n của `codedao12` để tự động hóa Zalo, Facebook và tải video mạng xã hội. Bộ node gồm 5 phần chính: Zalo User, Zalo Trigger, Zalo Bot, Facebook User, Download Social Videos và Message Debounce.

## Điểm nổi bật

**Trigger**
- **Zalo User**: tin nhắn, lời mời kết bạn, thả tim của tài khoản cá nhân.
- **Zalo Bot**: nhận tin nhắn đến của khách hàng.
- **Facebook User**: tin nhắn group messenger và nghe thông báo của tài khoản facebook.

**Action**
- **Zalo User**: gửi tin nhắn, quản lý bạn bè/nhóm, sticker, poll, tag, catalog
- **Zalo Bot**: API chính thức để gửi tin và webhook
- **Facebook User**: nhắn tin, quản lý bạn bè, nhóm chat, đăng bài (unofficial)
- **Download Social Videos**: tải TikTok/YouTube/Facebook Reels
- **Message Debounce**: gộp tin nhắn theo thời gian

## Lưu ý quan trọng

- Zalo User và Facebook User là **unofficial**, cần dùng cẩn trọng với tài khoản thật.
- Zalo Bot là **official** (API chính thống).
- Một số tính năng cần cài thêm `python3` và `ffmpeg` khi tải video.
- Khuyến nghị n8n v0.187 trở lên để tương thích tốt.

## Yêu cầu

- n8n v0.187 hoặc mới hơn

## Hỗ trợ

- **Github**: https://github.com/codedao12
- **Video hướng dẫn**: https://youtu.be/DPcGiIKUm1Q
- **Nhóm Zalo**: https://zalo.me/g/uinmin927
