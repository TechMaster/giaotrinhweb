# Basic
## 1. GET Method
### 1.1 Hello World
Chạy web app ở cổng 8080, khi người dùng vào http://localhost:8080 thì thấy web page có dòng chữ HelloWorld

### 1.2 Get method không tham số
Ứng dụng web ở cổng 8080 trả về web page ở 2 đường dẫn
```
/
/aboutus
```
### 1.3 Get method có tham số
Ứng dụng web ở cổng 8080 trả về web page ở 3 đường dẫn. Hai đường dẫn đầu như ví dụ trước
```
/
/aboutus
```
Truyền vào tham số URL param để in màn hình
```/say?name=Tom```

### 1.4 Đọc URL parameter để xử lý logic
/info?type
```
case type == 'os' then
   hiển thị tên hệ điều hành (dùng hàm để lấy đừng gán constant string)
case type == 'framework" then
   hiển thị tên web framework + version
case type == 'date' then
   lấy thời gian trên server hiển thị
```
### 1.5 Liệt kê file trong thư mục
```/``` liệt kê tất các file trong thư mục, có link tải về được ở mỗi tên file
hint: Hãy sử dụng hàm có sẵn của web framework sau đó mới tự lập trình
dùng hàm API để liệt kê thư mục rồi trả về. Xem ví dụ dưới
```
.
├── Basic.md
├── LICENSE
├── MiniProject.md
├── Project.md
└── ReadMe.md

0 directories, 5 files
```

### 1.6 Liệt kê cả file và folder trong thư mục (Khó)
```/``` liệt kê tất các file, folder trong thư mục. Click vào folder sẽ mở ra thư mục sâu hơn.
Click vào parent sẽ ra thư mục cha

## 2. POST Method
### 2.1 Cộng 2 số
```GET /add``` hiển thị form gồm 2 trường A và B, ấn nút submit trả về kết quả như sau ```A + B = C```
Nâng cao:
- Kiểm tra dữ liệu nhập vào tại server, nếu tham số không có dạng số hãy báo lỗi
- Bổ xung thêm ```/minus``` và ```/multiply``` để trừ và nhân

### 2.2 Login form user name, password

```GET /login``` hiển thị form login gồm user name và password

```POST /login``` người dùng gửi lên user name và password
Server có sẵn các bộ dữ liệu ```{name, password}``` gồm có ```[{'admin', '@123'}, {'bob', '#321'}, {'jane', 'bob'}]```
```
if login == thành công then
  redirect sang một trang /loginsuccess
else
  redirect sang một trang /loginfail
endif
```

### 2.3 Upload một file
```POST \upload``` Upload một file bất kỳ lên server, trả về link để tải file đó về.
Cải tiến server để chỉ cho phép upload file ảnh *.png, *.jpg, *.gif, kích thước file dưới 500 Kbytes


### POST method upload nhiều file

### POST method nhiều trường + file upload

### REST API


### Dùng session lưu biến counter
In ra màn hình biến counter tăng mỗi khi refresh web site.
Yêu cầu sử dụng session để lưu biến counter

### Dùng session lưu giỏ hàng (ứng dụng Multiple Web Page)
Trang chủ hiện ra danh sách 4 mặt hàng
- Cam


## 2. Ứng dụng đơn giản

## Ứng dụng trung bình

## Ứng dụng phức tạp