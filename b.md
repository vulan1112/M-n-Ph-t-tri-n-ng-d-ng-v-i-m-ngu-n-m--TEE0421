# b.md
VU LAN_K225480106036_mã nguồn mở_B1

***B. Cài đặt Ubuntu + Docker***

**Khởi tạo mới hyper-V**

<img width="1408" height="1004" alt="image" src="https://github.com/user-attachments/assets/5a748c3d-f391-42b6-9c43-5e7344ce7377" />

**Khởi động máy ảo**

<img width="1718" height="1071" alt="image" src="https://github.com/user-attachments/assets/52d7f4c4-5dd2-40cd-9140-c6b83707a2fd" />

**Khởi tạo máy ảo**

<img width="1908" height="1074" alt="image" src="https://github.com/user-attachments/assets/cd9af52d-4165-4754-9507-4e02af8b962e" />

**1.Cài đặt hệ điều hành Ubuntu 24.04.4 LTS thành công** 

Máy ảo đã boot OK

<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/c8f73c1a-7136-498a-aa61-fe2b4fc14848" />

**2.Tìm hiểu các lệnh cơ bản của ubuntu**

Đăng nhập:

<img width="1535" height="899" alt="image" src="https://github.com/user-attachments/assets/330ccdce-8d75-40b1-96d5-dbfff299b87a" />

Cấu hình mạng trong Ubuntu (và công cụ giả lập) để cho phép truy cập SSH vào Ubuntu từ cmd của windows.

<img width="1506" height="1075" alt="image" src="https://github.com/user-attachments/assets/cbea188d-a8bc-4ee2-b3c6-be75bb054bb0" />

SSH đã được cài & đang chạy, port 22 đang mở trong ubuntu

<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/9f750115-bffb-4405-9c07-2357d2296a58" />

SSH thành công từ windows

<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/8773694a-2a02-4e3c-af47-09abf31f53d5" />

**3.Cài docker cho Ubuntu:**

<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/45d1a2d5-e2b8-436d-8205-88d615225081" />

**4.Kiểm tra phiên bản docker vừa cài đặt, kiểm tra phiên bản của docker compose**

<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/717e5606-7733-42f7-a18a-3a9316ab4d1e" />

Thêm user vào docker group

<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/3ec9b1d3-92f9-4d80-8f88-5500b789619f" />

**5.Cấu hình để docker chạy mà không cần tiền tố sudo**

<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/10d4df87-7404-44b4-8359-c115a82cf760" />

**6.Tìm hiểu tập lệnh của docker và docker compose**
 
 Đã thực hành trong quá trình làm bài
 
**7.Đảm bảo tường lửa trên Ubuntu đã cho phép các cổng 80, 1880, 9630 (Lệnh: sudo ufw allow ...)**

<img width="1920" height="1079" alt="image" src="https://github.com/user-attachments/assets/12d1b108-3b3c-4d6a-936d-8805980fc501" />

Vượt tường lửa truy cập trình duyệt qua host cho phép trên Ubuntu

<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/74bedb28-08f5-4297-9e44-16e5adefa826" />
