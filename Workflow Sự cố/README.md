# Workflow Sự cố – KPI IT từ Ticket Bitrix24

Tài liệu mô tả giải pháp tính điểm KPI nhân viên IT dựa trên workflow **Service Request – Yêu cầu dịch vụ** trên Bitrix24.

## Workflow chuẩn

`Mới tiếp nhận → Phân loại & chuẩn bị → Đang thực hiện → Chờ KH → Hoàn thành/Đóng ticket`

## Nguyên tắc KPI

- Bitrix24 Ticket là nguồn dữ liệu gốc.
- KPI được tính từ dữ liệu công việc thực tế, không yêu cầu IT nhập KPI riêng.
- SLA được xác định theo Priority/SLA của từng Ticket.
- Thời gian ở trạng thái **Chờ KH/bên thứ ba** có thể được Pause SLA theo quy định.
- On-Time chỉ tính Ticket có Deadline hợp lệ.
- Ticket bắt buộc có Deadline nhưng không có Deadline được ghi nhận là vi phạm Process Compliance.
- Workload dùng điểm quy đổi theo độ khó thay vì chỉ đếm số Ticket.

## Bộ KPI mô phỏng

| KPI | Trọng số |
|---|---:|
| Productivity / Workload | 20% |
| SLA Compliance | 30% |
| On-Time Completion | 15% |
| Quality | 15% |
| Process Compliance | 10% |
| First Response & Escalation | 10% |
| **Tổng** | **100%** |

## SLA mẫu mô phỏng

| Priority | Response | Resolution | Hệ số |
|---|---:|---:|---:|
| P1 | 15 phút | 4 giờ | 4 |
| P2 | 30 phút | 8 giờ | 3 |
| P3 | 2 giờ | 24 giờ | 2 |
| P4 | 4 giờ | 48 giờ | 1 |

> Các ngưỡng trên là dữ liệu mô phỏng để kiểm thử công thức; khi áp dụng chính thức phải thay bằng SLA thực tế của M-Techcare.

## File mô phỏng

Xem thư mục `Excel/` để sử dụng file Excel tính KPI và kiểm thử các tình huống.
