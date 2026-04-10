# e.md
VU LAN_K225480106036_Phát triển ứng dụng với mã nguồn mở_bài tập 01

1. Chuyển vào trong thư mục ~/myapp

<img width="1918" height="1080" alt="image" src="https://github.com/user-attachments/assets/6276d20d-7936-4eb5-ae80-054a701bf259" />

2. Gõ lệnh để docker compose chạy: sẽ run tất cả các service khai báo trong file docker-compose.yml

<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/e3fc1707-defd-44e6-982e-3730fd6cce8d" />

<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/a396753a-d332-49b1-9065-02e8e208c959" />

<img width="1172" height="590" alt="image" src="https://github.com/user-attachments/assets/df6ac834-e1f0-4051-9895-177af1a1ceb2" />

<img width="971" height="598" alt="image" src="https://github.com/user-attachments/assets/c4f4f25b-ef7f-4c84-aff7-5af5fe982894" />

<img width="1920" height="1072" alt="image" src="https://github.com/user-attachments/assets/a7ceee23-9bfd-41a9-8688-5ffabd33c4ff" />

3. Kiểm tra các container đang chạy trong docker, nếu có cái nào bị restart cần tìm lỗi rồi edit lại docker-compose.yml

<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/1408b409-008c-4096-bcf3-4622ead1b9ba" />

<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/d15d8900-5df1-4906-aa91-f6704d43b18b" />

=> Không có container nào nỗi

4. Kiểm tra kiểm thử các service đang chạy độc lập thông qua ip và port của nó: ví dụ mở trình duyệt ip_ubuntu:1880 để check nodered đã chạy chưa

<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/a6c1ca4a-5460-432f-a44f-14d02745e1a3" />

=> ip_ubuntu:1880 đã chạy

<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/b129f164-f6eb-41ea-abe3-fde2eb47fd34" />

6. Sử dụng nodered: kéo nodered http_in , http_response, function : để tạo api get đơn giản (dùng cho /api proxy_pass của nginx)

<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/db5fc03c-3b6f-4d01-a7b2-a9ab1fd9fe28" />

<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/0f55af19-b202-4678-88ed-e9adb3dc33c0" />


<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/d36109c2-da86-43f1-b48d-fcbf865148e3" />

<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/014064c6-1f43-488b-8246-c4c290b03f9e" />
