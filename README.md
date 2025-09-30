Ứng dụng quản lý người dùng với tính năng đăng nhập, đăng ký
Đăng Huyền Trân 24521810
Nguyễn Thị Tuyết Thoa 24521719
Huỳnh Minh Tú 24521907
Võ Lê Uyên Trang 24521823
Mô tả bài tập: Ứng dụng quản lý người dùng đơn giản bằng C# WinForms, có hai chức năng chính là Đăng ký và Đăng nhập.
Khi người dùng đăng ký, thông tin sẽ được lưu xuống SQL Server, cụ thể là lưu vào bảng Users trong cơ sở dữ liệu Nhom9exercise2.2.
Mật khẩu người dùng sẽ được mã hóa bằng SHA-256 trước khi lưu để tăng tính bảo mật.
Sau khi đăng ký xong, người dùng có thể đăng nhập bằng tài khoản vừa tạo. Nếu đăng nhập đúng, ứng dụng sẽ chuyển sang Form chính và hiển thị thông tin người dùng.
Ứng dụng này được làm bằng Visual Studio (C# WinForms) và kết nối đến SQL Server
Hướng dẫn cài đặt: Visual Studio
.NET Framework 4.7.2 hoặc tương đương
SQL Server 
SQL Server Management Studio (SSMS)
Cách cài đặt & chạy project: 
Bước 1: Clone project từ GitHub
Mở Git Bash trong thư mục bạn muốn lưu, nhập lệnh:
git clone https://github.com/<tên_tài_khoản>/<tên_repo>.git
Sau khi clone xong, mở project trong Visual Studio bằng file .sln.
Bước 2: Tạo cơ sở dữ liệu trong SQL Server
Mở SQL Server Management Studio (SSMS) → tạo mới database
Bước 3: Cập nhật chuỗi kết nối (Connection String)
Mở file App.config hoặc phần code trong FormLogin.cs/FormRegister.cs, cập nhật dòng sau bằng Server Name và Database: string connectionString = 
    "Server=localhost\\MSSQLSERVER01;Database=Nhom9exercise2_2;User Id=sa;Password=123456;";
Bước 4: Build & Run
Trong Visual Studio:
Nhấn Start (F5) để chạy ứng dụng
Giao diện sẽ hiển thị Form Đăng nhập
Nếu chưa có tài khoản, bấm Đăng ký để tạo mới
Hướng dẫn sử dụng:
Mở ứng dụng → giao diện Đăng nhập
Chưa có tài khoản → click nút “Đăng ký”
Nhập:
Tên đăng nhập
Mật khẩu & Xác nhận mật khẩu
Email
→ Nhấn Đăng ký
Khi đăng ký thành công → quay lại màn hình Đăng nhập
Đăng nhập bằng tài khoản vừa tạo
Sau khi đăng nhập thành công → ứng dụng chuyển sang Form chính, hiển thị thông tin người dùng.
