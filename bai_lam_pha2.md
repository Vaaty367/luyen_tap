# BÀI LÀM PHA 2 (ĐỀ LUYỆN TẬP CHỦ ĐỀ CHẠY AFFILIATE)

- **Họ tên:** Trần Xuân Nhật
- **Lớp:** K26-CNNT3
- **Link repository Pha2:** https://github.com/Vaaty367/luyen_tap/commit/0c1c217bb6d72d960d631a5d9d7e096620e915fe
- **Công cụ AI đã dùng (ChatGPT/Claude/Gemini):** Gemini

> Pha 2 (20 phút cuối). Mỗi mục: mở cuộc trò chuyện mới, gửi nguyên văn prompt đã viết trong bai_lam_pha1.md, dán câu trả lời và link chia sẻ vào đây. Xong, kéo thả file này vào repository Pha2.

## 4.2. Trích xuất tin nhắn đăng ký gói Affiliate ra JSON

**KET QUA AI**

```text
[
  {
    "ma_goi": "TT",
    "ngay_bat_dau": "2026-12-20",
    "creator_chinh": 2,
    "thuc_tap_sinh": 1,
    "hang_tai_khoan": "thuong",
    "ghi_chu": null
  },
  {
    "ma_goi": "SP",
    "ngay_bat_dau": "2027-01-08",
    "creator_chinh": 3,
    "thuc_tap_sinh": 0,
    "hang_tai_khoan": null,
    "ghi_chu": "ngồi bàn gần cửa ra vào (có một bạn đang bó bột chân)"
  },
  {
    "ma_goi": "PRO",
    "ngay_bat_dau": null,
    "creator_chinh": 4,
    "thuc_tap_sinh": 0,
    "hang_tai_khoan": "vip",
    "ghi_chu": "mượn thêm đèn trợ sáng và phông xanh để quay mẫu"
  }
]
```

**Link trò chuyện:**https://share.gemini.google/fVt50eqNZgjh

## 4.3. Báo giá gói Affiliate bằng Chain-of-Thought

**KET QUA AI**

```text
Tiền Creator chính: 4 × 1.500.000 = 6.000.000 đồng

Tiền thực tập sinh: 2 × (1.500.000 × 60%) = 2 × 900.000 = 1.800.000 đồng (bé 7 tuổi miễn phí: 0 đồng)

Tổng tiền gói: 6.000.000 + 1.800.000 = 7.800.000 đồng

Giảm giá team: 7.800.000 × 10% = 780.000 đồng (tiền gói sau giảm: 7.800.000 - 780.000 = 7.020.000 đồng)

Phụ thu thuê mic: 2 × 250.000 = 500.000 đồng

Tổng tiền: 7.020.000 + 500.000 = 7.520.000 đồng

[RESULT: 7.520.000 đồng]
```

**Link trò chuyện:** https://share.gemini.google/ihDAFik9tasX

### b) Kiểm tra kết quả AI

kết luận AI đúng

## 4.4. Dây chuyền xử lý khiếu nại – kết quả Trạm 1

**KET QUA AI**

```text
{
  "loai_su_co": "sai_phong",
  "so_khach": 3,
  "so_ca_bi_anh_huong": 2,
  "tom_tat": "Bị xếp sai phòng thiếu đèn livestream và cách âm trong 2 ca thực hành đầu."
}
```

**Link trò chuyện:** https://share.gemini.google/qv4hch6e5xax

## 4.5. Prompt chấm bài theo Rubric

**KET QUA AI**

```text
| Tiêu chí | Điểm | Minh chứng | Đề xuất sửa |
| --- | --- | --- | --- |
| Đúng thông tin | 0/5,0 | - Nguyên văn: `"Gói TikTok Affiliate bên mình giá chỉ 1.200.000đ/người thôi"` -> Lý do sai: Giá chuẩn là 1.500.000 đồng/Creator chính, báo sai giá và sai đối tượng áp dụng.<br>

<br>- Nguyên văn: `"Bạn báo huỷ trước 5 ngày thì được hoàn lại đủ 100% tiền nha"` -> Lý do sai: Huỷ trước 5 ngày (thuộc khoảng từ 3 đến 6 ngày) chỉ được hoàn 50%, không phải 100%. | - `"Gói TikTok Affiliate bên mình có mức phí 1.500.000 đồng/Creator chính ạ."`<br>

<br>- `"Nếu anh/chị báo huỷ trước ngày bắt đầu 5 ngày (thuộc khung từ 3 đến 6 ngày), trung tâm sẽ hỗ trợ hoàn 50% học phí ạ."` |
| Đầy đủ | 1,5/3,0 | - Nguyên văn: Không có câu nào mời khách hàng cung cấp ngày đợt thực chiến và số lượng suất muốn đăng ký -> Lý do sai: Thiếu bước kêu gọi/thu thập thông tin cần thiết để chốt đăng ký dù đã trả lời 2 câu hỏi chính. | - `"Anh/chị cho em xin thông tin đợt thực chiến mong muốn và số lượng suất cần đăng ký để bên em giữ chỗ và hỗ trợ chi tiết ạ."` |
| Giọng điệu | 0/2,0 | - Nguyên văn: `"Dạ hello bạn nha!"`, `"cứ chốt lẹ kẻo hết slot nè!"` -> Lý do sai: Xưng hô suồng sã, dùng từ ngữ kém chuyên nghiệp và tạo áp lực không phù hợp.<br>

<br>- Nguyên văn: `"đăng ký xong gắn link là nổ đơn hoa hồng trăm triệu luôn ạ."` -> Lý do sai: Cam kết doanh thu/hoa hồng ảo, gây hiểu lầm cho khách hàng. | - `"Dạ em chào anh/chị ạ! Hiệu quả kinh doanh và hoa hồng sẽ phụ thuộc vào năng lực triển khai và sản phẩm của từng kênh, trung tâm sẽ đồng hành và hướng dẫn quy trình tối ưu cho anh/chị ạ."` |

Tổng điểm: 1,5/10
```

**Link trò chuyện:** https://share.gemini.google/NEyPgnG0dByw
