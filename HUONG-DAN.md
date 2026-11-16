# SoftsKit 3.2.0 — WPF

Giao diện theo mẫu đã chọn: bo góc, nền chuyển màu xanh/xám SVTECH, menu trái chỉ có chữ và icon thật trong danh sách phần mềm. Cửa sổ mặc định 1180×700, có bố cục gọn cho cửa sổ nhỏ.

- **Phần mềm:** chọn app trong danh sách, xem lượt cài bên phải; cửa sổ nhỏ chuyển nút thao tác xuống dưới. Giữ cơ chế bộ cài local, tải có kiểm tra hash/chữ ký và hàng đợi gỡ hiện có.
- **Office / Windows:** hai tab con. Đọc tên sản phẩm, phiên bản, tên license và trạng thái kích hoạt của Office. Windows hiển thị phiên bản, có key hay không, loại key và kích hoạt. Không hiển thị key đầy đủ. Office trùng sản phẩm/kiến trúc/ngôn ngữ/thành phần đã biết sẽ không cài lại, trừ khi chọn cài lại.
- **Kiểm tra / Gỡ license:** chọn đúng sản phẩm; có thể gỡ license hoặc xóa host KMS đặt thủ công riêng biệt. Hiển thị nội dung trước khi xác nhận, kiểm tra lại sản phẩm trước và sau thao tác. Không có reset trial/rearm.
- **Dấu hiệu can thiệp:** kiểm tra một số tên công cụ/tác vụ kích hoạt đã biết. KMS hợp lệ và trạng thái đã kích hoạt không đủ để kết luận crack; không ghi nhận dấu hiệu cũng không chứng minh máy sạch.
- **MAC & S/N:** xem MAC Wi-Fi vật lý và serial thiết bị, thêm ghi chú rồi bấm Gửi. Mã 6 số hiện trong hộp thoại lúc gửi. Giữ API và cấu hình triển khai hiện có.
- **Cấu hình → Ứng dụng:** áp dụng profile FortiClient VPN. Bấm chữ **Cấu hình → Thay đổi cấu hình → Thay đổi** để mở trình sửa bằng form hoặc JSON. Màn hình thường ẩn file/editor. Có lưu dự phòng `.bak`; lưu file chưa áp dụng lên FortiClient. Hỗ trợ FortiClient VPN 7.0.5 standalone đã xác minh.
- **Cấu hình → Nguồn điện:** đọc và thay thời gian tắt màn hình/ngủ khi dùng pin/cắm sạc. “Không bao giờ” là 0. Áp dụng cho power plan đang dùng, đọc lại để xác minh và khôi phục nếu ghi lỗi.

Đóng gói WPF x64 tại `Releases/v3.2.0/SoftsKit.exe`. Các bản Releases cũ được giữ nguyên. Không cần dùng `Release-WPF`.

Các kiểm tra thao tác gỡ license, ghi cấu hình VPN, thay nguồn điện và gửi dữ liệu dùng fixture; không thực thi các thao tác này trên máy phát triển. Kiểm tra đọc license và nguồn điện trên máy thật được thực hiện riêng, chỉ đọc. Không thay deployment Google/Sheet trong bản cập nhật desktop này.
