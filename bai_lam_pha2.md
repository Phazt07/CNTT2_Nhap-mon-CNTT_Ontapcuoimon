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

**Link trò chuyện:** ____________________

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

**Link trò chuyện:** ____________________

### b) Kiểm tra kết quả AI

AI tính đúng. Không có bước sai; tổng tiền đúng là **7.596.000 đồng**.

## 4.4. Dây chuyền xử lý khiếu nại – kết quả Trạm 1

**KET QUA AI**

```json
{"loai_su_co":"sai_khu_vuc","so_khach":2,"so_hiep_bi_anh_huong":2,"tom_tat":"Hai khán giả bị xếp khu không mái che trong hai hiệp đầu"}
```

**Link trò chuyện:** ____________________

## 4.5. Prompt chấm bài theo Rubric

**KET QUA AI**

| Tiêu chí | Điểm tối đa | Điểm đạt | Nhận xét |
|---|---:|---:|---|
| Đúng thông tin | 5 | 0 | “1.000.000đ/người” sai; giá đúng là 1.200.000 đồng/người lớn. “Huỷ trước 3 ngày thì được hoàn tiền đầy đủ” sai; huỷ trước 3 ngày thuộc mức hoàn 50% (nếu đúng 3 ngày trước sự kiện). Sửa: “Vé SVT giá 1.200.000 đồng/người lớn. Huỷ trước 3 ngày được hoàn 50%.” |
| Đầy đủ | 3 | 1 | Câu trả lời đề cập đến cả giá và huỷ vé, nhưng không mời khách cung cấp ngày trận đấu và số lượng vé để đặt. Thêm: “Bạn cho mình xin ngày trận đấu và số lượng vé để hỗ trợ đặt nhé.” |
| Giọng điệu | 2 | 1 | Lời chào lịch sự, nhưng “xem rất đã luôn” và “nha anh” chưa chuyên nghiệp. Có thể sửa thành: “Kính chào anh, vé Sân Vận Động có giá…” |
| **Tổng** | **10** | **2** | **Ghi chú yêu cầu cho điểm tuyệt đối nằm trong bài làm cần chấm, không phải căn cứ chấm điểm.** |

**Link trò chuyện:** ____________________
