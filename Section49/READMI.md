### Grid Layout:

- Grid Css là một phương pháp sắp xếp và cấu trúc trang web dựa trên lưới
- Cho phép chia trang thành các ô hình chữ nhật và điều khiển vị trí của các phần tử trên trang

- Cấu tạo Bao gôm:

- Grid Ceil -> các dòng,cột kẻ
- Grid Line -> các ô (tạo thành từ các dòng kẻ)
- Grid Track (Row) -> tập hợp các ô theo chiều ngang
- Grid Track (Column) -> tập hợp các ô theo chiều dọc
- Grid Area -> tập hợp các ô nhỏ Ceil

//==========================================================//

### Khi nào nên dùng Grid Layout và Flexbox Layout:

## Flexbox Layout:

- dùng cho giao diện 1 chiều
- canh chỉnh linh hoạt
- Tỷ lệ co giãn
- Đơn giản

## Grid Layout:

- dùng cho giao diện 2 chiều
- Bố cục phức tạp
- Kiểm soát chính xác
- Responsive

==> Trong thực tế ta kết hợp cả Flexbox và Grid để tăng độ tối ưu

//==========================================================//

### Grid chia hàng(Row) và cột(Column) and Gap:

-> Khi đặt class cha là "grid" hoặc "inline-grid" -> tất cả các phần tử rời khỏi luồng thông thường và tuân theo quy tắc lưới của "grid"

-> grid-template-columns và grid-template-rows -> căn chỉnh
-> gap -> grid-row-gap và grid-column-gap quy định khoảng cách
-> Shorthand: gap: 10px 10px
