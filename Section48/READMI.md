### Image srcset attribute:

## Trang web sử dụng ít hình ảnh (Tốc độ tải trang không bị ảnh hưởng nhiều bởi hình ảnh)

    - Tối ưu sử dụng hình ảnh trên trang web:
    -
        1. Sử dụng đúng định dạng ảnh phù hợp:
            + Hình học, vector,... -> SVG
            + Bitmap transparent   -> PNG,WEBP
            + Bitmap no transparent -> JPEG, WEBP
            => WEBP -> hỗ trợ ít trình duyệt nhưng nó tối ưu hơn PNG,JPEG...

        2. Nén hình ảnh (giảm dung lượng ảnh):
            + "https://tinypng.com/" -> dùng thủ công
            + BackEnd -> code

        3. Sử dụng kích thước ảnh tương ứng:
            + Original: 4000px x 4000px, Figma: 800px x 800px (css), Resize: 1600px x 1600px (2x) -> đáp ứng tốt cho cả màn hình PPI/DPI(retina):
            + PPI -> Pixel per inch
            + DPI -> Dots per inch : 100 DPI, 300 DPI (mật độ điểm ảnh).

    - Loại màn hình:
        1. Màn hình thường: (DPI thấp 1:1): 800px x 800px ✅, 1600px x 1600px ❌(có thể chấp nhận được đối với trang web ít hình ảnh)
        2. Màn hình retina(DPI cao 2:1): 800px x 800px ❌, 1600px x 1600px ✅ (2x)

=> Link ảnh DPI: "https://tse1.mm.bing.net/th?id=OIP.Ik2nPcz1O3-TfrVCQA2lVQHaCg&pid=Api&P=0&h=180"

## Trang web sử dụng nhiều hình ảnh:

    => Sử dụng đúng định dạng ảnh phù hợp -> ✅
    => Nén hình ảnh (giảm dung lượng ảnh) -> ✅
    => Sử dụng kích thước ảnh tương ứng   -> ❌

    - Thiết bị:
      + Mobile: 1600px x 1600px ❌ => Tốn băng thông , load lâu => giảm trải nghiệm người dùng
      + Tablet: 1600px x 1600px ❌
      + Desktop: 1600px x 1600px ✅(2x)

    -> "Resolution switching: Different sizes"
    ## Bài toán 1:
    1. Mobile: 50px x 50px
    2. Tablet: 100px x 100px
    3. Desktop: 200px x 200px

    <!-- Resolution switching: Same size, different resolution-->
    ## Bài toán 2:
    Desktop: 200px x 200px

    <!-- Resolution switching: Art Direction -->
    ## Bài toán 3:
    Desktop: /img/anh-1.jpg
    Mobile: /img/anh-2.jpg

     => Luư ý: Js ko tối ưu tuyệt đôí bằng
