# ĐẶC TẢ YÊU CẦU CHỨC NĂNG GAME & CATEGORY

## 1. Dành cho người dùng (Guest/User)
* **Xem danh sách Game:** Người dùng có thể xem danh sách game. Hệ thống phải phân trang (ví dụ 10 game/trang).
* **Tìm kiếm & Lọc:** Người dùng có thể tìm game theo từ khóa (keyword) và lọc theo thể loại (category_id).
* **Xem chi tiết Game:** Người dùng click vào game sẽ xem được chi tiết dựa trên đường dẫn `slug` (VD: `/games/lien-minh-huyen-thoai`).

## 2. Dành cho Quản trị viên (Admin)
* **Thêm mới Game:** Admin điền form gồm: Tên game, Thể loại, Nhà phát triển, Nền tảng, Ngày phát hành, Mô tả, và Upload ảnh cover.
* **Quy tắc tạo Slug:** Khi Admin nhập Tên game, hệ thống tự động tạo `slug` duy nhất (unique). Không cho phép trùng slug.
* **Ẩn/Xóa Game (Soft Delete):** Admin có thể đổi trạng thái (status) của game để ẩn khỏi trang chủ, thay vì xóa hẳn data.
* **Ràng buộc Thể loại (Category):** Không được xóa một Category nếu đang có Game thuộc Category đó.
