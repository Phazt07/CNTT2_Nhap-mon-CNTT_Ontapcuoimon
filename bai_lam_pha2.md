# BÀI LÀM PHA 2

- **Họ tên:** __Lã Đức Phát__
- **Lớp:** __CNTT2__
- **Link repository Pha2:** ____________________
- **Công cụ AI đã dùng:** ChatGPT

> Pha 2 (20 phút cuối). Kết quả dưới đây được tạo bằng ChatGPT theo các prompt đã soạn cho Pha 1. Thêm link chia sẻ thực tế sau khi chạy từng prompt trong tài khoản của bạn.

## 4.2. Trích xuất tin nhắn đặt vé ra JSON

**KET QUA AI**

```json
[
  {"ma_goi":"SVT","ngay_su_kien":"2026-12-20","nguoi_lon":2,"tre_em":1,"loai_ve":"thuong","ghi_chu":null},
  {"ma_goi":"FZ","ngay_su_kien":"2027-01-05","nguoi_lon":3,"tre_em":0,"loai_ve":"thuong","ghi_chu":"một người cần hỗ trợ xe lăn"},
  {"ma_goi":"VIP","ngay_su_kien":null,"nguoi_lon":4,"tre_em":0,"loai_ve":"vip","ghi_chu":"một người khiếm thị cần hỗ trợ tìm chỗ"}
]
```

**Link trò chuyện:** ___https://chatgpt.com/s/cx_6b05a34054108191bc9a1f1decb17671_____

## 4.3. Báo giá vé bằng Chain-of-Thought

**KET QUA AI**

```text
Bước 1: Tiền vé 5 người lớn = 5 × 1.200.000 = 6.000.000 đồng.
Bước 2: Hai trẻ 8 và 10 tuổi = 2 × 1.200.000 × 70% = 1.680.000 đồng. Bé 3 tuổi dưới 5 tuổi nên miễn phí = 0 đồng.
Bước 3: Tiền vé trước giảm = 6.000.000 + 1.680.000 + 0 = 7.680.000 đồng.
Bước 4: Giảm giá = 7.680.000 × 5% = 384.000 đồng. Tiền vé sau giảm = 7.680.000 − 384.000 = 7.296.000 đồng.
Bước 5: Phụ thu ghế ưu tiên = 1 × 300.000 = 300.000 đồng.
Bước 6: Tổng thanh toán = 7.296.000 + 300.000 = 7.596.000 đồng.
[RESULT: 7.596.000 đồng]
```

**Link trò chuyện:** _____https://chatgpt.com/s/cx_6b05a3cd63e48191a3badf9afc871717_____

### b) Kiểm tra kết quả AI

AI tính đúng. Không có bước sai; tổng tiền đúng là **7.596.000 đồng**.

## 4.4. Dây chuyền xử lý khiếu nại – kết quả Trạm 1

**KET QUA AI**

```json
{"loai_su_co":"sai_khu_vuc","so_khach":2,"so_hiep_bi_anh_huong":2,"tom_tat":"Hai khán giả bị xếp khu không mái che trong hai hiệp đầu"}
```

**Link trò chuyện:** ___https://chatgpt.com/s/cx_6b05a43902848191b5b846ba60ff7b04_________________

## 4.5. Prompt chấm bài theo Rubric

**KET QUA AI**

| Tiêu chí | Điểm tối đa | Điểm đạt | Nhận xét |
|---|---:|---:|---|
| Đúng thông tin | 5 | 0 | “1.000.000đ/người” sai; giá chuẩn là **1.200.000 đồng/người lớn**. “Được hoàn tiền đầy đủ” cũng sai: huỷ trước trận đúng 3 ngày được hoàn **50%**, nên vẫn mất 50% tiền vé. Có thể sửa thành: “Vé Sân Vận Động có giá 1.200.000 đồng/người lớn. Nếu anh huỷ trước trận 3 ngày, anh được hoàn 50% tiền vé.” |
| Đầy đủ | 3 | 1,5 | Bài làm có đề cập đến cả giá vé và chính sách huỷ, nhưng thiếu lời mời khách cung cấp ngày trận đấu và số lượng vé để đặt. Có thể thêm: “Anh vui lòng cho em biết ngày trận đấu và số lượng vé cần đặt nhé.” |
| Giọng điệu | 2 | 1 | “Xem rất đã luôn ạ”, “nha anh” và “cứ nhắn em nhé” mang sắc thái suồng sã, chưa chuyên nghiệp. Có thể dùng: “Nếu anh cần hỗ trợ đặt vé, em sẵn sàng hỗ trợ ạ.” |

**Link trò chuyện:** _______https://chatgpt.com/s/cx_6b05a4b4615c8191b4f7d126b8a97ade_____________
