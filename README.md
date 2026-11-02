# 🌸 Khu Vườn Của Con — V7.2

> **App theo dõi thói quen cho bé** — biến việc nhà, học bài, đọc sách thành hành trình chăm sóc khu vườn kỳ diệu. Một file HTML duy nhất, chạy offline, không cần tài khoản, không quảng cáo.

<p align="center">
  <img src="https://img.shields.io/badge/version-7.2-pink?style=for-the-badge" alt="Version 7.2">
  <img src="https://img.shields.io/badge/format%20version-6-purple?style=for-the-badge" alt="Format version 6">
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

## 🎯 Tính năng nổi bật (V7.2)

### Cho bé
- 📝 **Thói quen hằng ngày** chia 3 buổi (Sáng / Chiều / Tối)
- 🌱 **18 loại cây** × 5 giai đoạn, SVG động có gradient + đổ bóng
- 🐾 **16 bạn thú cưng** × 4 câu nói hài hước khích lệ
- ✨ **Pet Evolution 3 Form** — Sơ sinh → Trưởng thành ⭐ → Thần thoại 👑
- 🪄 **Khiên Phép Thuật (Magic Shield)** — Làm bài tập đặc biệt để bảo vệ Chuỗi ngày (Streak) khi lỡ không hoàn thành KPI.
- 🌟 **Gương Mẫu Nhà Mình** — Bé giám sát thói quen của Bố Mẹ, đạt KPI thì tặng quà (5 Sao) để khích lệ.
- 🏅 **32 nhãn dán** thành tựu (Ngày Hoàn Hảo, Thợ Săn Kho Báu,…)
- 🦉 **Cú Thông Thái** với 114 câu đố 10 chủ đề + giải thích đáp án
- ⏳ **Đồng hồ cát** focus 5/10/15/20 phút
- 🎁 **Rương Phép Thuật** mở khi hoàn thành 100% việc trong ngày
- 🎟️ **Đổi quà** bằng Sao tích lũy
- 🔊 **Giọng đọc Tiếng Việt** tự nhiên (Google Cloud + Local)

### Cho Bố Mẹ
- 🔐 **Khóa PIN** + tự khóa sau 5 phút
- ⏪ **Sửa Lỗi Quá Khứ** — Chọn ngày trong quá khứ (7 ngày gần nhất) để tích bù việc bé quên, tự động tính lại Streak chuẩn xác.
- 👨‍👩‍👧‍👦 **Multi-child** — tối đa 4 bé, hồ sơ độc lập
- 🔥 **Ngưỡng Streak tùy chỉnh** 30–95% (riêng từng bé)
- 🎯 **Slot Pet Evolution** 1–16 (mặc định 5)
- ⚠️ **Thẻ nhắc nhở + phạt sao** có hoàn tác
- 📊 **Biểu đồ tuần** + nhật ký 300 hoạt động
- 💾 **Backup 3 tầng** (LocalStorage + Mirror + IndexedDB)
- 🛡️ **Snapshot tự động** — khôi phục bất kỳ lúc nào
- ♿ **Font scale 3 cỡ + Reduced motion** cho bé nhạy cảm

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
