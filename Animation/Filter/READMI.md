### Filter:

1. Cú pháp:
   #. filter: none | -> giá trị mặc định

#. blur() | -> độ mờ ảnh

#. brightness() | -> hiệu chỉnh sáng tối Điều chỉnh độ sáng của hình ảnh.
-> 0% sẽ làm cho hình ảnh hoàn toàn đen.
-> 100% (1) là mặc định và thể hiện ảnh gốc.
-> Giá trị trên 100% sẽ cho kết quả sáng hơn.

#. contrast() | -> Điều chỉnh độ tương phản của hình ảnh.
-> 0% sẽ làm cho hình ảnh hoàn toàn đen.
-> 100% (1) là mặc định và thể hiện hình ảnh gốc.
-> Giá trị trên 100% sẽ cho kết quả có độ tương phản cao hơn.

#. drop-shadow() | -> đổ bóng, tương tự box-shadow

#. grayscale() | -> Chuyển đổi hình ảnh sang thang độ xám.
-> 0% (0) là mặc định và thể hiện ảnh gốc.
-> 100% sẽ làm cho ảnh có màu xám hoàn toàn (dùng cho ảnh đen trắng).
Lưu ý: Không cho phép giá trị âm.

#. hue-rotate() | -> Áp dụng xoay màu sắc trên hình ảnh. Giá trị xác định số độ xung quanh vòng tròn màu mà mẫu hình ảnh sẽ được điều chỉnh. 0deg là mặc định và đại diện cho hình ảnh gốc.
Lưu ý: Giá trị tối đa là 360deg.

#. invert() | -> Đảo ngược các mẫu trong hình ảnh.
-> 0% (0) là mặc định và thể hiện ảnh gốc.
-> 100% sẽ khiến hình ảnh bị đảo ngược hoàn toàn.
Lưu ý: Không cho phép giá trị âm.

#. opacity() | -> Đặt mức độ mờ cho hình ảnh. Mức độ mờ mô tả mức độ trong suốt, trong đó:
-> 0% là hoàn toàn minh bạch.
-> 100% (1) là mặc định và thể hiện ảnh gốc (không có độ trong suốt).
Lưu ý: Không cho phép giá trị âm.

#. saturate() | -> Bão hòa hình ảnh.
-> 0% (0) sẽ làm cho hình ảnh không bão hòa hoàn toàn.
-> 100% là mặc định và đại diện cho hình ảnh gốc.
-> Giá trị trên 100% mang lại kết quả siêu bão hòa.
Lưu ý: Không cho phép giá trị âm.

#. sepia() | -> Chuyển đổi hình ảnh sang màu nâu đỏ.
-> 0% (0) là mặc định và thể hiện ảnh gốc.
-> 100% sẽ làm cho hình ảnh có màu nâu đỏ hoàn toàn.
Lưu ý: Không cho phép giá trị âm.

#. url(); -> Hàm url() lấy vị trí của tệp XML chỉ định bộ lọc SVG và có thể bao gồm một neo cho một thành phần bộ lọc cụ thể.
-> Ví dụ:
bộ lọc: url(svg-url#element-id)

2. Box-shadow và Drop-shadow:

## Box Shadow:

-> Cách dùng: Sử dụng để tạo bóng cho hộp bao quanh phần tử.
-> Tác dụng: Tạo ra bóng xung quanh toàn bộ khung của phần tử.
-> Cú pháp: box-shadow: h-offset v-offset blur spread color;
-> box-shadow tạo ra bóng xung quanh khung của phần tử
-> box-shadow chỉ áp dụng cho khung xung quanh.

## Drop Shadow:

-> Cách dùng: Sử dụng để tạo bóng đổ từ phần tử ra ngoài.
-> Tác dụng: Tạo ra bóng đổ mô phỏng cảm giác phần tử nổi lên và tách biệt khỏi nền.
-> Cú pháp: filter: drop-shadow(h-offset v-offset blur color);
-> drop-shadow tạo bóng đổ từ phần tử ra ngoài.
-> đổ bóng xung quanh phần tử
-> drop-shadow có thể yêu cầu xử lý nhiều hơn vì nó áp dụng bóng đổ cho toàn bộ phần tử, bao gồm cả nội dung trong suốt
