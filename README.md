Bước 1: Download và cài đặt SQL Server 2025, phiên bản Developer
<img width="1906" height="1076" alt="image" src="https://github.com/user-attachments/assets/c63dc87b-2657-4854-9634-7454a7ee072e" />
Bước 2 : Cấu hình cho SQL Server làm việc ở cổng động (Dynamic Port), TCP - 3xxxx( 36078)_msv: K235480106078
<img width="1910" height="1079" alt="image" src="https://github.com/user-attachments/assets/1220c956-8054-4c99-bdd6-e527f945a732" /> 
<img width="1913" height="1068" alt="image" src="https://github.com/user-attachments/assets/41c41990-2c00-4f4b-88f1-cf6c5d97b8b1" />
<img width="1904" height="1079" alt="image" src="https://github.com/user-attachments/assets/42ec9e6f-92b0-4e01-8293-74133787e0bf" />
Bước 3: Kiểm tra xem service SQL Server có đang running và mở đúng cổng đã chọn hay không? _ Sử dụng lệnh trên cmd: netstat -ano | findstr LISTENING
<img width="1355" height="756" alt="image" src="https://github.com/user-attachments/assets/83762473-bc79-4c20-b02d-34f562397b61" /> 
Bước 4 :Cài đặt SQL Server Management Studio
<img width="1919" height="1070" alt="image" src="https://github.com/user-attachments/assets/6990c767-e16a-4033-88f8-3b8458c55bf3" />
Bước 5 :Chạy phần mềm ssms để Đăng nhập vào SQL Server bằng 2 cách:
  Cách 1: Windows Authentication 
  <img width="1915" height="1079" alt="image" src="https://github.com/user-attachments/assets/ee1f59b7-6bc7-4d2f-b308-905fd69ef9d5" />
  cách 2 : SQL Server Authentication
  <img width="1914" height="1079" alt="image" src="https://github.com/user-attachments/assets/cad62f68-2708-4485-91e9-4739249160be" />
Bước 6 : Tạo cơ sở dữ liệu mới (create database) với tên tuỳ ý, chọn Path (nơi lưu trữ db) cho file lưu dữ liệu và file lưu log ở ổ đĩa khác với ổ C
<img width="1919" height="1079" alt="image" src="https://github.com/user-attachments/assets/d541d027-eba5-4432-b738-434d890fc2b3" />
Bước 7 :Tạo bảng dữ liệu (create and design table) với tên bảng tuỳ ý, có các trường dữ liệu phù hợp với dữ liệu của file data mẫu (CSV), với Khoá chính (Primary Key) là trường masv.
