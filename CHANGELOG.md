# Changelog — Khu Vườn Của Con

Tất cả thay đổi đáng chú ý của project được ghi tại đây.

Định dạng tuân theo [Keep a Changelog](https://keepachangelog.com/vi/1.1.0/),
version tuân theo [Semantic Versioning](https://semver.org/lang/vi/).

---

## [7.2] — 2026-10-26

### Added
- 🪄 **Magic Shield (Khiên Phép Thuật)**: Tính năng cứu Streak khi bé lỡ không đạt KPI.
  - Bố mẹ cài đặt câu hỏi/đáp án trong Góc Quản Lý.
  - Khi bé sắp mất Streak, nút "Cứu Streak" xuất hiện. Bé trả lời đúng -> Bố mẹ xác nhận -> Nhận Khiên.
  - Khiên tự động kích hoạt bảo vệ Streak vào ngày hôm sau nếu bé không đạt mục tiêu.
- ⏪ **Sửa Lỗi Quá Khứ (Past Day Editing)**: Bố mẹ có thể chọn 1 ngày trong 7 ngày gần nhất để tích bù các task bé quên. Hệ thống tự động tính toán lại Chuỗi (Streak) và biểu đồ tuần chính xác.
- 🌟 **Gương Mẫu Nhà Mình (Parent Habits)**: Bé giám sát thói quen của Bố Mẹ.
  - Bố Mẹ đặt mục tiêu (VD: 3 lần/tuần) cho thói quen của mình.
  - Bé bấm xác nhận khi thấy Bố Mẹ hoàn thành. Đạt KPI, bé có thể dùng 5 Sao để Tặng Quà cho Bố Mẹ.

### Fixed
- 🐛 **Lỗi tích lũy giọt nước**: Sửa lỗi "Tích hoàn thành -> Hủy -> Tích lại thì không được cộng giọt nước". Hệ thống giờ đây cho phép hoàn tác và cộng lại phần thưởng (Sao, Nước, Dâu) một cách chính xác nếu task được tích lại.

### Changed
- State schema: `formatVersion: 5` → `6`.
- Thêm field `magicShield` và `parentHabits` vào mỗi profile.

---

## [7.1] — 2026-10-26

### Added
- 🐾 **Pet Evolution 3 Form**: Sơ sinh → Trưởng thành ⭐ → Thần thoại 👑
- 🎚️ **Slider giới hạn pet tiến hóa** 1–16 trong Góc Bố Mẹ (mặc định 5)
- 🎨 **Visual nâng cấp pet**: Viền vàng/tím phát sáng theo cấp độ.
- 💡 **Hint box** trong Sticker Album báo thiếu gì để tiến hóa.
- 🔄 **Reset pet** giải phóng slot nhưng bé vẫn giữ pet.

### Changed
- State schema: `formatVersion: 4` → `5`.

---

## [6.3] — 2026-10-26

### Added
- 🛡️ **Error boundary** — 1 lỗi không sập app.
- 🚨 **Global recovery UI** — khôi phục màn hình khi lỗi.
- 📴 **Offline fallback CSS**.
- 🔤 **Font scale 3 cỡ** + **Reduced motion**.
- 💾 **Debounce save 400ms** (chống mất dữ liệu).

---

## [6.2] — 2026-10-26

### Added
- 👨‍👩‍👧‍👦 **Multi-child profiles** (Tối đa 4 bé).
- 🔄 Nút **"Đổi bé"** và quản lý hồ sơ độc lập.
- 🎯 Ngưỡng streak và cấu hình riêng cho từng bé.

---

## [6.0] — 2026-10-26

### Added
- 🌱 10 loại cây mới (tổng 18), SVG nâng cấp.
- 🐾 8 thú cưng mới (tổng 16).
- 🏅 20 nhãn dán mới (tổng 32).
- 🦉 114 câu hỏi Cú Thông Thái.
- 🎚️ Slider ngưỡng Streak (30-95%).
- 📥 Import/Export JSON câu hỏi.

---

## [5.3] — 2026-10-26 (baseline)

### Added
- 📝 Thói quen hằng ngày 3 buổi + filter.
- 🔥 Streak > 70%.
- 🌱 8 loại cây (SVG cơ bản).
- ⚠️ Thẻ nhắc nhở / phạt sao.
- 📊 Biểu đồ tuần 7 ngày.
- 🎁 Đổi quà + Đồng hồ cát.
- 🐾 8 thú cưng + 12 nhãn dán.
- 🎁 Rương phép thuật 100%.
- 🔐 PIN bố mẹ + tự khóa.
- 💾 Snapshot 3 tầng.
- 🔊 Giọng đọc tiếng Việt.
