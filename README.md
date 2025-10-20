# 💌 Thiệp 20/10 - From With Love

Thiệp chúc mừng Ngày Phụ nữ Việt Nam 20/10 động (HTML/CSS/JS) với:
- ✨ Hiệu ứng **phong thư mở ra** mượt mà
- 💖 **Tim bay** nền + **confetti tim rơi xuống**
- 📝 **Dòng chữ hiện dần** (typewriter-like, 1 giây/dòng)
- 🎨 Font chữ **handwritten** (Dancing Script) cho tiêu đề
- 🎵 Hỗ trợ **nhạc nền** (tùy chọn)

---

## 🚀 Hướng dẫn sử dụng

### Bước 1: Mở thiệp
- Mở `index.html` trong trình duyệt (kéo thả hoặc chuột phải -> Open with...).

### Bước 2: Chạy animation
- Nhấn nút **"Play"** để chạy hoạt ảnh. **"Replay"** phát lại.
- Animation tự động chạy khi tải trang lần đầu.

### Bước 3 (Tùy chọn): Thêm nhạc nền
- Trình duyệt có chính sách autoplay cho audio — nếu muốn nhạc nền, sửa file `index.html` và thêm đường dẫn âm thanh vào thẻ `<audio id="bgm">` như:

```html
<audio id="bgm" loop>
  <source src="./bgm/piano.mp3" type="audio/mpeg">
</audio>
```

Sau đó nhấn "Play" để phát nhạc (người dùng cần tương tác trước theo chính sách trình duyệt).

---

## 🎨 Tùy chỉnh nội dung

### Đổi lời chúc
Mở `index.html`, tìm phần:
```html
<div class="message" id="message">
  <div class="line">💌 Gửi cậu!</div>
```
Chỉnh sửa text trong các thẻ `<div class="line">`.

### Đổi màu sắc
- Nội dung thiệp: sửa các dòng trong phần `<div class="message">` (các thẻ `.line`).
- Màu sắc: chỉnh các biến trong `:root` (ví dụ `--accent`, `--bg1`).

### Điều chỉnh tốc độ hiện chữ
- Độ dài animation: chỉnh `setTimeout` trong `playSequence()` (hiện tại: 1000ms = 1 giây/dòng).

---

## 📹 Gợi ý khi xuất video

### Cách 1: Quay màn hình
- Nếu muốn xuất thành video (ví dụ để đăng Instagram), mình khuyên dùng công cụ quay màn hình 10s ở 1080p trong khi animation chạy.
- Dùng **OBS Studio**, **ShareX** (Windows), hoặc **QuickTime** (Mac).

### Cách 2: Headless rendering (nâng cao)
- Hoặc dùng FFMPEG compositing nếu muốn tạo file bền vững từ assets SVG/canvas (yêu cầu script bổ sung).
- Xuất thành video MP4 10s 1080p bằng cách tạo script headless (puppeteer + ffmpeg).

---

## 📝 License

- Miễn phí cho mục đích cá nhân. Cấp phép sử dụng và chỉnh sửa tự do.

---

## 💡 Hỗ trợ thêm

Nếu bạn muốn, mình có thể:

- ✅ Thêm bản nhạc mẫu miễn phí (piano/guitar) vào thư mục `bgm/` và cập nhật `index.html`.
- ✅ Tạo nhiều biến thể nội dung (cho mẹ, chị, bạn gái, đồng nghiệp).
- ✅ Thêm hiệu ứng 3D flip hoặc parallax advanced.

