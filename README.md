# Taxi'sGrab Rạch Giá LuXuRy - Dịch Vụ Đặt Xe Taxi Trực Tuyến

Website giới thiệu dịch vụ và đặt xe taxi 24/7 hàng đầu tại Rạch Giá, An Giang, Kiên Giang và các tỉnh miền Tây.

## Project Overview
This repository contains the static website source for **Taxi'sGrab Rạch Giá LuXuRy** (`https://taxigrabrachgia.netlify.app`), providing taxi booking services in Rạch Giá, Kiên Giang, An Giang, and the Mekong Delta region.

## Key Files & Structure
- `index.html`: Main landing page featuring Hero, Fleet Showcase, Price Cards, Popular Route Pricing Table, Shortened 5-field Booking Form, and Fixed Dual Contact Bar.
- `__forms.html`: Static skeleton form file used by Netlify build bot for form detection.
- `cam-on.html`: Thank you page displayed upon successful form submission.
- `chinh-sach-bao-mat.html`: Privacy policy page.
- `chinh-sach-thanh-toan.html`: Payment policy page.
- `README.md`: General description and user instructions.

## Important Design Decisions & Conventions
1. **Font & Typography**: All Vietnamese text relies on `Be Vietnam Pro` (`'Be Vietnam Pro', sans-serif`). Avoid fallback fonts like Georgia or Trebuchet MS for body copy to prevent distorted Vietnamese glyphs/accents.
2. **Booking Form (`#dat-xe`)**:
   - Strictly 5 required fields: `ho-ten`, `so-dien-thoai`, `loai-xe`, `diem-don`, `diem-den`.
   - Target notification email: `thienduongkg3536@gmail.com`.
   - Netlify Forms + FormSubmit integration (`action="https://formsubmit.co/thienduongkg3536@gmail.com"` and `data-netlify="true"`).
3. **Contact Action Buttons**:
   - Always pair **Nút Gọi** (`tel:0775856456`) and **Nút Chat Zalo** (`https://zalo.me/0328181085`).
   - Sticky floating bar (`.fixed-action-bar`) positioned at the bottom-left corner of the screen, stacked vertically (Nút Gọi on top, Nút Chat Zalo below) with a rotating La Bàn map compass highlight badge and mobile-optimized compact styling.

## Các Tính Năng Chính
- **Biểu mẫu đặt xe gọn 5 mục**: Họ và Tên, Số điện thoại, Loại xe, Điểm đón, Điểm đến.
- **Tích hợp gửi Email tự động**: Gửi toàn bộ thông tin đơn đặt xe về email `thienduongkg3536@gmail.com` thông qua Netlify Forms & FormSubmit.
- **Phông chữ tiếng Việt chuẩn**: Sử dụng Google Font `Be Vietnam Pro` hiển thị sắc nét, thẳng hàng, không bị lỗi phông hay xô lệch.
- **Nút tương tác kép Nút Gọi + Nút Chat Zalo**: Bố trí đồng bộ từ Topbar, Header, Hero, Bảng Giá, Đội Xe đến Thanh cuộn cố định (Sticky Action Bar).
- **Hình ảnh xe đời mới**: Hình ảnh thực tế chất lượng cao cho xe 4 chỗ, 7 chỗ, 7 chỗ Kia Carnival VIP, 16 chỗ Hyundai Solati/Ford Transit.
- **Bảng giá chi tiết & Giới thiệu tuyến xe**: Cung cấp bảng giá niêm yết theo kilomet và bảng giá trọn gói cho các tuyến đường phổ biến từ Rạch Giá đi Cần Thơ, Sài Gòn, Hà Tiên, Châu Đốc, Phú Quốc...

## Công Nghệ Sử Dụng
- **HTML5 & CSS3**: Thiết kế chuẩn Responsive, tối ưu hiển thị mượt mà trên Điện thoại, Máy tính bảng và Máy tính bàn.
- **Be Vietnam Pro**: Font chữ Google chuẩn Unicode tiếng Việt.
- **Font Awesome 6**: Hệ thống biểu tượng trực quan.
- **Netlify Forms & FormSubmit**: Xử lý phản hồi đơn đặt xe serverless gửi trực tiếp về email nhà xe.

## Hướng Dẫn Chạy Cục Bộ (Local)
Mở file `index.html` trực tiếp bằng bất kỳ trình duyệt web nào (Chrome, Edge, Safari, Firefox), hoặc sử dụng extension Live Server trong VS Code để xem trang web.
Huy hiệu trạng thái triển khai :
[![Netlify Status](https://api.netlify.com/api/v1/badges/d0b5ee9f-4420-4379-8f1d-f3c437823c27/deploy-status)](https://app.netlify.com/projects/luxurywebtaxi/deploys)
