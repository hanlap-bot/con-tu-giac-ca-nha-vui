# Changelog — Khu Vườn Của Con

Tất cả thay đổi đáng chú ý của project được ghi tại đây.

Định dạng tuân theo [Keep a Changelog](https://keepachangelog.com/vi/1.1.0/),
version tuân theo [Semantic Versioning](https://semver.org/lang/vi/).

---

## [7.1] — 2026-10-26

### Added
- 🐾 **Pet Evolution 3 Form**: Sơ sinh → Trưởng thành ⭐ → Thần thoại 👑
  - Điều kiện Form 2: 100% thân thiết + 10 việc tốt
  - Điều kiện Form 3: Form 2 + chuỗi 7 ngày
  - Tên pet thay đổi theo form: `Tên gốc` → `Tên gốc ✨` → `Tên gốc 👑`
- 🎚️ **Slider giới hạn pet tiến hóa** 1–16 trong Góc Bố Mẹ (mặc định 5)
- 🎨 **Visual nâng cấp pet**:
  - Form 2: viền vàng + hiệu ứng glow nhẹ + badge ⭐
  - Form 3: viền tím + glow mạnh + badge 👑
- 💡 **Hint box trong Sticker Album** — hiển thị rõ còn thiếu gì để tiến hóa
- 🔘 **Nút "Tiến hóa → Form N"** ngay trên card pet
- 🔄 **Reset pet** — giải phóng slot nhưng bé vẫn giữ pet
- ✨ **Badge Nhãn Dán phát sáng** khi có pet sẵn sàng tiến hóa
- 📋 **Danh sách 16 pet** trong Góc Bố Mẹ với trạng thái từng con

### Changed
- State schema: `formatVersion: 4` → `5`
- Thêm field `petEvolutionMax` (default 5) + `petEvolution` (default `{}`) vào mỗi profile
- Companion card đổi viền theo form pet đang chọn

### Fixed
- Không còn "pet ma" khi đổi bé — pet evolution reset đúng theo profile
- Toast khi đạt điều kiện evolve không còn spam liên tục

### Migration
- V6.3 → V7.1: tự động, không mất dữ liệu
- Tất cả pet mặc định ở Form 1
- **Không downgrade** về V6.3 sau khi lên V7.1

---

## [6.3] — 2026-10-26

### Added
- 🛡️ **Error boundary** — mỗi hàm render bọc `safeRender()`, 1 lỗi không sập app
- 🚨 **Global recovery UI** — modal "Có lỗi xảy ra" với 2 nút Tải lại / Vẽ lại
- 📴 **Offline fallback CSS** — app vẫn dùng được khi mất WiFi
- 🔤 **Font scale 3 cỡ** (A / A+ / A++) — lưu ở key riêng `UI_PREFS_KEY`
- 🧘 **Reduced motion** — tắt animation cho bé nhạy cảm chuyển động
- ⚠️ **Banner cảnh báo localStorage sắp đầy** + nút "Xóa snapshot cũ"
- 💾 **Debounce save 400ms** — không serialize state mỗi lần render
- 🏷️ **Modal badge "Đang chỉnh cho: Bé X"** trên 4 modal (habit/reward/penalty/focus)

### Changed
- `saveState()` → debounced, flush khi `beforeunload` / `visibilitychange`
- Snapshot trim động theo size: 12 → 6 → 3 → 2 mốc khi storage tăng

### Fixed
- Toast z-index (từ V5.4.1) giữ nguyên `z-[9999]`
- Focus timer không còn chạy "ma" khi đổi bé
- Storage warning tự check mỗi 30s khi mở Góc Bố Mẹ

---

## [6.2] — 2026-10-26

### Added
- 👨‍👩‍👧‍👦 **Multi-child profiles** — tối đa 4 bé, độc lập hoàn toàn
- 🔄 **Nút "Đổi bé"** trong Góc Bố Mẹ với list 4 hồ sơ
- ➕ **Thêm bé mới** — tự đặt tên "Bé 2", "Bé 3",…
- 🗑️ **Xóa bé** — có confirm + snapshot tự động
- 👶 **Badge `👶 1/2`** trên header khi có > 1 bé
- 🎯 **Ngưỡng streak riêng** cho từng bé
- 🔄 **Reset độc lập** — chỉ reset bé đang chọn

### Changed
- State schema: `formatVersion: 3` → `4`
- Cấu trúc mới: `state.profiles = { p1, p2, p3, p4 }` + `activeProfileId`
- Các field dùng chung (PIN, voice, quiz, snapshots) vẫn ở top-level
- Migration V6.1 → V6.2: dữ liệu cũ wrap vào profile `p1` tự động

### Fixed
- Chuyển bé khi focus timer đang chạy → reset timer (fix tạm thời, hoàn thiện ở V6.3)

### Breaking
- **Không tương thích ngược** với V6.1 — Export JSON backup trước khi upgrade

---

## [6.0] — 2026-10-26

### Added
- 🌱 **10 loại cây mới** (tổng 18): Sồi, Thông, Nho, Đào, Chanh, Râm Bụt, Tulip, Cúc, Bonsai, Xương Rồng
- 🎨 **SVG cây nâng cấp toàn diện**: gradient 3 điểm dừng, đổ bóng, gân lá, đài hoa, quả có highlight, lấp lánh động
- 🐾 **8 thú cưng mới** (tổng 16): Bạch Tuộc, Rùa, Ong, Sư Tử, Voi, Hươu Cao Cổ, Ếch, Nhím
- 💬 **Mỗi pet có 4 câu nói hài hước** khích lệ bé (thay vì text đơn giản)
- 🏅 **20 nhãn dán mới** (tổng 32) — Ngày Hoàn Hảo, Vua Ngày Hoàn Hảo, Thợ Săn Kho Báu,…
- 🦉 **114 câu hỏi** (thay 8 câu cũ), 10 chủ đề, có giải thích đáp án
- 🔀 **Pool xáo trộn chống lặp** câu hỏi
- 📥 **Import/Export JSON** kho câu hỏi (textarea + file picker)
- 📋 **Tải file mẫu** câu hỏi JSON
- 🎚️ **Slider ngưỡng streak** 30–95% (thay cứng 70%)
- 📊 **Tracking mới**: `chestClaimCount`, `perfectDayCount`, `petsTriedSet`

### Changed
- State schema: `formatVersion: 2` → `3`
- Toàn bộ SVG cây được viết lại với chất lượng cao hơn

---

## [5.3] — 2026-10-26 (baseline)

### Added
- 📝 Thói quen hằng ngày 3 buổi + filter
- 🔥 Streak > 70% với reward ledger chống trùng
- 🌱 8 loại cây × 5 giai đoạn (SVG cơ bản)
- ⚠️ Thẻ nhắc nhở / phạt sao + hoàn tác
- 📊 Biểu đồ tuần 7 ngày
- 🎁 Đổi quà + lịch sử
- ⏳ Đồng hồ cát focus timer
- 🐾 8 thú cưng + 12 nhãn dán
- 🎁 Rương phép thuật 100%
- 📜 Nhật ký 300 hoạt động + lưu trữ ngày
- 🔐 PIN bố mẹ + tự khóa 5 phút
- 💾 Snapshot 3 tầng (LocalStorage + Mirror + IndexedDB)
- 🔊 Giọng đọc tiếng Việt (Google Cloud + Local voice)
- 💾 Sao lưu / khôi phục / nạp mẫu / reset
- 🎉 Confetti + Web Audio sound effects

### Known Issues (đã fix ở V5.4.1+)
- Toast bị modal che khuất (`z-50` trùng với modal)
- Câu đố chỉ có 8 câu, lặp lại rất nhanh

---

## Quy ước version

- **Major (X.0)**: Thay đổi cấu trúc state không tương thích (breaking changes)
- **Minor (X.Y)**: Thêm tính năng mới, không breaking
- **Patch (X.Y.Z)**: Fix bug, không thêm tính năng

---

## Format version (nội bộ)

| Format | Version app | Ghi chú |
|---|---|---|
| 1 | V5.3 | State 1 tầng |
| 2 | V5.4.1 | Thêm `_meta` + custom quiz |
| 3 | V6.0 | Thêm pet evolution fields chuẩn bị |
| 4 | V6.2 | Multi-child profiles |
| 5 | V7.1 | Pet evolution 3 form |
