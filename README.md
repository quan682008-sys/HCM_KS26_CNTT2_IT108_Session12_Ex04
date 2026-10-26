# HCM_KS26_CNTT2_IT108_Session12_Ex04
# Bài 4: Chuẩn hóa quy trình quản lý bệnh án điện tử

##  Phần 1. Phân tích

| Tiêu chí | Yêu cầu chức năng | Yêu cầu phi chức năng |
|---|---|---|
| Định nghĩa | Mô tả hệ thống làm được những gì. | Mô tả hệ thống hoạt động như thế nào (hiệu năng, bảo mật, vận hành). |
| Trọng tâm đề bài | **Khám bệnh:**<br>- Tiếp nhận và tạo hồ sơ bệnh nhân mới.<br>- Đặt lịch khám, phân bổ bác sĩ/phòng khám.<br>- Nhập kết quả khám, đơn thuốc, lịch sử bệnh án.<br>- Xuất đơn thuốc, hóa đơn và hẹn tái khám. | **Bảo mật dữ liệu y tế:**<br>- Bảo mật (Security): Mã hóa dữ liệu lưu trữ và truyền tải.<br>- Phân quyền: Chỉ bác sĩ phụ trách mới xem được chi tiết bệnh án, lễ tân chỉ xem thông tin khác.<br>- Sao lưu (Backup): Sao lưu định kỳ tự động, có phương án phục hồi sau sự cố. |

---

##  Phần 2. Triển khai

###  Cấu trúc lưu trữ đám mây (Cloud Storage & Database)

Sử dụng cơ sở dữ liệu trên Cloud và kết hợp dịch vụ lưu trữ file an toàn để lưu trữ hình ảnh X-quang, kết quả xét nghiệm,...

###  Đồng bộ và tra cứu

Tập trung hóa dữ liệu: bỏ lưu trữ rời rạc trên từng máy cá nhân, toàn bộ dữ liệu đồng bộ lên Cloud để đảm bảo tính đồng bộ, hỗ trợ tra cứu nhanh chóng theo mã bệnh nhân, số CCCD hoặc Số điện thoại.
