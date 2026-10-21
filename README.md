# E-commerce UI Improvement

**Môn học:** Phát triển ứng dụng WEB/TMĐT  
**Giảng viên:** TS. Nguyễn Mạnh Tuấn – tuannm@ueh.edu.vn  

---

## 1. Giới thiệu
Bài tập cá nhân thực hiện khảo sát website thương mại điện tử thực tế và đề xuất cải tiến giao diện Thẻ sản phẩm (Product Card). Sản phẩm cải tiến tập trung vào việc tối ưu hóa khả năng hiển thị thông tin giá bán và đảm bảo giao diện hiển thị mượt mà trên cả máy tính lẫn thiết bị di động (Responsive Web Design).

## 2. Website tham khảo
- **Tên website:** Shopee Việt Nam
- **URL:** https://shopee.vn
- **Khu vực đã khảo sát:** Trang chủ, Danh mục sản phẩm, Chi tiết sản phẩm, Tìm kiếm, Giỏ hàng.

## 3. Chức năng
- Hiển thị danh sách sản phẩm nổi bật dưới dạng lưới (Product Grid).
- Hiển thị hình ảnh, tên sản phẩm, giá bán khuyến mãi, giá gốc gạch ngang, nhãn giảm giá (%) và đánh giá sao.
- Bố cục hỗ trợ nhiều kích thước màn hình: Tự động chuyển đổi linh hoạt giữa giao diện Desktop (4 cột) và Mobile (2 cột).
- Tích hợp nút "Thêm vào giỏ" hỗ trợ tương tác người dùng.

## 4. Công nghệ
- **HTML5:** Sử dụng các thẻ chuẩn Semantic (`<article>`, `<section>`, `<figure>`).
- **CSS3:** Áp dụng CSS Grid, Flexbox, CSS Variables và Media Queries `@media (max-width: 768px)`.

## 5. Cách chạy
1. Tải thư mục dự án về máy tính.
2. Mở trực tiếp file `index.html` bằng các trình duyệt web phổ biến (Google Chrome, Microsoft Edge, Mozilla Firefox).
3. Sử dụng công cụ DevTools (`F12`) để trải nghiệm thử chế độ giao diện trên điện thoại di động.

## 6. Cải tiến đã thực hiện
- **Vấn đề ban đầu:** Trên màn hình di động, thẻ sản phẩm của Shopee bị thu hẹp, thông tin giá bán và tỷ lệ giảm giá hiển thị chèn ép, tên sản phẩm quá dài dễ làm lệch hàng và vỡ khung.
- **Thay đổi đã thực hiện:** 
  - Đã thiết kế lại bố cục thẻ sản phẩm gọn gàng, làm nổi bật giá khuyến mãi.
  - Sử dụng CSS Grid tự động co giãn 2 cột trên điện thoại.
  - Tự tay thêm thuộc tính CSS `-webkit-line-clamp: 2` kết hợp `overflow: hidden` giúp khống chế tên sản phẩm chỉ hiển thị tối đa 2 dòng kèm dấu `...`, giữ chiều cao các thẻ sản phẩm luôn cân bằng.

## 7. Hỗ trợ từ AI
- **Phần AI hỗ trợ:** Đề xuất bảng phân tích UI/UX 5 khu vực của Shopee, hỗ trợ tạo cấu trúc mã HTML5 và CSS3 Responsive mẫu cho 4 thẻ sản phẩm.
- **Phần tôi đã kiểm tra & chỉnh sửa:**
  - Tự kiểm chứng thực tế website Shopee bằng Chrome DevTools và loại bỏ các nhận xét chưa chính xác của AI về tốc độ tải trang.
  - Tự tay bổ sung và tinh chỉnh thuộc tính cắt tên sản phẩm (`line-clamp`) trong CSS để giải quyết triệt để lỗi vỡ khung.
  - Kiểm tra hoàn thiện khả năng hiển thị responsive trên nhiều độ phân giải màn hình khác nhau (Desktop, Tablet, Mobile).