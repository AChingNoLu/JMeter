Kiểm tra hiệu năng API
1. Mục tiêu
Sử dụng Apache JMeter để xây dựng kịch bản kiểm thử (test script) mô phỏng hành vi người dùng truy cập API thời tiết tại địa chỉ: [https://openweathermap.org/current](https://openweathermap.org/current).

Thực thi kịch bản kiểm tra và thu thập dữ liệu kết quả thực tế.

Phân tích các chỉ số hiệu năng quan trọng bao gồm: thời gian phản hồi (response time), tỷ lệ yêu cầu thành công, tỷ lệ yêu cầu thất bại, v.v.

Đưa ra đánh giá và kết luận khách quan về hiệu năng của API dựa trên số liệu phân tích.

2. Kịch bản kiểm tra (Test Plan)
Thread Group:

Số lượng người dùng ảo (Threads): 100

Thời gian chạy (Duration): 60 giây

Thời gian khởi động (Ramp-up period): 10 giây

HTTP Request:

URL: [https://openweathermap.org/current](https://openweathermap.org/current)

Method: GET

Content encoding: UTF-8

Listeners (Công cụ ghi nhận kết quả):

View Results Tree

Aggregate Report

3. Kết quả kiểm tra & Phân tích
Tổng quan kết quả:

Số lượng yêu cầu thành công: 996 / 1000 (đạt 99,6%)

Số lượng yêu cầu thất bại: 4 / 1000 (chiếm 0,4%)

Thời gian phản hồi trung bình (Average Response Time): 10 ms (hoặc bổ sung đơn vị tùy theo báo cáo thực tế của bạn)

4. Kết luận
API thời tiết duy trì được hiệu năng ổn định và độ tin cậy cao dưới tải kiểm thử. Tỷ lệ thành công vượt trội (99,6%) trong khi tỷ lệ lỗi ở mức tối thiểu (0,4%). Bên cạnh đó, thời gian phản hồi trung bình rất nhanh, đáp ứng tốt yêu cầu kỹ thuật cho các tác vụ truy vấn thời tiết thời gian thực.
