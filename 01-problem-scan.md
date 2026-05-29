# Phase 1 — SCAN

## Opportunity Scan Table

| # | Subsidiary | Lens             | Mô tả ngắn bài toán                                                                                                  |
| - | ---------- | ---------------- | -------------------------------------------------------------------------------------------------------------------- |
| 1 | Vinmec     | Time-consuming   | Bác sĩ phải đọc và tổng hợp hồ sơ bệnh án dài trước khi khám, mất nhiều thời gian và dễ bỏ sót thông tin quan trọng. |
| 2 | VinFast    | Repetitive       | Nhân viên CSKH phải đọc, phân loại và trả lời hàng nghìn ticket hỗ trợ khách hàng mỗi ngày.                          |
| 3 | Vinhomes   | Stakeholder Pain | Ban quản lý nhận nhiều yêu cầu sửa chữa, phản ánh từ cư dân và thường mất thời gian điều phối đúng bộ phận xử lý.    |
| 4 | Xanh SM    | Stakeholder Pain | Tài xế phàn nàn về việc hệ thống gợi ý điểm đón khách chưa tối ưu, dẫn đến thời gian chờ và quãng đường rỗng cao.    |
| 5 | Vinpearl   | AI-upgrade       | Nhân viên tư vấn phải trả lời lặp lại các câu hỏi về phòng, giá và dịch vụ trước khi khách đặt phòng.                |

---

# QUICK PROBLEM CARD #1

## Bài toán

**Tự động tóm tắt hồ sơ bệnh án trước khám**

### Công ty thành viên

* [x] Vinmec
* [ ] VinFast
* [ ] Xanh SM
* [ ] Vinhomes
* [ ] Khác

### Ai đang đau (Actor)?

Bác sĩ khám ngoại trú.

### Workflow thủ công hiện tại

1. Mở hồ sơ bệnh án.
2. Đọc lịch sử khám.
3. Đọc xét nghiệm và đơn thuốc cũ.
4. Tự tổng hợp thông tin trước khi khám.

### Bước nào tốn thời gian/lỗi nhất?

Đọc và tổng hợp hồ sơ bệnh án.

**Thời gian xử lý:** khoảng 10 phút/lượt.

### AI có thể hỗ trợ ở bước nào?

Tự động tóm tắt hồ sơ và highlight các thông tin quan trọng.

### Metric thành công

Giảm thời gian chuẩn bị từ **10 phút xuống dưới 2 phút**.

### Quick Architecture

* [ ] No AI
* [ ] Rule
* [x] LLM
* [ ] Agent

---

# QUICK PROBLEM CARD #2

## Bài toán

**Tự động phân loại và phản hồi ticket CSKH**

### Công ty thành viên

* [x] VinFast
* [ ] Xanh SM
* [ ] Vinhomes
* [ ] Vinmec
* [ ] Khác

### Ai đang đau (Actor)?

Nhân viên Customer Support.

### Workflow thủ công hiện tại

1. Nhận ticket.
2. Đọc nội dung.
3. Phân loại vấn đề.
4. Soạn phản hồi hoặc chuyển bộ phận liên quan.

### Bước nào tốn thời gian/lỗi nhất?

Phân loại ticket.

**Thời gian xử lý:** khoảng 6 phút/ticket.

### AI có thể hỗ trợ ở bước nào?

Tự động phân loại, đề xuất phản hồi và route ticket.

### Metric thành công

Giảm thời gian xử lý từ **6 phút xuống dưới 1 phút/ticket**.

### Quick Architecture

* [ ] No AI
* [ ] Rule
* [ ] LLM
* [x] Agent

---

# QUICK PROBLEM CARD #3

## Bài toán

**Tự động điều phối yêu cầu cư dân**

### Công ty thành viên

* [x] Vinhomes
* [ ] VinFast
* [ ] Xanh SM
* [ ] Vinmec
* [ ] Khác

### Ai đang đau (Actor)?

Nhân viên ban quản lý tòa nhà.

### Workflow thủ công hiện tại

1. Nhận phản ánh cư dân.
2. Đọc nội dung.
3. Phân loại yêu cầu.
4. Chuyển đội kỹ thuật hoặc dịch vụ xử lý.

### Bước nào tốn thời gian/lỗi nhất?

Phân loại và điều phối yêu cầu.

**Thời gian xử lý:** khoảng 15 phút/lượt.

### AI có thể hỗ trợ ở bước nào?

Tự động phân loại, xác định mức độ ưu tiên và route ticket.

### Metric thành công

Giảm thời gian điều phối từ **15 phút xuống dưới 3 phút**.

### Quick Architecture

* [ ] No AI
* [ ] Rule
* [ ] LLM
* [x] Agent
