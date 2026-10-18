# AI English Companion

Ứng dụng học tiếng Anh trên máy tính Windows: AI Tutor sửa lỗi bằng tiếng Việt, luyện nói theo tình huống, từ vựng ôn
theo lịch FSRS, luyện nghe, ngữ pháp, giao tiếp, luyện thi TOEIC và IELTS. Dữ liệu học lưu trên máy của bạn, AI chạy
ngay trên máy.

Repo này chỉ chứa **bản cài đặt, bản cập nhật và gói bài học**.

## ⬇️ Tải về

**[Tải bản mới nhất](https://github.com/1995mars/ai-english-companion-releases/releases/latest)** → trong mục
*Assets*, tải file `AI-English-Companion_<phiên bản>_x64-setup.exe`.

## Yêu cầu hệ thống

| | Tối thiểu (học không cần AI hội thoại) | Khuyến nghị (đầy đủ AI) |
|---|---|---|
| Hệ điều hành | Windows 10 22H2 / Windows 11, 64-bit | Windows 11 |
| RAM | 8 GB | 16 GB trở lên |
| Card đồ họa | Không bắt buộc | NVIDIA ≥ 8 GB VRAM |
| Ổ đĩa trống | ~1 GB | ~12 GB (gồm các model AI) |

## Cài đặt

1. Chạy file `AI-English-Companion_..._x64-setup.exe` vừa tải.
2. Nếu Windows hiện **"Windows protected your PC"** (SmartScreen): bấm **More info → Run anyway**.
   Cảnh báo này xuất hiện vì bộ cài chưa có chứng chỉ ký mã thương mại.
3. Làm theo trình cài đặt. Ứng dụng cài cho tài khoản Windows hiện tại, **không cần quyền admin**. Nếu máy chưa có
   WebView2, bộ cài sẽ tự tải (Windows 11 đã có sẵn).
4. Mở **AI English Companion** từ Start menu. Lần đầu, ứng dụng hỏi vài câu (trình độ, mục tiêu, thời gian học) và
   cho làm bài kiểm tra đầu vào khoảng 15 phút (có thể bỏ qua) để tạo lộ trình học riêng.

> Đã học trên máy khác và bật đồng bộ Google Drive? Ở màn hình chào mừng, bấm **Đăng nhập bằng Google** để tải dữ
> liệu học về, không cần thiết lập lại.

## Bật các tính năng AI (tùy chọn)

Từ vựng, luyện nghe, ngữ pháp, bài giao tiếp và luyện đề TOEIC/IELTS **dùng được ngay**. AI Tutor, luyện nói và
chấm Writing/Speaking cần thêm model AI chạy trên máy:

1. **Cài Ollama** (dùng cho AI Tutor, chấm bài): tải ở <https://ollama.com/download> hoặc chạy
   `winget install Ollama.Ollama`, rồi mở Ollama.
2. Trong ứng dụng, vào **Cài đặt → Mô hình AI**:
   - **Mô hình hội thoại:** bấm *Tải model*. Chọn Qwen3.5 9B (6.6 GB, cần GPU ≥ 8 GB VRAM) hoặc Qwen3.5 4B
     (3.4 GB, chạy được bằng CPU nhưng chậm hơn).
   - **Nhận dạng giọng nói:** bấm *Chuẩn bị model* (Whisper large-v3-turbo 1.6 GB, hoặc small.en 0.5 GB cho máy yếu).
   - **Máy có GPU NVIDIA:** bấm *Cài gói tăng tốc GPU* (~1.2 GB) để nhận dạng giọng nói nhanh hơn.
3. Mỗi model chỉ tải **một lần** (cần Internet); sau đó dùng được khi không có mạng.

## Cập nhật

- **Ứng dụng:** tự kiểm tra bản mới khi mở và mỗi ngày một lần. Khi có bản mới, bấm *Cập nhật*; ứng dụng tải, kiểm tra
  chữ ký, cài đặt rồi tự mở lại. Dữ liệu học được giữ nguyên.
- **Bài học mới:** **Cài đặt → Cập nhật → Bài học mới** để tải thêm gói bài học.
- Có thể tắt tự kiểm tra trong **Cài đặt → Cập nhật**.

## Sao lưu & gỡ cài đặt

- **Sao lưu:** **Cài đặt → Dữ liệu → Sao lưu ngay**, rồi bấm *Tải về* để lưu file `.zip` ra nơi khác. Khôi phục ở
  cùng mục.
- **Gỡ cài đặt:** Windows **Settings → Apps → Installed apps → AI English Companion → Uninstall**. Dữ liệu học
  **không** bị xóa. Muốn xóa hẳn, xóa thư mục `%APPDATA%\AIEnglishCompanion\`.

## Gặp sự cố?

- Nhật ký lỗi: `%APPDATA%\AIEnglishCompanion\logs\backend.log` (không chứa nội dung hội thoại hay bài viết).
- Chỉ báo **"AI cần thiết lập"** ở góc trên: vào **Cài đặt → Mô hình AI** để xem model nào còn thiếu.

## Lưu ý

Điểm TOEIC và band IELTS trong ứng dụng là **ước lượng tham khảo**, không phải điểm thi chính thức. Ứng dụng không chấm
phát âm theo âm vị.
