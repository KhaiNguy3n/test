# ptud-gk-de-2

## 📌 Giới thiệu
Dự án **ptud-gk-de-2** là một ứng dụng quản lý công việc (Task Management) sử dụng Django. Hệ thống cho phép người dùng (user) tạo công việc, theo dõi trạng thái hoàn thành và thời gian hoàn thành. Quản trị viên (admin) có thể quản lý toàn bộ công việc của các user.

## 👤 Thông tin cá nhân
- **Họ và tên:** Nguyễn Khải
- **Email:** [khaikaka555@gmail.com]
- **MSSV:** 20025651
- **GitHub:** [https://github.com/KhaiNguy3n/ptud-gk-de-2]

## ✨ Tính năng chính
- Đăng nhập và phân quyền (Admin, User)
- Quản lý công việc (Task): tạo, cập nhật, xóa
- Theo dõi tình trạng công việc (Chưa hoàn thành, Đang thực hiện, Đã hoàn thành)
- Ghi nhận thời gian tạo và thời gian hoàn thành công việc
- Trang thống kê số liệu công việc

## 📂 Cấu trúc thư mục
```
ptud-gk-de-2/
│── manage.py           # File chạy Django
│── requirements.txt    # Danh sách thư viện cần cài đặt
│── README.md           # Hướng dẫn dự án
│── gk/                 # Thư mục chứa project Django
│   ├── settings.py     # Cấu hình Django
│   ├── urls.py         # Điều hướng URL
│   ├── wsgi.py         # Cấu hình chạy trên server
│── task/              # Ứng dụng quản lý công việc
│   ├── models.py       # Định nghĩa database
│   ├── views.py        # Xử lý logic
│   ├── urls.py         # Điều hướng cho app
│   ├── templates/      # HTML templates
│   ├── static/         # Tệp tĩnh (CSS, JS)
│── db.sqlite3          # Cơ sở dữ liệu SQLite
```

## 🚀 Hướng dẫn cài đặt

### 1. Clone dự án từ GitHub
```bash
git clone https://github.com/KhaiNguy3n/ptud-gk-de-2
cd ptud-gk-de-2
```

### 2. Tạo môi trường ảo (virtual environment) và cài đặt thư viện
```bash
python -m venv venv
source venv/bin/activate   # Trên macOS/Linux
venv\Scripts\activate      # Trên Windows
pip install -r requirements.txt
```

### 3. Chạy migration để tạo database
```bash
python manage.py makemigrations
python manage.py migrate
```

### 4. Tạo tài khoản Admin
```bash
python manage.py createsuperuser
```
Nhập thông tin đăng nhập admin theo hướng dẫn.

### 5. Chạy server Django
```bash
python manage.py runserver
```
Truy cập `http://127.0.0.1:8000/` để sử dụng.

## 📊 Thống kê mô tả dữ liệu
- Tổng số công việc đã tạo
- Số lượng công việc theo trạng thái (Chưa hoàn thành, Đang thực hiện, Đã hoàn thành)
- Tỷ lệ công việc hoàn thành đúng hạn

## 📜 Hướng dẫn sử dụng
1. **User:**
   - Đăng ký tài khoản
   - Đăng nhập và tạo công việc mới
   - Cập nhật trạng thái công việc
   - Xem danh sách công việc cá nhân
2. **Admin:**
   - Quản lý toàn bộ công việc của user
   - Thống kê công việc theo trạng thái
   - Quản lý người dùng

## 📄 Giấy phép
Dự án này được phát triển với mục đích học tập.

