### Phần 1: Phân tích lỗi sai của từng tên file

1\. File Poster Phim Hài.jpg

* Lỗi tiếng Việt có dấu (Hài): Dễ gây lỗi mã hóa ký tự (UTF-8/ASCII) khi lưu trữ hoặc tải lên server Linux.  
* Lỗi khoảng trắng: Làm đứt gãy đường dẫn URL hoặc bắt buộc phải dùng ký tự mã hóa %20.  
* Lỗi tên mơ hồ: Đặt tên quá chung chung, không xác định rõ đây là poster của bộ phim cụ thể nào.

2\. File Avengers\_end\_game\_final\_2.PNG

* Lỗi không nhất quán kiểu chữ: Trộn lẫn chữ viết hoa (Avengers) và chữ viết thường (end\_game\_final\_2).  
* Lỗi đuôi mở rộng viết hoa (.PNG): Hệ điều hành phân biệt hoa/thường như Linux sẽ báo lỗi 404 Not Found nếu gọi file bằng .png.  
* Lỗi dư thừa hậu tố: Việc đính kèm final\_2 thể hiện quản lý phiên bản thủ công, gây rác hệ thống tài nguyên.

3\. File LậtMặt6-Bảnchuẩn.jpeg

* Lỗi tiếng Việt có dấu (LậtMặt6-Bảnchuẩn): Gây xung đột định dạng trên hệ thống.  
* Lỗi pha trộn kiểu đặt tên: Dùng CamelCase (LậtMặt) kết hợp dấu gạch ngang (\-) không thống nhất.  
* Lỗi định dạng đuôi file: Sử dụng .jpeg thay vì chuẩn hóa về .jpg cho toàn bộ tài nguyên ảnh tĩnh.

4\. File icon tài khoản.SVG

* Lỗi tiếng Việt có dấu và khoảng trắng (tài khoản): Gây lỗi đường dẫn CLI và Web.  
* Lỗi đuôi mở rộng viết hoa (.SVG): Vi phạm quy tắc viết thường toàn bộ đuôi tệp tin (.svg).

### Phần 2: Chuẩn hóa tên file (Áp dụng chuẩn kebab-case)

Toàn bộ tên file được chuyển sang dạng kebab-case (viết thường toàn bộ, không dấu, phân cách bằng dấu gạch ngang \-, đuôi file viết thường):

* File 1: Poster Phim Hài.jpg $\rightarrow$ comedy-movie-poster.jpg *(hoặc đặt theo tên phim cụ thể: hai-tet-poster.jpg)*  
* File 2: Avengers\_end\_game\_final\_2.PNG $\rightarrow$ avengers-endgame-poster.png  
* File 3: LậtMặt6-Bảnchuẩn.jpeg $\rightarrow$ lat-mat-6-poster.jpg  
* File 4: icon tài khoản.SVG $\rightarrow$ user-account-icon.svg

