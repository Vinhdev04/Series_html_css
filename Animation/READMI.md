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
