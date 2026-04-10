1. Tại sao phải dùng Nginx làm Reverse Proxy mà không trỏ thẳng Tunnel vào Node-RED?

   -> Em dùng Nginx làm reverse proxy để tách frontend và backend. Nginx xử lý web tĩnh nhanh hơn và có thể route /api sang Node-RED, đồng thời giúp không phải expose trực tiếp Node-RED ra ngoài nên an toàn hơn.

2. Sự khác biệt giữa việc Mount file và Mount thư mục trong Docker là gì?

   ->Mount file là gắn một file cụ thể vào container, còn mount thư mục là gắn cả thư mục. Thường mount thư mục để chứa web hoặc dữ liệu, còn mount file để cấu hình.

3. Nếu thay đổi file index.html ở máy Ubuntu, nội dung trên web có thay đổi ngay không? Tại sao?

   ->Có, vì đang mount trực tiếp thư mục từ máy host vào container nên khi sửa file thì Nginx đọc lại ngay, không cần restart.

4. docker-compose.yml khai báo các services có phần restart: always hoặc restart: unless-stopped : chúng để làm gì?

   ->Để container tự chạy lại khi bị lỗi hoặc khi server restart, giúp hệ thống luôn hoạt động liên tục.

5. Cách khai báo để tất cả các services đều dùng chung 1 network? lợi ích của việc khai báo này là gì? Sửa đổi file docker-compose để tất cả các service đều dùng chung 1 network.

   ->Để các container giao tiếp với nhau bằng tên service như nginx gọi nodered. Như vậy không cần nhớ IP và hệ thống dễ quản lý hơn.

6. Tìm cách đưa Cloudflare Token vào trong file .env rồi sau đó thêm .env vào file .gitignore trước khi push code lên github. Tại sao nói đây là điều quan trọng về bảo mật mã nguồn?

   ->Vì token là thông tin nhạy cảm. Nếu push lên GitHub mà không ignore thì người khác có thể dùng token đó truy cập vào tunnel, gây mất bảo mật.
  
7. Tại sao chúng ta nên thêm hậu tố :ro khi mount file cấu hình Nginx?

   ->Để container chỉ được đọc file cấu hình mà không sửa được, tránh lỗi và tăng bảo mật.

8. Khi dùng Cloudflare Tunnel: có cần thiết phải mở cổng cho các service nữa không?

   ->Không cần, vì tunnel tạo kết nối từ server ra Cloudflare nên không cần mở port hay public IP mà vẫn truy cập được từ Internet.
