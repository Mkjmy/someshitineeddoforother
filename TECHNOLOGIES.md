# Các Công Nghệ Chi Tiết Được Sử Dụng Trong Dự Án "Báo Tường Tết Nguyên Đán"

Tài liệu này cung cấp giải thích toàn diện về mọi thẻ HTML và thuộc tính CSS được sử dụng trong dự án "Báo Tường Tết Nguyên Đán", cùng với tóm tắt các kỹ thuật phát triển web chính được áp dụng.

## 1. Các Thẻ HTML5 và Cách Sử Dụng

HTML5 cung cấp cấu trúc và nội dung cho tất cả các trang web trong dự án này. Dưới đây là danh sách tất cả các thẻ HTML duy nhất được tìm thấy, với mô tả về mục đích chung và cách chúng được sử dụng cụ thể trong dự án này.

*   `<html>`: Phần tử gốc của một trang HTML.
    *   **Cách sử dụng:** Bao bọc tất cả nội dung của mọi tệp `.html`, khai báo tài liệu là HTML. Sử dụng `lang="vi"` cho ngôn ngữ tiếng Việt.
*   `<head>`: Chứa thông tin máy đọc được (metadata) về tài liệu, như tiêu đề, tập lệnh và biểu định kiểu của nó.
    *   **Cách sử dụng:** Có mặt trong tất cả các tệp `.html`. Nó bao gồm các thẻ `<meta>` cho cài đặt bộ ký tự và chế độ xem, `<title>` cho tiêu đề trang và `<link>` cho CSS bên ngoài hoặc `<style>` cho CSS nội bộ.
*   `<meta>`: Định nghĩa siêu dữ liệu về tài liệu HTML. Siêu dữ liệu là dữ liệu về dữ liệu.
    *   **Cách sử dụng:**
        *   `<meta charset="UTF-8">`: Chỉ định mã hóa ký tự cho tài liệu, đảm bảo hiển thị đúng các ký tự tiếng Việt.
        *   `<meta name="viewport" content="width=device-width, initial-scale=1.0">`: Cấu hình chế độ xem cho thiết kế đáp ứng, giúp trang web thích ứng với các kích thước màn hình khác nhau.
*   `<title>`: Định nghĩa tiêu đề của tài liệu hiển thị trên thanh tiêu đề hoặc tab của trình duyệt.
    *   **Cách sử dụng:** Mỗi tệp `.html` có một tiêu đề mô tả liên quan đến nội dung của nó (ví dụ: "Báo Tường Tết Nguyên Đán", "Bánh Chưng").
*   `<link>`: Chỉ định mối quan hệ giữa tài liệu hiện tại và một tài nguyên bên ngoài.
    *   **Cách sử dụng:** Chỉ trong `main.html`: `<link rel="stylesheet" href="style.css">` để liên kết một tệp CSS bên ngoài để tạo kiểu.
*   `<style>`: Được sử dụng để chứa thông tin kiểu CSS cho một tài liệu.
    *   **Cách sử dụng:** Trong `banh-chung.html`, `gui-loi-chuc.html`, `khong-khi-ngay-xuan.html` và `members.html`, thẻ này nhúng tất cả các quy tắc CSS trực tiếp vào trong tài liệu HTML.
*   `<body>`: Chứa tất cả nội dung của tài liệu HTML, chẳng hạn như tiêu đề, đoạn văn, hình ảnh, siêu liên kết, bảng, danh sách, v.v.
    *   **Cách sử dụng:** Bao gồm tất cả nội dung hiển thị của mọi tệp `.html`.
*   `<header>`: Đại diện cho nội dung giới thiệu, thường chứa một nhóm các trợ giúp giới thiệu hoặc điều hướng.
    *   **Cách sử dụng:** Được sử dụng trên tất cả các trang, thường ở trên cùng, chứa tiêu đề chính (`<h1>`) của trang.
*   `<h1>`: Đại diện cho tiêu đề quan trọng nhất trên trang.
    *   **Cách sử dụng:** Được sử dụng cho tiêu đề chính của mỗi trang (ví dụ: "TẾT NGUYÊN ĐÁN - NÉT VĂN HÓA VIỆT" trên `main.html`, "Bánh Chưng" trên `banh-chung.html`).
*   `<p>`: Đại diện cho một đoạn văn bản.
    *   **Cách sử dụng:** Được sử dụng cho nội dung văn bản chung, mô tả, tín dụng và chú thích trong suốt dự án.
*   `<nav>`: Đại diện cho một phần của trang cung cấp các liên kết điều hướng.
    *   **Cách sử dụng:** Trong `main.html`, nó chứa menu điều hướng chính (`#menu`) liên kết đến các phần và trang khác nhau.
*   `<ul>`: Đại diện cho một danh sách không có thứ tự các mục.
    *   **Cách sử dụng:** Trong `main.html` bên trong `<nav>` để tạo các mục menu.
*   `<li>`: Đại diện cho một mục danh sách.
    *   **Cách sử dụng:** Được sử dụng cho các mục riêng lẻ trong danh sách điều hướng `<ul>` trong `main.html`.
*   `<a>`: Đại diện cho một siêu liên kết, liên kết đến các trang web, tệp hoặc vị trí khác trong cùng một trang.
    *   **Cách sử dụng:** Được sử dụng cho các liên kết điều hướng trong menu, các nút "Quay lại trang chính" và các liên kết xung quanh các thẻ bài viết.
*   `<main>`: Đại diện cho nội dung thống trị của `<body>`.
    *   **Cách sử dụng:** Bao gồm khu vực nội dung chính của tất cả các tệp `.html` (ví dụ: `#content` trong `main.html`, `.container` trong `members.html`).
*   `<section>`: Đại diện cho một phần độc lập về chức năng có trong tài liệu HTML.
    *   **Cách sử dụng:** Được sử dụng để nhóm nội dung liên quan (ví dụ: các phần `#gioi-thieu`, `#am-nhac`, `#bai-viet`, `#binh-luan` trên `main.html`).
*   `<h2>`: Đại diện cho tiêu đề cấp hai, ít quan trọng hơn `<h1>` nhưng quan trọng hơn `<h3>`.
    *   **Cách sử dụng:** Được sử dụng cho các tiêu đề phụ hoặc tiêu đề phần trong các khu vực nội dung `main` (ví dụ: "Lời Ngỏ: Ý Nghĩa Tết Cổ Truyền").
*   `<video>`: Được sử dụng để nhúng nội dung video.
    *   **Cách sử dụng:** Trong `main.html`, `<video class="tet_video" controls>` nhúng `video/am_thuc.mp4`. Thuộc tính `controls` cung cấp các điều khiển video mặc định.
*   `<source>`: Chỉ định nhiều tài nguyên phương tiện cho các phần tử `<picture>`, `<audio>` hoặc `<video>`.
    *   **Cách sử dụng:** Bên trong các thẻ `<video>` và `<audio>` để chỉ định tệp phương tiện và loại của nó (ví dụ: `<source src="video/am_thuc.mp4" type="video/mp4">`).
*   `<div>`: Một vùng chứa chung cho nội dung luồng. Nó không ảnh hưởng đến nội dung hoặc bố cục cho đến khi được tạo kiểu trong CSS.
    *   **Cách sử dụng:** Được sử dụng làm vùng chứa đa năng để nhóm các phần tử (ví dụ: `.audio-container`, `.card-container`, `.card-text-content`, `.gallery`, `.img-container`). *Lưu ý: Mặc dù phổ biến, các phương pháp hay nhất hiện nay thường đề xuất sử dụng các phần tử HTML5 có ý nghĩa hơn nếu `div` phục vụ mục đích cấu trúc hơn là mục đích trình bày thuần túy.*
*   `<audio>`: Được sử dụng để nhúng nội dung âm thanh.
    *   **Cách sử dụng:** Trong `main.html`, `<audio controls class="tet_audio">` nhúng `audio/nhac.m4a`. Thuộc tính `controls` cung cấp các điều khiển âm thanh mặc định.
*   `<strong>`: Cho biết nội dung của nó có tầm quan trọng, nghiêm trọng hoặc khẩn cấp.
    *   **Cách sử dụng:** Được sử dụng để nhấn mạnh, ví dụ: trong phần tín dụng trong `<footer>` hoặc trong văn bản đoạn văn.
*   `<article>`: Đại diện cho một bố cục độc lập trong tài liệu, trang, ứng dụng hoặc trang web, có ý định được phân phối hoặc tái sử dụng độc lập.
    *   **Cách sử dụng:** Được sử dụng cho các "mục bài đăng" hoặc bài viết riêng lẻ trong các phần, chẳng hạn như những phần liên kết đến `banh-chung.html` trên `main.html`.
*   `<img>`: Nhúng một hình ảnh vào tài liệu.
    *   **Cách sử dụng:** Được sử dụng để hiển thị nhiều hình ảnh khác nhau, bao gồm hình thu nhỏ (`pic/bangtrung.jpg`, `pic/chotet.jpg`) và hình ảnh cụ thể theo nội dung (ví dụ: hình ảnh Bánh Chưng trên `banh-chung.html`). Bao gồm các thuộc tính `alt` cho khả năng tiếp cận.
*   `<h3>`: Đại diện cho tiêu đề cấp ba.
    *   **Cách sử dụng:** Được sử dụng cho các tiêu đề phụ trong các bài viết hoặc thẻ (ví dụ: "Bánh Chưng - Bánh Giầy", "Hoa Đào Rực Rỡ").
*   `<span>`: Một vùng chứa nội tuyến chung cho nội dung từ ngữ, không có ý nghĩa gì vốn có.
    *   **Cách sử dụng:** Được sử dụng để tạo kiểu cho một phần cụ thể của văn bản, chẳng hạn như liệt kê tên tác giả với `class="tac-gia"`.
*   `<footer>`: Đại diện cho một chân trang cho nội dung phân đoạn gần nhất hoặc phần tử gốc phân đoạn của nó.
    *   **Cách sử dụng:** Được sử dụng ở cuối `main.html` để chứa bản quyền, tín dụng và thông tin liên hệ.
*   `<form>`: Đại diện cho một phần tài liệu chứa các điều khiển tương tác để gửi thông tin.
    *   **Cách sử dụng:** Trong `gui-loi-chuc.html`, nó bao bọc các trường nhập liệu để gửi bình luận/lời chúc.
*   `<label>`: Đại diện cho một chú thích cho một mục trong giao diện người dùng.
    *   **Cách sử dụng:** Được sử dụng với các phần tử `<input>` và `<textarea>` trong `gui-loi-chuc.html` để liên kết văn bản mô tả với các điều khiển biểu mẫu, cải thiện khả năng tiếp cận.
*   `<input>`: Được sử dụng để tạo các điều khiển tương tác cho các biểu mẫu dựa trên web nhằm chấp nhận dữ liệu từ người dùng.
    *   **Cách sử dụng:** Trong `gui-loi-chuc.html` để nhập văn bản (`type="text"`) và nhập email (`type="email"`).
*   `<textarea>`: Đại diện cho một điều khiển chỉnh sửa văn bản thuần túy nhiều dòng.
    *   **Cách sử dụng:** Trong `gui-loi-chuc.html` cho trường "Lời chúc".
*   `<button>`: Đại diện cho một nút có thể nhấp.
    *   **Cách sử dụng:** Trong `gui-loi-chuc.html` để gửi "Gửi Bình Luận".
*   `<table>`: Đại diện cho dữ liệu dạng bảng.
    *   **Cách sử dụng:** Trong `members.html` để cấu trúc danh sách thành viên nhóm.
*   `<thead>`: Định nghĩa một tập hợp các hàng xác định tiêu đề của các cột của bảng.
    *   **Cách sử dụng:** Trong `members.html` cho tiêu đề bảng, chứa tiêu đề cột.
*   `<tr>`: Định nghĩa một hàng các ô trong một bảng.
    *   **Cách sử dụng:** Được sử dụng cho mỗi hàng trong bảng, cả cho tiêu đề và dữ liệu.
*   `<th>`: Định nghĩa một ô tiêu đề trong một bảng.
    *   **Cách sử dụng:** Trong `members.html` cho các tiêu đề cột bảng ("Họ và Tên", "STT").
*   `<tbody>`: Nhóm nội dung chính của bảng.
    *   **Cách sử dụng:** Trong `members.html` để chứa các hàng dữ liệu chính của bảng.
*   `<td>`: Định nghĩa một ô dữ liệu tiêu chuẩn trong một bảng.
    *   **Cách sử dụng:** Trong `members.html` cho các mục dữ liệu riêng lẻ trong các hàng bảng.

## 2. Các Thuộc Tính CSS và Cách Sử Dụng

Các thuộc tính CSS kiểm soát kiểu dáng và bố cục của các phần tử HTML. Dưới đây là danh sách tất cả các thuộc tính CSS duy nhất được tìm thấy trong `style.css` (và do đó được nhúng vào các tệp HTML khác), với giải thích về chức năng của chúng.

*   `font-family`: Chỉ định phông chữ cho một phần tử.
    *   **Cách sử dụng:** `Arial, sans-serif` được đặt cho `body` để cung cấp một kiểu chữ nhất quán, dễ đọc trên toàn bộ trang web.
*   `margin`: Đặt lề cho một phần tử, tạo khoảng trống xung quanh nó.
    *   **Cách sử dụng:** Được sử dụng rộng rãi để tạo khoảng cách cho các phần tử (ví dụ: `margin: 0` để đặt lại lề mặc định của trình duyệt, `margin: 0 auto` để căn giữa theo chiều ngang, `margin-top`, `margin-bottom` để tạo khoảng cách theo chiều dọc).
*   `background-image`: Đặt một hoặc nhiều hình ảnh nền cho một phần tử.
    *   **Cách sử dụng:** `url("Hinh-nen-tet-2025-cho-may-tinh-10")` được sử dụng trên `body` để đặt một hình nền lễ hội cho toàn bộ trang.
*   `background-size`: Chỉ định kích thước của hình ảnh nền.
    *   **Cách sử dụng:** `cover` được sử dụng trên `body` để đảm bảo hình ảnh nền luôn bao phủ toàn bộ phần tử, ngay cả khi nó phải cắt một chút.
*   `background-repeat`: Đặt xem hình ảnh nền có lặp lại hay không.
    *   **Cách sử dụng:** `no-repeat` trên `body` ngăn hình ảnh nền lặp lại.
*   `background-attachment`: Đặt xem hình ảnh nền có cuộn cùng với khối chứa của nó hay được cố định.
    *   **Cách sử dụng:** `fixed` trên `body` giữ hình ảnh nền ở vị trí cố định so với chế độ xem.
*   `background-position`: Đặt vị trí ban đầu cho mỗi hình ảnh nền.
    *   **Cách sử dụng:** `center` trên `body` căn giữa hình ảnh nền theo chiều ngang và chiều dọc.
*   `display`: Chỉ định loại hộp hiển thị mà một phần tử tạo ra.
    *   **Cách sử dụng:** Được sử dụng để kiểm soát bố cục (ví dụ: `block` cho các phần tử toàn chiều rộng, `inline-block` cho các phần tử nằm cạnh nhau nhưng vẫn giữ các thuộc tính khối, `flex` cho các vùng chứa flexbox, `grid` cho các vùng chứa grid, `none` trong các truy vấn phương tiện để ẩn các phần tử).
*   `height`: Đặt chiều cao của một phần tử.
    *   **Cách sử dụng:** Được sử dụng cho các chiều cao phần tử cụ thể (ví dụ: `500px` cho `.tet_video`, `150px` cho hình thu nhỏ).
*   `width`: Đặt chiều rộng của một phần tử.
    *   **Cách sử dụng:** Được sử dụng cho nhiều phần tử khác nhau, thường là với phần trăm (`100%`) hoặc giá trị cố định (`300px`).
*   `max-width`: Đặt chiều rộng tối đa của một phần tử.
    *   **Cách sử dụng:** Được sử dụng để giới hạn chiều rộng của các phần tử, đảm bảo chúng không quá rộng trên các màn hình lớn (ví dụ: `800px` cho `.tet_video`, `.audio-container`, `.container`).
*   `background-color`: Đặt màu nền của một phần tử.
    *   **Cách sử dụng:** Được sử dụng cho tiêu đề (`#header`, `#menu`), chân trang (`#footer`), nền nội dung (`#content`) và các phần tử tương tác (nút, thẻ). Ví dụ bao gồm `red`, `yellow`, `#003366`, `#f9f9f9`, `white`, `#555`, `#f2f2f2`, `#6c757d`.
*   `border`: Thuộc tính viết tắt để đặt tất cả các thuộc tính đường viền trong một khai báo.
    *   **Cách sử dụng:** Được sử dụng để định nghĩa đường viền xung quanh các phần tử như `.audio-container`, `.post`, `.comment-form`, `.section-link-card`, `.members-table`, `img`.
*   `border-radius`: Đặt bán kính của các góc của phần tử.
    *   **Cách sử dụng:** Được sử dụng để tạo các góc tròn cho các vùng chứa (`.audio-container`, `.section-link-card`, `.container`, `#footer`, `img`).
*   `padding`: Đặt vùng đệm ở cả bốn phía của một phần tử.
    *   **Cách sử dụng:** Được sử dụng để tạo khoảng cách giữa nội dung của phần tử và đường viền của nó (ví dụ: `padding: 20px` cho các vùng chứa khác nhau, `padding: 10px` cho các mục danh sách, ô bảng, trường nhập liệu).
*   `margin-top`: Đặt vùng lề ở phía trên của một phần tử.
    *   **Cách sử dụng:** Được sử dụng để tạo khoảng cách theo chiều dọc giữa các phần tử.
*   `box-shadow`: Gắn một hoặc nhiều bóng đổ vào phần tử.
    *   **Cách sử dụng:** Được sử dụng để tạo độ sâu trực quan trên `.audio-container`, `.section-link-card`, `.container`.
*   `margin-left`: Đặt vùng lề ở phía bên trái của một phần tử.
    *   **Cách sử dụng:** Được sử dụng để tạo khoảng cách theo chiều ngang hoặc căn giữa (`auto`).
*   `margin-right`: Đặt vùng lề ở phía bên phải của một phần tử.
    *   **Cách sử dụng:** Được sử dụng để tạo khoảng cách theo chiều ngang hoặc căn giữa (`auto`).
*   `font-weight`: Đặt độ đậm (hoặc độ dày) của các ký tự trong văn bản.
    *   **Cách sử dụng:** `bold` để nhấn mạnh (ví dụ: các thẻ `strong`, `.audio-container p`, `.details-text`).
*   `color`: Đặt giá trị màu tiền cảnh của nội dung văn bản của một phần tử.
    *   **Cách sử dụng:** Được sử dụng cho màu văn bản trên nhiều phần tử khác nhau (ví dụ: `yellow`, `white`, `#003366`, `gray`, `#333`, `#0056b3`, `#555`).
*   `text-align`: Đặt căn chỉnh ngang của nội dung nội tuyến của một phần tử khối.
    *   **Cách sử dụng:** Được sử dụng để căn giữa văn bản (`center`) hoặc căn chỉnh nó (`left`, `right`) trong các phần tử như tiêu đề, menu và các phần nội dung.
*   `list-style`: Thuộc tính viết tắt để đặt tất cả các thuộc tính kiểu danh sách trong một khai báo.
    *   **Cách sử dụng:** `none` trên các phần tử `ul` (ví dụ: `#menu ul`, `.main-nav-list`) để loại bỏ các dấu đầu dòng mặc định.
*   `text-decoration`: Đặt giao diện của các đường trang trí trên văn bản.
    *   **Cách sử dụng:** `none` trên các liên kết (`a`) để loại bỏ gạch chân mặc định.
*   `border-bottom`: Thuộc tính viết tắt để đặt `border-bottom-width`, `border-bottom-style` và `border-bottom-color`.
    *   **Cách sử dụng:** Được sử dụng để tạo một đường kẻ bên dưới tiêu đề (ví dụ: `.post-title`).
*   `padding-bottom`: Đặt chiều cao của vùng đệm ở phía dưới của một phần tử.
    *   **Cách sử dụng:** Được sử dụng để tạo khoảng cách bên dưới tiêu đề.
*   `font-size`: Đặt kích thước của phông chữ.
    *   **Cách sử dụng:** Được sử dụng để định nghĩa kích thước văn bản cho các phần tử khác nhau (ví dụ: `24px` cho `.post-title`, `18px` cho `.button-link`).
*   `grid-template-columns`: Định nghĩa tên dòng và các hàm định cỡ track của các cột lưới.
    *   **Cách sử dụng:** `repeat(auto-fit, minmax(250px, 1fr))` cho `.animal-grid` để tạo bố cục cột đáp ứng, linh hoạt.
*   `gap`: Đặt khoảng cách (rãnh) giữa các hàng và cột.
    *   **Cách sử dụng:** `20px` cho `.animal-grid` và `.card-container` để tạo khoảng cách giữa các mục lưới/flex.
*   `flex-direction`: Thiết lập trục chính, do đó định nghĩa hướng các mục flex được đặt trong vùng chứa flex.
    *   **Cách sử dụng:** `column` cho `.section-link-card` để xếp chồng hình ảnh và nội dung văn bản theo chiều dọc.
*   `align-items`: Đặt giá trị `align-self` trên tất cả các phần tử con trực tiếp dưới dạng một nhóm. Trong Flexbox, nó kiểm soát căn chỉnh dọc theo trục chéo.
    *   **Cách sử dụng:** `center` cho `.section-link-card` để căn giữa các mục theo chiều ngang trong vùng chứa flex.
*   `flex-wrap`: Kiểm soát xem các mục flex có bị buộc trên một dòng hay có thể xuống nhiều dòng.
    *   **Cách sử dụng:** `wrap` cho `.card-container` để cho phép các thẻ xuống dòng trên màn hình nhỏ hơn.
*   `transition`: Một thuộc tính viết tắt cho `transition-property`, `transition-duration`, `transition-timing-function`, và `transition-delay`.
    *   **Cách sử dụng:** `box-shadow 0.3s ease, transform 0.3s ease` cho `.section-link-card` để tạo hiệu ứng hình ảnh mượt mà khi di chuột.
*   `object-fit`: Chỉ định cách nội dung của một phần tử được thay thế, chẳng hạn như `<img>` hoặc `<video>`, nên được thay đổi kích thước để phù hợp với vùng chứa của nó.
    *   **Cách sử dụng:** `cover` cho `.section-link-card img` để đảm bảo hình ảnh bao phủ không gian được phân bổ mà không bị biến dạng.
*   `flex`: Thuộc tính viết tắt cho `flex-grow`, `flex-shrink`, và `flex-basis`.
    *   **Cách sử dụng:** `1` cho `.section-link-card .card-text-content` để cho phép nội dung văn bản phát triển và thu nhỏ, chiếm không gian có sẵn.
*   `content`: Thay thế hoặc thêm nội dung trước hoặc sau nội dung của một phần tử.
    *   **Cách sử dụng:** `attr(data-label)` trong các truy vấn phương tiện cho `.members-table td::before` để hiển thị tiêu đề cột trên thiết bị di động.
*   `position`: Chỉ định loại phương pháp định vị được sử dụng cho một phần tử.
    *   **Cách sử dụng:** `relative` cho `.members-table td` và `absolute` cho `.members-table td::before` để định vị `data-label` chính xác trong các bảng đáp ứng.
*   `left`: Chỉ định vị trí bên trái của một phần tử được định vị.
    *   **Cách sử dụng:** `10px` cho `.members-table td::before` để bù đắp `data-label` từ cạnh trái.
*   `white-space`: Đặt cách xử lý khoảng trắng bên trong một phần tử.
    *   **Cách sử dụng:** `nowrap` cho `.members-table td::before` để ngăn `data-label` xuống dòng.

## 3. Các Kỹ Thuật Phát Triển Web Chính Được Áp Dụng

Ngoài các thẻ và thuộc tính riêng lẻ, dự án còn thể hiện một số kỹ thuật phát triển web cơ bản:

*   **Cấu trúc HTML5 có ý nghĩa:** Việc sử dụng các phần tử như `<header>`, `<nav>`, `<main>`, `<section>`, `<article>`, và `<footer>` tạo ra một dàn ý tài liệu hợp lý và có ý nghĩa, mang lại lợi ích cho khả năng tiếp cận và SEO.
*   **CSS để trình bày:** Tạo kiểu chủ yếu được xử lý bởi CSS, tách nội dung khỏi trình bày. Điều này giúp mã dễ bảo trì và sửa đổi hơn.
*   **Thiết kế đáp ứng (Responsive Design):** Dự án kết hợp các nguyên tắc thiết kế đáp ứng bằng cách sử dụng:
    *   **Thẻ Meta Viewport:** Đảm bảo tỷ lệ phù hợp trên các thiết bị.
    *   **Đơn vị tương đối:** Sử dụng `width: 100%`, `max-width`, và bố cục `flexbox` / `grid` thích ứng với không gian màn hình có sẵn.
    *   **Truy vấn phương tiện (Media Queries):** Cụ thể, quy tắc `@media (max-width: 768px)` được sử dụng để điều chỉnh bố cục của bảng thành viên để dễ sử dụng hơn trên màn hình nhỏ.
*   **Nhúng đa phương tiện:** Nhúng trực tiếp âm thanh và video bằng các thẻ `<audio>` và `<video>` HTML5, cung cấp nội dung phong phú mà không cần dựa vào các plugin của bên thứ ba.
*   **Tạo biểu mẫu:** Các biểu mẫu HTML cơ bản được sử dụng để thu thập thông tin đầu vào của người dùng, thể hiện tương tác phía máy khách đơn giản.
*   **Chiến lược CSS bên ngoài so với CSS nội bộ:** Dự án thể hiện hai cách phổ biến để áp dụng CSS: một biểu định kiểu bên ngoài cho trang trung tâm (`main.html`) và các biểu định kiểu nội bộ cho các trang khác. Điều này minh họa tính linh hoạt trong quản lý CSS, mặc dù đối với các dự án lớn hơn, phương pháp tiếp cận hoàn toàn bên ngoài thường được ưu tiên.
*   **Cải tiến trực quan:** Việc sử dụng các thuộc tính `box-shadow`, `border-radius`, và `transition` bổ sung thêm vẻ hiện đại và tương tác tinh tế cho các phần tử khác nhau.
*   **Điều hướng:** Điều hướng rõ ràng được cung cấp cả thông qua menu chính và các nút "quay lại trang chủ" trên các trang con, đảm bảo luồng người dùng dễ dàng.

Giải thích chi tiết này sẽ cung cấp sự hiểu biết toàn diện về các công nghệ và kỹ thuật làm nền tảng cho dự án "Báo Tường Tết Nguyên Đán".