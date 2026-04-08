# Phát triển ứng dụng với mã nguồn mở--TEE0421
VU LAN_K225480106036_Phát triển ứng dụng với mã nguồn mở_bài tập 01

deadline : 23h59 ngày 13 tháng 4 năm 2026.

***A. Đăng ký tên miền xịn cho cá nhân:***

1.**Đăng ký domain xịn**
   
   <img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/61896ac4-df8d-4861-8b4a-8c3718dfd497" />

2.**Đăng ký tài khoản cloudflare**
   
   <img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/32ceb025-3334-4139-bd78-429ae7a446b5" />

3. **Thêm domain đã đăng ký vào trong cloudflare : Nhận 2 dòng namespace**

   <img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/a2e9adef-93d5-48cf-b384-7e96890c053c" />

5. **Nhập 2 dòng namespace của cloudflare vào trong trang quản lý DNS record của tên miền đăng ký**

   <img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/d0a7657d-5ff9-40a9-a80f-db6e76953d1f" />

=>> **Sau thời gian đợi khoảng 5-10 phút thì thu được kết quả:(Tên miền của bạn hiện đã được bảo vệ bởi Cloudflare)**
   
   <img width="1920" height="1075" alt="image" src="https://github.com/user-attachments/assets/37745c57-9509-4b81-b62b-f4113f28e2fe" />

***B. Cài đặt Ubuntu + Docker***

**Khởi tạo mới hyper-V**

<img width="1408" height="1004" alt="image" src="https://github.com/user-attachments/assets/5a748c3d-f391-42b6-9c43-5e7344ce7377" />

**Khởi động máy ảo**

<img width="1718" height="1071" alt="image" src="https://github.com/user-attachments/assets/52d7f4c4-5dd2-40cd-9140-c6b83707a2fd" />

**Khởi tạo máy ảo**

<img width="1908" height="1074" alt="image" src="https://github.com/user-attachments/assets/cd9af52d-4165-4754-9507-4e02af8b962e" />

1. Cài đặt hệ điều hành Ubuntu 24.04.4 LTS thành công 

Máy ảo đã boot OK
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/c8f73c1a-7136-498a-aa61-fe2b4fc14848" />

Đăng nhập:
<img width="1535" height="899" alt="image" src="https://github.com/user-attachments/assets/330ccdce-8d75-40b1-96d5-dbfff299b87a" />

Cấu hình mạng trong Ubuntu (và công cụ giả lập) để cho phép truy cập SSH vào Ubuntu từ cmd của windows.

<img width="1506" height="1075" alt="image" src="https://github.com/user-attachments/assets/cbea188d-a8bc-4ee2-b3c6-be75bb054bb0" />

SSH đã được cài & đang chạy, port 22 đang mở trong ubuntu
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/9f750115-bffb-4405-9c07-2357d2296a58" />

SSH thành công từ windows
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/8773694a-2a02-4e3c-af47-09abf31f53d5" />

Cài docker:
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/45d1a2d5-e2b8-436d-8205-88d615225081" />

Kiểm tra lại:
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/717e5606-7733-42f7-a18a-3a9316ab4d1e" />

Thêm user vào docker group
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/3ec9b1d3-92f9-4d80-8f88-5500b789619f" />
