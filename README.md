# 📱 Ứng Dụng Chat Thời Gian Thực


Ứng dụng chat bảo mật thời gian thực xây dựng bằng Flask và công nghệ WebSocket, với tính năng mã hóa end-to-end và xác thực người dùng.

## 🌟 Tính Năng Chính

- **Xác thực bảo mật**: Đăng ký và đăng nhập người dùng với mật khẩu được mã hóa

- **Nhắn tin thời gian thực**: Gửi tin nhắn tức thì với WebSocket

- **Mã hóa end-to-end**: Mã hóa tất cả tin nhắn bằng thuật toán Fernet

- **Chia sẻ tệp**: Gửi hình ảnh, tài liệu và các loại tệp khác

- **Yêu cầu kết nối**: Gửi yêu cầu kết nối trước khi trò chuyện

- **Theo dõi người dùng trực tuyến**: Xem ai đang online trong thời gian thực

## ⚙️ Công Nghệ Sử Dụng

**Frontend:**

- HTML5/CSS3

- JavaScript (Vanilla)

- Socket.IO

**Backend:**

- Python 3.9+

- Flask

- Flask-SocketIO

- Cryptography (Fernet)

## 🚀 Bắt Đầu

### Yêu Cầu Hệ Thống

- Python 3.9 trở lên

- Trình quản lý gói Pip

### Cài Đặt

1. Sao chép kho lưu trữ:

```bash

git clone https://github.com/giangleco/chat_app.git

cd ung-dung-chat

```

2. Cài đặt các gói phụ thuộc cho cả server và client:

```bash

# Cài đặt phụ thuộc cho server

cd server

pip install -r requirements.txt

# Cài đặt phụ thuộc cho client

cd ../client

pip install -r requirements.txt

```

### Chạy Ứng Dụng

#### Cách 1: Sử Dụng VS Code (Khuyến Nghị)

1. Mở 2 terminal riêng biệt trong VS Code

2. Ở Terminal 1:

```bash

cd server

python app.py

```

3. Ở Terminal 2:

```bash

cd client

python app.py

```

#### Cách 2: Sử Dụng Command Line

```bash

# Khởi động server

cd server && python app.py &

# Khởi động client

cd ../client && python app.py &

```

## 🔑 Truy Cập Ứng Dụng

1. **Giao Diện Người Dùng**:

- Mở trình duyệt và truy cập: [http://127.0.0.1:5001/login](http://127.0.0.1:5001/login)

- Đăng ký tài khoản mới hoặc đăng nhập với thông tin hiện có

- Bắt đầu trò chuyện với người dùng khác!

2. **Bảng Điều Khiển Quản Trị**:

- Truy cập bảng điều khiển tại: [http://192.168.3.191:5000/](http://192.168.3.191:5000/)

- Theo dõi người dùng đang hoạt động và trạng thái server

## 🛠 Cấu Trúc Dự Án

```

ung-dung-chat/

├── client/                  # Ứng dụng client

│   ├── app.py               # Ứng dụng chính client

│   ├── templates/           # Giao diện HTML

│   │   ├── chat.html        # Giao diện chat

│   │   ├── login.html       # Trang đăng nhập

│   │   └── users.html       # Danh sách người dùng online

│   └── requirements.txt     # Phụ thuộc client

│

├── server/                  # Ứng dụng server

│   ├── app.py               # Ứng dụng chính server

│   ├── templates/           # Giao diện server

│   │   └── server.html      # Bảng điều khiển admin

│   ├── uploads/             # Thư mục tải lên tệp

│   ├── users.json           # Cơ sở dữ liệu người dùng

│   ├── messages.json        # Cơ sở dữ liệu tin nhắn

│   ├── requests.json        # Yêu cầu kết nối

│   └── requirements.txt     # Phụ thuộc server

│

├── .gitignore               # File bỏ qua của Git

├── LICENSE                  # Giấy phép dự án

└── README.md                # File này

```


## 👥 Người Đóng Góp

- [Giang Lê Hoàng ](https://github.com/giangleco)

```
