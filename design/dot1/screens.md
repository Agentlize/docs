# Danh sách màn hình — Đợt 1 Vaohoc.vn

## Web học sinh (prefix: `hs-`)

| File | Màn hình | Mục đích | Dữ liệu | Hành động | Trạng thái |
|------|----------|----------|----------|-----------|------------|
| hs-home | Trang chủ | Landing page thầy | Banner, khóa nổi bật, combo, tài liệu, SĐT/Zalo | Xem khóa, đăng ký, đăng nhập | Chưa đăng nhập / đã đăng nhập |
| hs-register | Đăng ký | Tạo tài khoản | Form email+mật khẩu, nút Google/Facebook | Đăng ký, chuyển đăng nhập | Mặc định / lỗi validation / đang gửi |
| hs-login | Đăng nhập | Vào tài khoản | Form email+mật khẩu, nút Google/Facebook | Đăng nhập, quên MK, chuyển đăng ký | Mặc định / lỗi / đang gửi |
| hs-verify-email | Xác nhận email | Nhắc xác nhận | Thông báo đã gửi email | Gửi lại | Đã gửi / gửi lại thành công |
| hs-forgot-pw | Quên mật khẩu | Đặt lại MK | Form email | Gửi link | Mặc định / đã gửi / email không tồn tại |
| hs-reset-pw | Đặt lại mật khẩu | Nhập MK mới | Form mật khẩu mới | Lưu | Mặc định / thành công / link hết hạn |
| hs-courses | Danh sách khóa học | Duyệt khóa | Thẻ khóa: ảnh, tên, giá, giá gốc, danh mục | Lọc danh mục, xem chi tiết | Có khóa / trống |
| hs-course-detail | Chi tiết khóa | Xem nội dung + mua | Tên, mô tả, mục lục chương-bài, giá, video học thử | Thêm giỏ, mua ngay, xem học thử | Chưa mua / đã mua / video khóa |
| hs-lesson | Bài học | Học video + tài liệu | Video YouTube, tài liệu, lời giải, link nhóm | Xem video, tải tài liệu, xem lời giải | Đang học / video khóa |
| hs-exams | Danh sách đề thi | Chọn đề | Tên đề, số câu, thời gian, trạng thái | Vào thi, xem kết quả cũ | Có đề / trống / đề chưa mở / đề đã khóa |
| hs-exam-take | Làm bài | Thi | Câu hỏi, đáp án, đồng hồ, công thức KaTeX | Chọn đáp án, nộp bài, chuyển câu | Đang làm / hết giờ tự nộp / hết lượt |
| hs-exam-result | Kết quả thi | Xem điểm + lời giải | Điểm, đáp án đúng/sai, lời giải, thời gian | Xem lời giải, làm lại, bảng xếp hạng | Có lời giải / không cho xem lời giải |
| hs-leaderboard | Bảng xếp hạng | So điểm | Danh sách: tên, điểm, thời gian, hạng | — | Có dữ liệu / trống |
| hs-docs | Tài liệu PDF | Tìm + xem PDF | Danh mục cây, danh sách tài liệu, thanh tìm kiếm | Tìm, xem PDF, tải (nếu được) | Có tài liệu / trống / đang tải |
| hs-doc-viewer | Xem PDF | Đọc PDF trực tuyến | PDF viewer nhúng | Phóng to, chuyển trang | Đang tải / đã tải / lỗi |
| hs-cart | Giỏ hàng | Xem + sửa giỏ | Danh sách khóa/combo, giá, tổng tiền | Xóa, thanh toán, nhập mã kích hoạt | Có hàng / trống |
| hs-checkout | Thanh toán | Chuyển khoản | Mã VietQR, số tiền, tài khoản thầy, mã đơn | Quét QR, upload ảnh chuyển khoản | Hiện QR / đã gửi ảnh / chờ xác nhận |
| hs-orders | Đơn hàng | Lịch sử mua | Danh sách đơn: mã, ngày, tổng, trạng thái | Xem chi tiết | Có đơn / trống |
| hs-activate | Nhập mã kích hoạt | Mở khóa bằng mã | Form nhập mã | Kích hoạt | Mặc định / thành công / mã sai / mã đã dùng |
| hs-profile | Hồ sơ | Sửa thông tin | Tên, email, avatar | Sửa, đổi mật khẩu | Xem / đang sửa |
| hs-my-courses | Khóa đã mua | Truy cập nhanh | Danh sách khóa đã mua, % (placeholder) | Vào học | Có khóa / trống |

## Quản trị thầy (prefix: `admin-`)

| File | Màn hình | Mục đích | Dữ liệu | Hành động | Trạng thái |
|------|----------|----------|----------|-----------|------------|
| admin-login | Đăng nhập | Vào quản trị | Form email, nút Google/Facebook | Đăng nhập | Mặc định / lỗi |
| admin-dashboard | Dashboard | Tổng quan | Số đơn chờ, học sinh mới (placeholder) | Chuyển đến các mục | Mặc định |
| admin-brand | Thương hiệu | Cài đặt web | Tên, logo, màu chủ đạo, SĐT, Zalo, MXH, favicon | Lưu, xem trước web | Mặc định / đang lưu / đã lưu |
| admin-bank | Tài khoản NH | Nhận tiền | Tên NH, số TK, tên chủ TK | Lưu | Mặc định / đã lưu |
| admin-homepage | Trang chủ web | Sắp xếp khu vực | Danh sách block: banner, khóa, combo, tài liệu | Kéo thả, bật/tắt, chọn nội dung | Mặc định |
| admin-courses | Danh sách khóa | Quản lý khóa | Bảng: tên, danh mục, giá, trạng thái, số HS | Tạo, sửa, bật/tắt | Có khóa / trống |
| admin-course-edit | Sửa khóa | Nội dung khóa | Tên, mô tả, ảnh, danh mục, giá, giá gốc | Lưu, thêm chương | Tạo mới / sửa |
| admin-chapter-edit | Sửa chương + bài | Nội dung bài | Danh sách bài: tên, link YouTube, tài liệu, lời giải, học thử, ngày mở | Thêm/sửa/xóa bài, kéo thả thứ tự | Mặc định |
| admin-exams | Danh sách đề | Quản lý đề | Bảng: tên, số câu, loại, trạng thái | Tạo, sửa, nhập Word | Có đề / trống |
| admin-exam-edit | Sửa đề | Nội dung đề | Tên, thời gian, lượt, lời giải, lịch mở/khóa, bảng xếp hạng | Lưu cài đặt | Tạo mới / sửa |
| admin-exam-questions | Câu hỏi | Soạn câu | Danh sách câu: nội dung, dạng, đáp án, lời giải, KaTeX | Thêm/sửa/xóa câu, kéo thả | Mặc định |
| admin-exam-import | Nhập Word | Upload đề | Upload zone, preview kết quả parse | Upload, xem trước, xác nhận | Chưa upload / đang xử lý / xem trước / lỗi parse |
| admin-docs | Tài liệu PDF | Quản lý tài liệu | Cây danh mục, danh sách file | Tạo danh mục, upload, xóa | Có tài liệu / trống |
| admin-combos | Combo | Quản lý combo | Bảng: tên, khóa trong combo, giá | Tạo, sửa | Có combo / trống |
| admin-combo-edit | Sửa combo | Nội dung combo | Tên, chọn khóa, giá, giá gốc | Lưu | Tạo mới / sửa |
| admin-orders | Đơn hàng | Xác nhận đơn | Bảng: mã, HS, tổng, trạng thái, ngày | Lọc trạng thái, xem chi tiết | Có đơn / trống |
| admin-order-detail | Chi tiết đơn | Xác nhận | Thông tin HS, khóa, ảnh chuyển khoản, tổng tiền | Xác nhận / từ chối | Chờ / đã xác nhận / đã từ chối |
| admin-codes | Mã kích hoạt | Quản lý mã | Bảng: mã, khóa/combo, trạng thái, HS dùng | Tạo hàng loạt, xem | Có mã / trống |
| admin-codes-generate | Tạo mã | Tạo hàng loạt | Chọn khóa/combo, số lượng | Tạo, tải danh sách | Form / kết quả |
| admin-students | Học sinh | Quản lý HS | Bảng: tên, email, ngày ĐK, khóa đã mua | Lọc theo khóa, xuất CSV, xem chi tiết | Có HS / trống |
| admin-student-detail | Chi tiết HS | Xem thông tin | Hồ sơ, danh sách khóa, đơn hàng | — | Mặc định |
