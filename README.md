# FinAuto_App_FE 📱

**FinAuto_App_FE** là ứng dụng di động quản lý thu chi tiện lợi và chuyên nghiệp dành cho các chủ cửa hàng. Ứng dụng được xây dựng trên nền tảng **Flutter** với thiết kế hiện đại, tinh tế theo phong cách **Vivid Kinetic** và các trải nghiệm chuyển động mượt mà.

---

## ✨ Tính năng chính

- **Màn hình chào (Splash Screen):** Màn hình khởi đầu ấn tượng với hiệu ứng tải trang chuyên nghiệp.
- **Đăng nhập (Login Screen):** Hỗ trợ đăng nhập bảo mật cho chủ cửa hàng để quản lý dữ liệu cá nhân.
- **Trang chủ & Báo cáo (Dashboard Screen):**
  - Biểu đồ tròn trực quan (**Donut Chart**) phân tích tỷ lệ thu chi thực tế.
  - Thống kê tổng quan số dư, tổng thu và tổng chi.
  - Danh sách lịch sử giao dịch gần đây được cập nhật liên tục.
- **Quản lý Thu Chi (Thu Chi Screen):**
  - Thêm mới các khoản thu/chi dễ dàng với biểu mẫu nhập liệu thân thiện.
  - Quản lý danh sách các giao dịch (Xem chi tiết, xóa giao dịch).
- **Hồ sơ (Profile Screen):** Quản lý thông tin cá nhân của chủ cửa hàng và các cài đặt ứng dụng.
- **Thanh điều hướng dưới (Bottom Navigation Bar):** Shell điều hướng mượt mà giữa các phân hệ Trang chủ, Thu Chi và Hồ sơ.

---

## 🎨 Thiết kế & Giao diện (Design System)

Ứng dụng áp dụng bộ quy chuẩn thiết kế hiện đại và nhất quán:
- **Bảng màu Vivid Kinetic:**
  - `Primary`: `#B31F56` (Màu hồng đậm sang trọng)
  - `Primary Container`: `#FF5C8D`
  - `Secondary`: `#5C6300`
  - `Secondary Container`: `#DCE944`
  - `Background/Surface`: `#F8F9FA` (Trắng xám nhẹ nhàng, dễ chịu cho mắt)
- **Typography:** Sử dụng phông chữ cao cấp **Roboto Flex** được tích hợp qua Google Fonts để mang lại giao diện văn bản sắc nét và chuyên nghiệp giống bản vẽ thiết kế.
- **Định dạng tiền tệ:** Tích hợp gói `intl` hiển thị chuẩn tiền tệ Việt Nam (Ví dụ: `1.500.000đ`).

---

## 🛠️ Công nghệ sử dụng

- **Framework:** Flutter (SDK `>=3.0.0 <4.0.0`)
- **Ngôn ngữ:** Dart
- **Thư viện chính:**
  - `google_fonts: ^6.1.0` - Hỗ trợ font chữ Roboto Flex.
  - `intl: ^0.19.0` - Hỗ trợ định dạng ngôn ngữ & tiền tệ Việt Nam.

---

## 📂 Cấu trúc thư mục dự án

```text
lib/
├── main.dart               # Điểm khởi chạy ứng dụng & định nghĩa Routes, Theme
├── models/
│   └── transaction.dart    # Model dữ liệu cho Giao dịch (Thu/Chi)
├── screens/
│   ├── splash_screen.dart  # Màn hình Splash
│   ├── login_screen.dart   # Màn hình Đăng nhập
│   ├── dashboard_screen.dart # Màn hình Dashboard (Trang chủ)
│   ├── thu_chi_screen.dart # Màn hình Quản lý Thu/Chi
│   ├── profile_screen.dart # Màn hình Hồ sơ người dùng
│   └── side_drawer.dart    # Drawer menu điều hướng phụ
└── widgets/
    ├── donut_chart_painter.dart # Widget vẽ biểu đồ tròn (Donut Chart) bằng Canvas
    └── transaction_item_card.dart # Widget hiển thị thẻ thông tin giao dịch lẻ
```

---

## 🚀 Hướng dẫn cài đặt & Chạy ứng dụng

### Yêu cầu hệ thống
- Đã cài đặt Flutter SDK (phiên bản 3.0.0 trở lên).
- Thiết bị giả lập (Emulator/Simulator) hoặc thiết bị thật đã bật chế độ gỡ lỗi (Developer Mode).

### Các bước thực hiện

1. **Tải mã nguồn về máy:**
   ```bash
   git clone https://github.com/NguyenBaMinhTien/FinAuto_App_FE.git
   cd FinAuto_App_FE
   ```

2. **Cài đặt các gói phụ thuộc:**
   ```bash
   flutter pub get
   ```

3. **Chạy ứng dụng:**
   - Để chạy trên thiết bị đang kết nối:
     ```bash
     flutter run
     ```
   - Hoặc chạy ở chế độ Release để tối ưu hóa hiệu năng:
     ```bash
     flutter run --release
     ```
