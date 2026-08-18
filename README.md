# CP Năng Lượng

Web cổ phiếu ngành Năng lượng Việt Nam · **Holy Grail Update 17/08/2026**

## Link (GitHub Pages)
https://nganhnangluong.github.io/cp-nang-luong/

## Tên khi ghim màn hình chính
**CP Năng Lượng**

## Wallpaper / Ảnh nền điện thoại

Ảnh blackhole cầu vồng siêu đẹp (phù hợp màn hình điện thoại dọc):

- **Tải ảnh full HD**: [blackhole-wallpaper.jpg](https://nganhnangluong.github.io/cp-nang-luong/blackhole-wallpaper.jpg)  
  (Sau khi bạn upload file này lên repo thì link sẽ hoạt động)

**Cách đặt làm hình nền:**
1. Mở link ảnh trên điện thoại → nhấn giữ → **Lưu ảnh** / Download
2. Vào Cài đặt → Hình nền / Wallpaper → Chọn ảnh vừa tải

> **Lưu ý về cập nhật tự động**: Hình nền hệ thống (iOS/Android) **không tự cập nhật**. Khi có phiên bản ảnh mới, bạn chỉ cần tải lại và đặt lại hình nền.  
> App PWA thì sẽ tự tải phiên bản mới khi bạn mở lại (nhờ cache-buster trong index.html).

## Cấu trúc hiện tại
- `index.html` – loader (tải + giải nén `app.b64 2.new`)
- `app.b64 2.new` – payload HTML đầy đủ (gzip + base64)
- `manifest.json` + `icon.svg` – PWA
- `blackhole-wallpaper.jpg` – ảnh nền (cần upload)
- `README.md`

## Bật GitHub Pages (nếu chưa)
1. https://github.com/NganhNangLuong/cp-nang-luong/settings/pages
2. Source → **Deploy from a branch**
3. Branch **main** · folder **/ (root)** → Save

## Ghim màn hình chính (Add to Home Screen)
- iPhone Safari → Share → Thêm vào Màn hình chính
- Android Chrome → Cài đặt ứng dụng / Thêm vào màn hình chính

## Cách cập nhật app khi có bản mới
1. Upload file HTML mới + cập nhật `app.b64 2.new` (nếu cần)
2. Sửa dòng cache-buster trong `index.html` (ví dụ `?v=20260818` → `?v=20260819`)
3. Commit & push → người dùng mở app sẽ tự lấy bản mới (không cần xóa app)
