# C.md
VU LAN_K225480106036_phát triển ứng dụng với mã nguồn mở_B1

****C. Cấu hình docker compose:****

**Khởi động ubuntu**
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/8eac20ce-8b8f-4c3c-9a78-b46e9140153b" />

**nano ~/myapp/nginx/nginx.conf**

<img width="1315" height="1052" alt="image" src="https://github.com/user-attachments/assets/745c3f4d-48ab-4de3-8865-e5b48f455869" />

**1.Tạo thư mục: ~/myapp**

<img width="1024" height="765" alt="image" src="https://github.com/user-attachments/assets/eb1f1b88-45f8-4efd-86b4-deba55d861c8" />

**2.Chuyển vào trong thư mục ~/myapp**

<img width="943" height="711" alt="image" src="https://github.com/user-attachments/assets/26cd4e94-4669-4f87-b089-a83db92a9104" />

**3.Tạo thư mục: ./myweb**

<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/85d6d61a-1c23-48e4-9fdd-6bb8d29df42b" />

**4.Tạo file ./myweb/index.html (với nội dung là thông tin cá nhân của em)**

<img width="1913" height="1080" alt="image" src="https://github.com/user-attachments/assets/5fa13034-af70-4f7f-b061-9c696ce5ea26" />

**5.Tạo file docker-compose.yml để nó sẽ có các dịch vụ sau:**

Khai báo sử dụng nodered/node-red, cổng 1880, dữ liệu nằm tại thư mục ./nodered

Khai báo sử dụng nginx, cổng 80, cấu hình trong file ./nginx/nginx.conf

Mount thư mục ./myweb thành thư mục /myweb trong nginx

Mount file ./nginx/nginx.conf vào file /etc/nginx/nginx.conf trong nginx

Tạo file nginx.conf
<img width="818" height="1080" alt="image" src="https://github.com/user-attachments/assets/2fe5eba0-af1d-4ac2-92d0-b32f92c86a83" />

<img width="1738" height="1080" alt="image" src="https://github.com/user-attachments/assets/5743f699-ec49-44b0-a882-4a3669d064a8" />

****Em lỡ tạo nhầm thành thư mục lên xóa thư mục tạo lại thành file****  
<img width="1822" height="1080" alt="image" src="https://github.com/user-attachments/assets/500fd9ab-1907-49ef-8591-4d0b5ce8b5a1" />

<img width="582" height="145" alt="image" src="https://github.com/user-attachments/assets/75f22745-bca7-4e62-aec8-961a37a02415" />

**6. Edit file ./nginx/nginx.conf để:**

Cấu hình web server cổng 80

server_name là sub-domain (sub-domain tuỳ ý của em)

location / trỏ tới root là thư mục /myweb

location /api dùng proxy_pass trỏ tới 1 (hoặc nhiều) node http_in của nodered

<img width="2568" height="1926" alt="image" src="https://github.com/user-attachments/assets/6578f0bc-b84f-481f-a45b-57fab5516adb" />

<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/1ea1e4a6-0484-4448-827e-3472ffe8c07c" />

Mở Node-RED:
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/9af95bc0-42dd-455f-a360-17c4c1a90022" />

**7.Edit file ./nodered/settings.js để nodered bắt buộc đăng nhập**

<img width="1920" height="1071" alt="image" src="https://github.com/user-attachments/assets/77d57e53-f8b5-4f3a-927b-5c8c1483c0b7" />

<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/632405fc-97a0-40d0-8ffd-708fbc12b7bf" />

<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/ea74b632-9fdf-42c9-899d-594075ee3f1e" />

<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/a4e016d4-c2d3-464b-b112-ebdfe7e594dc" />

***Sau khi đăng nhập node-red : username: admin MK: 123456***
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/2f2b6d30-f373-4dbf-8a56-5606abcbea85" />
