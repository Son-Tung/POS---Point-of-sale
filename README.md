# 📦 HỆ THỐNG WEBSITE HỖ TRỢ BÁN HÀNG (POS)

## 🧾 Giới thiệu

Dự án **Website Hỗ Trợ Bán Hàng (Point of Sale - POS)** là hệ thống tích hợp giúp quản lý toàn bộ quy trình bán hàng, tồn kho, thanh toán và chăm sóc khách hàng cho các cửa hàng bán lẻ. Dự án được xây dựng nhằm đơn giản hóa các thao tác bán hàng và nâng cao trải nghiệm người dùng, đồng thời cung cấp các công cụ phân tích hữu ích cho chủ doanh nghiệp.

## 🎯 Mục tiêu chính

* Tự động hóa và tối ưu quy trình bán hàng.
* Quản lý kho hàng và khách hàng hiệu quả.
* Tích hợp xử lý thanh toán đa phương thức.
* Báo cáo, phân tích số liệu phục vụ ra quyết định kinh doanh.

## 🛠️ Công nghệ sử dụng

* **Ngôn ngữ lập trình**: Java
* **Framework**: Spring Boot
* **Cơ sở dữ liệu**: MySQL
* **IDE**: IntelliJ IDEA
* **Kiến trúc**: Mô hình MVC
* **Giao diện**: JavaFX / Swing (nếu có UI client), hoặc Thymeleaf (nếu frontend dạng web)

## 📌 Các chức năng chính

### 1. Quản lý khách hàng

* Thêm/sửa/xóa khách hàng.
* Tìm kiếm và hiển thị danh sách.
* Lưu trữ thông tin như tên, địa chỉ, mức lương.

### 2. Quản lý sản phẩm

* Thêm/sửa/xóa sản phẩm.
* Cập nhật tồn kho.
* Quản lý mô tả, giá cả và số lượng sản phẩm.

### 3. Quản lý đơn hàng

* Tạo đơn hàng mới.
* Tính toán tổng giá trị, chiết khấu, cập nhật tồn kho.
* In hóa đơn và xử lý thanh toán.

### 4. Lịch sử mua hàng

* Xem chi tiết đơn hàng cũ.
* Tra cứu theo mã đơn hàng, khách hàng, ngày đặt.

### 5. Báo cáo và phân tích (nếu có)

* Doanh số bán hàng theo thời gian.
* Sản phẩm bán chạy.
* Hiệu suất bán hàng.

## 🧱 Cơ sở dữ liệu

### Các bảng chính:

* `customer`: lưu thông tin khách hàng.
* `item`: lưu thông tin mặt hàng.
* `orders`: thông tin đơn hàng.
* `order_details`: chi tiết đơn hàng.
* `payment`: thông tin thanh toán.

### Quan hệ:

* 1 khách hàng ↔ nhiều đơn hàng.
* 1 đơn hàng ↔ nhiều sản phẩm.
* 1 sản phẩm ↔ nhiều chi tiết đơn hàng.
* 1 đơn hàng ↔ 1 thanh toán.

## 📂 Cấu trúc dự án 

```
BackEnd/
├── pom.xml                     # File cấu hình Maven
├── src/
│   └── main/
│       ├── java/              # Mã nguồn Java (controller, service, model, repository)
│       └── resources/         # File cấu hình, templates (nếu có)
└── target/
    └── classes/
        └── application.properties
```

```
FrontEnd/
├── index.html                  # Trang chính của giao diện
├── controllers/               # JavaScript điều khiển logic trang (theo MVC)
├── pages/                     # Các trang chức năng (customer.html, order.html, v.v.)
├── util/                      # JS dùng chung: alert, validate,...
├── assets/
│   ├── Bootstrap/             # Bootstrap 5.2.1 + bootstrap-icons
│   ├── jQuery/                # Thư viện jQuery 3.6.1
│   └── styles/                # style.css, sweetalert,...
```

## ⚙️ Cách chạy dự án

1. Clone project:

   ```bash
   git clone <link-repo>
   ```
2. Mở bằng IntelliJ IDEA hoặc Eclipse.
3. Cấu hình database trong `application.properties`.
4. Chạy file `Application.java` (Spring Boot Main).
5. Truy cập tại: `http://localhost:8080` (nếu có frontend web).

## ✅ Tác giả

* **Ma Duy Long** – BIT220097
* **Nguyễn Sơn Tùng** – BIT220166
* Giảng viên hướng dẫn: *Nguyễn Ngọc Khải*

## 📅 Thời gian thực hiện

Hà Nội, tháng 08 năm 2024
