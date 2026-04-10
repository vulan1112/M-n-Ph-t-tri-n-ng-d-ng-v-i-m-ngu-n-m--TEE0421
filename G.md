****G. Triển khai ứng dụng đến End-user****

1. Trong Cloudflare: Tạo tunnel (đường hầm), chọn loại triển khai cho docker

<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/daf2f848-77a1-44e8-963d-42be7bc89fdb" />

<img width="1919" height="1064" alt="image" src="https://github.com/user-attachments/assets/3530c17c-b606-4ca7-9fa7-a8649ab4232b" />

<img width="1920" height="1077" alt="image" src="https://github.com/user-attachments/assets/82d57c73-5bf7-45ca-8466-a0c3b7b77b48" />

<img width="1920" height="1061" alt="image" src="https://github.com/user-attachments/assets/04d511db-b65d-4cf4-8650-49640edd3b4c" />

 **lanvukhong.vulan2k4bg.id.vn**
 
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/4a734526-2e64-437e-96c7-a859395ba423" />

Kết quả tính

<img width="1920" height="1063" alt="image" src="https://github.com/user-attachments/assets/ef078bd0-a8b9-4042-bad0-77090c114c6d" />

2. Convert lệnh docker run ... sang dạng docker compose

<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/dc6a74b3-1a52-4cea-94cb-b2d3a9c4a9ed" />

<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/cf56a8b6-5f93-4da1-923e-fa6557aec0a9" />

3. Khai báo kết quả convert vào trong file docker-compose.yml

Phần này đã làm trước đó giờ chạy lại

<img width="1920" height="463" alt="image" src="https://github.com/user-attachments/assets/ed360973-9159-4ffc-972b-09e744c5290f" />

4. Chạy lại docker compose

<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/aa5293ab-0da3-4198-b94a-d08edc71b099" />

<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/b48e1201-1f0d-436c-ad66-4773b14737b9" />

<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/95a4c39a-4a34-446f-8e2c-2f11e5c9c055" />

<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/c0ef96cb-934a-492c-b0d4-b09f4d1e299c" />

5.Public ứng dụng bằng cách thêm 1 router trỏ tới container đang chạy trong docker, dữ liệu sẽ đi qua tunnel, url dạng sub-domain

<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/1229b64f-f022-4432-9c9e-dd00dedc87b1" />

<img width="1920" height="1073" alt="image" src="https://github.com/user-attachments/assets/7a3c6692-45f6-461b-9cd9-b253172d9a47" />

<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/9411a245-1dd1-4273-a40a-0bf6607d9191" />

<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/289aa5ea-7f2d-4225-8b04-0a8aca1e304a" />

<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/4bab3f9b-0d23-485d-9eea-87ee95cea849" />

6.Kiểm tra url sub-domain đã hoạt động public cho mọi end-user

