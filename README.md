# CP Năng Lượng

Web cổ phiếu ngành Năng lượng Việt Nam · **v4.5 – 18/08/2026**

## Link (GitHub Pages)
https://nganhnangluong.github.io/cp-nang-luong/

## Tên khi ghim màn hình chính
**CP Năng Lượng**

## Wallpaper / Ảnh nền điện thoại

Ảnh blackhole cầu vồng (phù hợp màn hình điện thoại dọc):

- **Tải ảnh full HD**: [blackhole-wallpaper.jpg](https://nganhnangluong.github.io/cp-nang-luong/blackhole-wallpaper.jpg)

**Cách đặt làm hình nền:**
1. Mở link ảnh trên điện thoại → nhấn giữ → **Lưu ảnh**
2. Vào Cài đặt → Hình nền / Wallpaper → Chọn ảnh vừa tải

> **Lưu ý**: Hình nền hệ thống (iOS/Android) **không tự cập nhật**. Khi có ảnh mới chỉ cần tải lại và đặt lại.  
> App PWA sẽ tự tải phiên bản mới nhờ cache-buster.

## Cấu trúc hiện tại (sạch)
- `index.html` – loader (tải + giải nén app.b64.new)
- `app.b64.new` – payload HTML đầy đủ (gzip + base64)
- `manifest.json` + `icon.svg` – PWA
- `blackhole-wallpaper.jpg` – ảnh nền
- `README.md`

## Ghim màn hình chính
- iPhone Safari → Share → Thêm vào Màn hình chính
- Android Chrome → Cài đặt ứng dụng / Thêm vào màn hình chính

## Cách cập nhật app khi có bản mới
1. Tạo file `app.b64.new` mới (gzip HTML rồi base64)
2. Upload đè lên `app.b64.new`
3. Sửa cache-buster trong `index.html` (ví dụ `?v=20260818-1807` → `?v=20260819`)
4. Commit → người dùng mở lại app sẽ tự lấy bản mới (không cần xóa app)
