# Nguyễn Quang Thắng - B24CDT246
## 1. Thư viện 
![alt text](image.png)
## 2. Khởi tạo kết nối với broker (broker sử dụng ở đây là emqx)
![alt text](image-1.png)
- broker emqx.io là broker public nên ko cần mật khẩu với tài khoản 
## 3. Cách đẩy dữ liệu lên broker 
![alt text](image-2.png)
## 4. Cách tải emqx lên pc 
- truy cập vào link và tải 
![alt text](image-3.png)
## 5. Kết nối broker với esp32
- Mở app emqx
- Bấm vào new connection
![alt text](image-4.png)
- 1 số thông tin cần thiết 
![alt text](image-6.png)
- các thông tin còn lại là tuỳ chỉnh của bản thân 
- bấm connect để kết nối với esp
![alt text](image-7.png)
- "new subscription" : đăng kí topic để nhận dữ liệu theo topic
## 6. Tạo giao diện nhận dữ liệu trực tiếp từ broker bằng node-red
- làm theo hướng dẫn trong link https://nodered.org/docs/getting-started/windows
### Cách chạy node-red
- mở cmd gõ "node-red" nhấn enter, lướt xuống để tìm địa chỉ (server now running...)
![alt text](image-9.png)
- truy cập địa chỉ ở trên để tạo flow
### Cách tạo flow trên node-red
#### input
- tìm "mqtt in" và kéo vào 
![alt text](image-10.png)
- nhấn đúp vào "mqtt in" để cài đặt 
- chọn server, nếu chưa có server bấm vào dấu cộng
![alt text](image-12.png)
![alt text](image-11.png)
- copy đúng topic và dán vào 
![alt text](image-13.png)
![alt text](image-14.png)
- bấm done
#### output
- lướt xuống dashboard và chọn giao diện tuỳ thích 
![alt text](image-15.png)
- bấm đúp vào 
- chọn group, nếu chưa có group bấm vào dấu cộng để tạo group
![alt text](image-16.png)
![alt text](image-17.png)
- bấm done
#### nối input với output với nhau 
- bấm deploy 
![alt text](image-19.png)


