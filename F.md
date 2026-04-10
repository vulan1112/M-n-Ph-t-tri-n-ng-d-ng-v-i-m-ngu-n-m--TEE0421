****F. Gỡ lỗi:****

1. Nếu có lỗi xẩy ra trong quá trình triển khai docker compose up -dc

2. Thêm healthcheck cho myapi trong file docker-compose.yml

<img width="1897" height="1080" alt="image" src="https://github.com/user-attachments/assets/3993aa5b-3ff9-4ab6-af85-054c9d98696c" />

code check

<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/0fee2e58-0102-47cb-9d0a-3920715697d3" />

sau khi chạy test node-red vẫn ok

<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/cb7779af-cb22-4183-887c-42af258bc4bb" />

3. giới hạn resource cho một service: (tránh việc 1 service chiếm quá nhiều ram)

Mở file 

<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/019851e5-ded8-4047-972d-93152c09aa5c" />

code resource giới hạn

<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/f9fbf049-7638-430a-9e24-6b399859b887" />

<img width="1920" height="1067" alt="image" src="https://github.com/user-attachments/assets/700cb6ab-4c20-4816-85d6-c6d9e1bdcd0e" />

<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/680053b9-c8f7-4238-b286-658be159cb20" />

kiểm tra ram

<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/f7cb1b41-c143-45eb-8db2-6f98bc98297f" />

<img width="1913" height="1080" alt="image" src="https://github.com/user-attachments/assets/38f848a4-1c4e-48d8-9a75-5b932c51f32a" />
