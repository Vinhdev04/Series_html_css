### Animation

// ---------------------------------- //

## Transition:

-> Làm châm quá trình biến đổi -> mượt

1. Transition:
   -> Syntax:
   transition: property timing-function duration delay

   -> property: mặc định all

   -> timing-function: Xác định cách thay đổi xảy ra theo thời gian. (ease, linear, ease-in, ease-out, ease-in-out)

   -> duration: transition từ trạng thái A -> B => bắt buộc phải có

   -> delay: Xác định thời gian trê trước khi transition bắt đầu

   ==> Shorthand:
   transition: property timing function duration delay
   transition: property duration delay timing function
   ...

## Lưu ý:

- Đối với cú pháp shorthand thì các giá trị " property" và "timing function" có thể linh hoạt vị trí
- Đối với "duration" luôn đứng trước "delay"
- Transition không được hỗ trợ trên nhiều thuộc tính : display: none,.....
- Ko nên tác động transition vào hover và active
- Hạn chế dùng thuộc tính transition: all cho dự án lớn, ko tối ưu web

// ---------------------------------- //

## Transform:

2.Transform:
-> Cho phép thay đổi hình dạng, kích thước , vị trí phần tử trên trang web

-> Transform: + rotate(), rotateX(), rotateY() -> xoay góc phần tử

               + scale(), scaleX(), scaleY() -> thay đổi tỉ lệ nhìn (zoom,..)

               + skew(), skewX(), skewY()  -> xoay nghiêng phần tử

               + translate(), translateX(), translateY() -> dùng để di chuyển phần tử
               + matrix(scaleX(), skewY(), skewX(), scaleY(), translateX(), translateY()) -> phương pháp kết hợp tất cả các phương pháp biến đổi 2D thành một.

## Lưu ý:

- Có thể kết hợp nhiều thuộc tính thông qua cú pháp shorthand
- Transform ko thể đẩy phần tử xung quanh ra xa
- Nên dùng tiền tố prefix cho 1 số trình duyệt cũ

// ---------------------------------- //

## Animation:

1. Animation:
   -> Tạo ra các chuyển động mà ko cần tác động vào phần tử

2.CSS Keyframes:
-> Cách tạo các bước cụ thể cảu animation, từ điểm xuất phát đến điểm kết thúc

3. Transition:
   -> Tạo ra các chuyển động khi tác động vào phần tử: hover,active,...

## Animation:

1. Cáu trúc:
   ==> Shorthand:
   -> animation: name duration timing-function delay iteration-count direction fill-mode

- Name: tên của keyframes

- Duration: thời gian áp dụng animation

- Timing-function: kiểu animation: linear, ease-in, ease-out, ease-out-in,....

  - ease -> mặc định có khởi đầu chậm, sau đó nhanh, rồi kết thúc chậm
  - ease-in -> có khởi đầu chậm
  - ease-out -> có kết thúc chậm
  - ease-in-out -> bắt đầu và kết thúc chậm
  - linear -> cùng tốc độ từ đầu đến cuối

- Delay: Thời gian chờ trước khi chạy animation

- Iteration-count: Số lần thực hiện

- Direction: hướng chạy của animation:

  - normal -> mặc định
  - reverse -> chạy ngược lại
  - alternate -> chạy bình thường sau đó chạy ngược lại
  - alternate reverse -> chạy ngược lại sau đó chạy bình thường

- Fill-mode: xác định vị trí cảu phần tử sau khi kết thúc animations
  - none -> mặc định
  - forward -> giá trị cuối cùng của keyframe animations
  - backword -> ngay khi bắt đầu animation ở vị trí keyframe đầu tiên
  - both -> bắt đầu tại keyframe đầu và kết thúc tại keyframe cuối

### Thư viện AOS:

-> Link: https://github.com/michalsnik/aos

  <!-- <link rel="stylesheet" href="https://unpkg.com/aos@next/dist/aos.css" /> -->

-> Thêm vào trước thẻ đóng body:

 <!-- <script src="https://unpkg.com/aos@next/dist/aos.js"></script>
  <script>
    AOS.init();
  </script> -->

=> dùng js tác động vào transition là chính,

### Thư viện Animate.css:

-> Link: https://animate.style/

 <!-- <link
    rel="stylesheet"
    href="https://cdnjs.cloudflare.com/ajax/libs/animate.css/4.1.1/animate.min.css"
  /> -->

=> animation nhưng ko linh hoạt

### Kết hợp thư viện AOS và Animate.css :
