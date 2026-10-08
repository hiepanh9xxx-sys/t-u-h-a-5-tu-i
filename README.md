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
- Tiến độ (bộ phận, sao, chặng đã mở) lưu trong trình duyệt của máy đang chơi.

## Giọng đọc tiếng Việt

Game dùng giọng đọc có sẵn của trình duyệt và tự ưu tiên giọng **Google Tiếng Việt**.

- **Chrome trên máy tính**: có sẵn giọng Google Tiếng Việt.
- **Android**: vào Cài đặt → Chuyển văn bản thành giọng nói → chọn bộ máy của Google và tải gói tiếng Việt.
- **iPhone / Safari**: dùng giọng tiếng Việt của Apple.

Có thể đổi giọng và nghe thử ở màn chọn tàu.

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
- Web Audio API cho hiệu ứng âm thanh
- Web Speech API cho giọng đọc
- Phông chữ Baloo 2 từ Google Fonts

Các đầu tàu và yêu quái đều là thiết kế nguyên bản, không dùng nhân vật có bản quyền.
