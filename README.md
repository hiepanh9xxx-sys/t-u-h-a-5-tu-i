# 🚂 Đoàn Tàu Nhỏ – Cuộc chạy trốn Tàu Nhện

Game 3D giáo dục cho bé khoảng 5 tuổi, chạy ngay trên trình duyệt (điện thoại và máy tính).
Bé trả lời câu hỏi để giúp đoàn tàu thoát khỏi yêu quái Tàu Nhện qua 7 chặng đường.

## Cách chơi

1. Chọn một đầu tàu: Bí Ngô, Mây Hồng, Rêu Ngọc, Ong Mật, Mực Tím hoặc Bông Tuyết.
2. Chọn chặng đường rồi bấm **Xuất phát!**
3. Trả lời câu hỏi:
   - **Đúng**: tàu ném một đồ vật (dưa hấu, bánh kem, quả bóng…) vào yêu quái, yêu quái mất 1 thanh máu và bé nhận một bộ phận tàu mới.
   - **Sai**: yêu quái tiến lại gần hơn. Sai lần 2 có gợi ý, sai lần 3 đáp án đúng sẽ nhấp nháy. Không có Game Over.
4. Hạ hết 5 thanh máu của yêu quái là về đích.

## Nội dung

| Chặng | Kiến thức | Yêu quái |
|---|---|---|
| Ga Bình Minh | Đếm số 1–10 | Tàu Nhện |
| Rừng Kỳ Bí | Màu sắc, hình dạng | Tàu Cá Sấu |
| Cầu Gỗ | So sánh, quy luật | Tàu Ma |
| Núi Lửa | Cộng, trừ trong phạm vi 10 | Tàu Núi Lửa |
| Nhà Máy Bỏ Hoang | Vị trí: trên/dưới, trái/phải, trong/ngoài, gần/xa | Tàu Nhện Sắt |
| Thung Lũng Cầu Vồng | Ôn tập | Tàu Ma Tím |
| Đường Hầm Cuối Cùng | Tổng hợp | Vua Tàu Nhện |

- 16 bộ phận tàu để sưu tập: đèn pha, chuông, ống khói vàng, cờ, bánh xe vàng, vương miện và 6 toa tàu.
- Combo: đúng 3 câu liên tiếp được COMBO ×3, 5 câu được TURBO, 10 câu thành SIÊU TÀU.
- Đủ 3 năng lượng: tàu kéo Siêu còi đẩy yêu quái lùi lại.

## Lưu game

- **Tự lưu** sau mỗi câu trả lời đúng, khi về đích và khi đóng hoặc chuyển tab.
- **Chơi tiếp:** nếu thoát giữa chặng, lần sau màn chọn tàu có nút **▶ Chơi tiếp**, quay lại đúng chặng với máu yêu quái, năng lượng và bộ phận đã nhận.
- **3 ô lưu:** bấm **💾 Lưu game** ở màn chọn tàu để tạo, đổi tên, chuyển hoặc xóa hồ sơ. Mỗi bé một ô riêng.
- **Lưu ngay:** nút 💾 trên thanh trên cùng khi đang chơi.
- **Chuyển sang máy khác:** trong bảng Lưu game, bấm **Lấy mã lưu**, gửi mã sang máy kia, dán vào ô và bấm **Dùng mã này**.
- Dữ liệu lưu trong trình duyệt của từng máy. Nếu xóa dữ liệu trình duyệt hoặc dùng chế độ ẩn danh thì sẽ mất, nên hãy giữ mã lưu nếu cần.

## Giọng đọc tiếng Việt

Mặc định game đọc câu hỏi bằng **giọng Google Tiếng Việt** (giọng của Google Dịch), phát dưới dạng âm thanh nên nghe rõ và giống nhau trên mọi máy, kể cả iPhone.

- Cần có kết nối mạng khi chơi.
- Đây là dịch vụ đọc miễn phí, không chính thức của Google Dịch. Nếu một lúc nào đó không tải được, game tự chuyển sang giọng tiếng Việt có sẵn của máy.
- Ở màn chọn tàu có ô **Giọng đọc** để đổi sang giọng của máy, và nút **Nghe thử**.
- Muốn có giọng máy tốt trên Android: Cài đặt → Chuyển văn bản thành giọng nói → chọn bộ máy của Google và tải gói tiếng Việt.

## Nhạc nền

Nhạc nền vui tươi được tạo trực tiếp bằng Web Audio (không cần file nhạc). Mỗi chặng có giai điệu và nhịp riêng, nhạc tự nhỏ lại khi giọng đọc câu hỏi. Bấm nút 🎵 để bật hoặc tắt.

## Chạy trên máy

Toàn bộ game nằm trong một file `index.html`. Mở trực tiếp file đó bằng trình duyệt là chơi được (cần mạng để tải thư viện Three.js và phông chữ).

Hoặc chạy một máy chủ tĩnh:

```bash
python3 -m http.server 8000
# mở http://localhost:8000
```

## Đưa lên GitHub và GitHub Pages

```bash
git init
git add .
git commit -m "Đoàn Tàu Nhỏ: game 3D cho bé"
git branch -M main
git remote add origin https://github.com/<tên-tài-khoản>/doan-tau-nho.git
git push -u origin main
```

Sau đó vào **Settings → Pages**, mục *Build and deployment* chọn **Deploy from a branch**, nhánh `main`, thư mục `/ (root)`, rồi bấm **Save**.
Sau khoảng 1 phút game sẽ có ở địa chỉ `https://<tên-tài-khoản>.github.io/doan-tau-nho/`.

## Công nghệ

- [Three.js r128](https://threejs.org/) (tải từ cdnjs) cho đồ họa 3D
- Web Audio API cho nhạc nền và hiệu ứng âm thanh
- Giọng Google Dịch (trực tuyến) và Web Speech API cho giọng đọc
- Phông chữ Baloo 2 từ Google Fonts

Các đầu tàu và yêu quái đều là thiết kế nguyên bản, không dùng nhân vật có bản quyền.
