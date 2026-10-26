# 🌸 Khu Vườn Của Con — V7.1

> **App theo dõi thói quen cho bé** — biến việc nhà, học bài, đọc sách thành hành trình chăm sóc khu vườn kỳ diệu. Một file HTML duy nhất, chạy offline, không cần tài khoản, không quảng cáo.

<p align="center">
  <img src="https://img.shields.io/badge/version-7.1-pink?style=for-the-badge" alt="Version 7.1">
  <img src="https://img.shields.io/badge/format%20version-5-purple?style=for-the-badge" alt="Format version 5">
  <img src="https://img.shields.io/badge/single--file-HTML-amber?style=for-the-badge" alt="Single file HTML">
  <img src="https://img.shields.io/badge/license-MIT-green?style=for-the-badge" alt="MIT License">
</p>

---

## ✨ Vì sao có app này?

Bé nhà mình lười đánh răng, hay quên cất đồ chơi, đọc sách 2 phút là chán. Mình thử đủ cách: bảng sticker giấy, app trên App Store (toàn tính phí + quảng cáo + thu thập dữ liệu trẻ em),… Không cái nào hợp.

Nên mình tự làm **1 file HTML duy nhất**:
- ✅ **Không cần tài khoản, không quảng cáo, không theo dõi**
- ✅ **Chạy offline 100%** (sau lần đầu load CDN)
- ✅ **Dữ liệu lưu trên máy** — không gửi đi đâu
- ✅ **Miễn phí mãi mãi** cho gia đình dùng
- ✅ **Có thể tải về, sửa, chia sẻ** (giấy phép MIT)

---

## 🎯 Tính năng nổi bật (V7.1)

### Cho bé
- 📝 **Thói quen hằng ngày** chia 3 buổi (Sáng / Chiều / Tối)
- 🌱 **18 loại cây** × 5 giai đoạn, SVG động có gradient + đổ bóng
- 🐾 **16 bạn thú cưng** × 4 câu nói hài hước khích lệ
- ✨ **Pet Evolution 3 Form** — Sơ sinh → Trưởng thành ⭐ → Thần thoại 👑
- 🏅 **32 nhãn dán** thành tựu (Ngày Hoàn Hảo, Thợ Săn Kho Báu,…)
- 🦉 **Cú Thông Thái** với 114 câu đố 10 chủ đề + giải thích đáp án
- ⏳ **Đồng hồ cát** focus 5/10/15/20 phút
- 🎁 **Rương Phép Thuật** mở khi hoàn thành 100% việc trong ngày
- 🎟️ **Đổi quà** bằng Sao tích lũy
- 🔊 **Giọng đọc Tiếng Việt** tự nhiên (Google Cloud + Local)

### Cho Bố Mẹ
- 🔐 **Khóa PIN** + tự khóa sau 5 phút
- 👨‍👩‍👧‍👦 **Multi-child** — tối đa 4 bé, hồ sơ độc lập
- 🔥 **Ngưỡng Streak tùy chỉnh** 30–95% (riêng từng bé)
- 🎯 **Slot Pet Evolution** 1–16 (mặc định 5)
- ⚠️ **Thẻ nhắc nhở + phạt sao** có hoàn tác
- 📊 **Biểu đồ tuần** + nhật ký 300 hoạt động
- 💾 **Backup 3 tầng** (LocalStorage + Mirror + IndexedDB)
- 🛡️ **Snapshot tự động** — khôi phục bất kỳ lúc nào
- ♿ **Font scale 3 cỡ + Reduced motion** cho bé nhạy cảm
- 📥 **Import/Export JSON** kho câu hỏi

---

## 🚀 Dùng ngay (không cần cài đặt)

### Cách 1: Mở file trực tiếp
1. Tải file `index.html` về máy
2. Đúp chuột → mở bằng Chrome / Safari / Edge
3. **Xong!** Không cần cài đặt gì

### Cách 2: Dùng trên iPad như app thật
1. Mở URL của app (sau khi deploy GitHub Pages)
2. Safari → nút **Chia sẻ** → **"Thêm vào MH chính"**
3. Có icon 🌸 trên màn hình chính, chạy toàn màn hình như app native

---

## 📱 Tương thích

| Thiết bị | Trạng thái |
|---|---|
| iPad (Safari) | ✅ Tốt nhất — thiết kế chính cho iPad |
| iPhone (Safari) | ✅ Chạy được, layout thu gọn |
| Android (Chrome) | ✅ Chạy tốt |
| Windows / macOS | ✅ Chrome, Edge, Safari |
| Firefox | ⚠️ TTS có thể chậm hơn |

**Yêu cầu**: Trình duyệt hiện đại (2022+), có `localStorage` + `IndexedDB`.

---

## 💾 Dữ liệu & Quyền riêng tư

- **Toàn bộ dữ liệu lưu trên máy bạn** — không có server, không cloud
- **Không có tài khoản** — không email, không mật khẩu
- **Không quảng cáo, không analytics, không tracking**
- **3 tầng bảo vệ**: LocalStorage → Mirror → IndexedDB
- **Snapshot tự động** trước mọi thao tác nguy hiểm
- **Backup thủ công**: Góc Bố Mẹ → Tải file `.JSON`

⚠️ **Lưu ý**: Xóa cache trình duyệt = mất dữ liệu. **Nên export JSON định kỳ** và lưu vào Google Drive / iCloud.

---

## 📂 Cấu trúc repo
khuvuoncuabe/
├── index.html ← File V7.1 (mở là chạy)
├── README.md ← File này
├── CHANGELOG.md ← Lịch sử version
├── LICENSE ← Giấy phép MIT
├── .gitignore ← Loại trừ file rác
└── versions/ ← Lưu lịch sử các bản cũ
├── v5.3-final.html
├── v6.0-final.html
├── v6.2-final.html
├── v6.3-final.html
└── v7.1-final.html

---

## 🗺️ Lộ trình

| Phiên bản | Nội dung | Trạng thái |
|---|---|---|
| V5.3 | App cơ bản cho 1 bé | ✅ |
| V6.0 | 18 cây, 16 pets, 114 câu hỏi | ✅ |
| V6.2 | Multi-child 4 bé | ✅ |
| V6.3 | Patch ổn định | ✅ |
| **V7.1** | **Pet Evolution 3 Form** | ✅ |
| V7.2 | Weekly Report | ⏳ Sắp tới |
| V7.3 | Bé tặng quà bố mẹ | ⏳ |
| V8 | Story mode + Time capsule | 💭 |

---

## 🛠️ Phát triển

App là **1 file HTML duy nhất** — không cần build, không cần npm, không cần bundler.

### Muốn sửa?
1. Mở `index.html` bằng VS Code hoặc bất kỳ editor
2. Sửa code → lưu → reload trình duyệt (F5)
3. **Không cần** compile

### Muốn thêm câu hỏi đố vui?
- Dùng UI: Góc Bố Mẹ → Import JSON
- Hoặc sửa mảng `DEFAULT_QUIZ_QUESTIONS` trong code

### Muốn thêm cây / pet mới?
- Sửa `PLANT_TYPES` hoặc `GARDEN_PETS` trong object constant
- Không cần sửa logic

---

## 🤝 Đóng góp

Đây là project cá nhân cho gia đình, nhưng:
- 🐛 **Báo bug** — mở Issue
- 💡 **Gợi ý tính năng** — mở Issue với tag `enhancement`
- 🔧 **Pull request** — luôn welcome, đặc biệt về SVG cây/pet

---

## 📜 Giấy phép

MIT License — xem file [LICENSE](LICENSE).

**Được phép**: Dùng, sửa, chia sẻ, bán (nếu muốn) — miễn giữ copyright notice.

---

## 💖 Credits

- **Font**: [Quicksand](https://fonts.google.com/specimen/Quicksand) — Google Fonts
- **Icons**: [Font Awesome 6](https://fontawesome.com/)
- **CSS Framework**: [Tailwind CSS](https://tailwindcss.com/)
- **Confetti**: [canvas-confetti](https://github.com/catdad/canvas-confetti)
- **TTS**: Google Translate TTS (fallback) + Web Speech API (local)

---

<p align="center">
  Made with ❤️ for bé yêu
  <br>
  🌸 🌱 🐾 🦉 ⭐
</p>
