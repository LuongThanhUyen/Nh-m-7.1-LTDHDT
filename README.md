# Nh-m-7.1-LTDHDT
# Khái niệm 1: Đối tượng (Objects) là các thực thể trong hệ thống hoạt động khi chương trình đang chạy. 
Một đối tượng được xác định rõ ràng thông qua 3 yếu tố: Định danh (Identity): Tên hoặc mã phân biệt đối tượng này với đối tượng khác, Trạng thái (State): Giá trị của các thuộc tính tại một thời điểm, Hoạt động (Behavior): Các hành động mà đối tượng đó có thể thực hiện.
Ví dụ:
Đối tượng cụ thể từ Lớp BankAccount:
Định danh: Tài khoản của bạn Ly (STK: 1900123456).
Trạng thái: TenChuTaiKhoan = "Dao Huong Ly", SoDu = 5,000,000 VNĐ.
Hành vi: Thực hiện lệnh rutTien(500000).

# Khái niệm 2: Lớp (Class / Lớp đối tượng) là một khái niệm trừu tượng dùng để chỉ một tập hợp các đối tượng có chung các đặc tính trong hệ thống. Nó đóng vai trò như một khuôn mẫu (prototype) hay bản thiết kế để tạo ra các đối tượng.
Thành phần của Lớp:
Thuộc tính (Attributes): Tương ứng với thông tin/trạng thái chung của các đối tượng.
Phương thức (Methods): Tương ứng với các hành động của đối tượng.
Các khả năng thiết kế của một Lớp:
Chỉ có thuộc tính, không có phương thức.
Chỉ có phương thức, không có thuộc tính.
Ví dụ:
Lớp Tài khoản ngân hàng (BankAccount):
Thuộc tính: soTaiKhoan, tenChuTaiKhoan .
Phương thức: guiTien(), rutTien(), chuyenKhoan()
Có cả thuộc tính và phương thức (Trường hợp phổ biến nhất).
# Lớp trừu tượng (Abstract Class): Lớp đặc biệt dùng làm khuôn mẫu chung và không tạo trực tiếp đối tượng tương ứng.

# phân biệt giữa Lớp (Class) và Lớp trừu tượng (Abstract Class)
Về định nghĩa và bản chất:
- Lớp (Concrete Class): Là bản thiết kế hoàn chỉnh, định nghĩa chi tiết toàn bộ thuộc tính và triển khai đầy đủ logic cho tất cả các phương thức.
- Lớp trừu tượng (Abstract Class): Là bản thiết kế dở dang hoặc khung xương, dùng làm mẫu chung cho các lớp con kế thừa chứ chưa cài đặt chi tiết cho toàn bộ hành vi.
Về khả năng khởi tạo đối tượng:
- Lớp: Có thể dùng từ khóa new để tạo trực tiếp đối tượng thực thi trong chương trình.
- Lớp trừu tượng: Không thể khởi tạo đối tượng trực tiếp.
Về phương thức:
- Lớp: Chỉ chứa các phương thức thông thường có phần thân triển khai {}.
- Lớp trừu tượng: Có thể chứa cả phương thức thông thường lẫn phương thức trừu tượng (phương thức không có phần thân, chỉ có tên và tham số).
Về tính kế thừa và triển khai:
- Lớp: Lớp con khi kế thừa lớp thông thường có thể chọn ghi đè (override) hoặc giữ nguyên các phương thức của lớp cha.
- Lớp trừu tượng: Bắt buộc lớp con (nếu là lớp cụ thể) phải viết code triển khai chi tiết cho tất cả các phương thức trừu tượng do lớp cha quy định.
Về từ khóa khai báo (trong các ngôn ngữ OOP như Java, C#):
- Lớp: Khai báo bằng từ khóa "class".
- Lớp trừu tượng: Bắt buộc phải khai báo bằng từ khóa "abstract class".
Về mục đích sử dụng:
- Lớp: Dùng để tạo ra các thực thể cụ thể trực tiếp lưu trữ dữ liệu và xử lý tác vụ khi chương trình chạy.
- Lớp trừu tượng: Dùng để xây dựng khung cấu trúc chuẩn cho một nhóm đối tượng có liên quan, giúp đảm bảo tính nhất quán và tái sử dụng mã nguồn.

# So sánh và Mối liên hệ giữa Lớp và Đối tượng
Dù có mối quan hệ chặt chẽ, bản chất của lớp và đối tượng hoàn toàn khác nhau:
Bản chất: lớp là một khái niệm trừu tượng, mang tính lý thuyết; trong khi đối tượng là một thực thể cụ thể, có thực và tồn tại trong hệ thống khi chương trình đang chạy.
Số lượng: một lớp chỉ cần định nghĩa một lần, nhưng từ lớp đó có thể tạo ra vô vô số đối tượng khác nhau.
Vai trò trong hệ thống: lớp định nghĩa ra khuôn mẫu chứa thông tin thuộc tính và phương thức; đối tượng sử dụng các thuộc tính và trực tiếp thực thi các phương thức/hành động đó.

