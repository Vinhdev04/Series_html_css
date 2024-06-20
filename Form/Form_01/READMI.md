### HTML FORM:

# Cấu trúc:

->

  <!-- <form action="">
    <label>
      <input>
    </label>
  </form> -->

## Thuộc tính:

- id: -> trong cùng 1 trang id là duy nhất
- name: -> xác định tên của trường dữ liệu biểu bẫu khi gửi tới máy chủ
- value: -> xác định giá trị của trường dữ liệu khi gửi tới máy chủ
- placeholder: -> hiển thị văn bản gợi í cho người dùng
- required: -> trường dữ liệu bắt buộc phải nhập trước khi gửi biểu mẫu
- default: -> mặc định
- autocomplete = "off" -> đề xuất hoặc lưu trữ các giá trị đã nhập trước đó

## Input type:

- button
- checkbox
- radio
- color
- date
- datetime-local
- email
- file
- hidden
- image
- month
- number
- password
- range
- reset
- search
- submit
- tel
- text
- time
- url()
- week
- ......

## Thuộc tính action của form:

-> trong form khi người dùng nhấn submit thì dữ liệu trên form sẻ được gửi đi
-> dữ liệu sẻ gửi đến url() được khai báo trong thuộc tính action
-> phía backend sau khi nhận dữ liệu sẻ xử lý dữ liệu này.
