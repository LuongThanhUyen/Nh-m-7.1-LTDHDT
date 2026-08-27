# Nh-m-7.1-LTDHDT
Khái niệm 1: Đối tượng (Objects) là các thực thể trong hệ thống hoạt động khi chương trình đang chạy. 
Một đối tượng được xác định rõ ràng thông qua 3 yếu tố:
Định danh (Identity): Tên hoặc mã phân biệt đối tượng này với đối tượng khác.
Trạng thái (State): Giá trị của các thuộc tính tại một thời điểm.
Hoạt động (Behavior): Các hành động mà đối tượng đó có thể thực hiện.

Khái niệm 2: Lớp (Class / Lớp đối tượng) là một khái niệm trừu tượng dùng để chỉ một tập hợp các đối tượng có chung các đặc tính trong hệ thống. Nó đóng vai trò như một khuôn mẫu (prototype) hay bản thiết kế để tạo ra các đối tượng.
Thành phần của Lớp:
Thuộc tính (Attributes): Tương ứng với thông tin/trạng thái chung của các đối tượng (Ví dụ: NhanHieu, MauSac, GiaBiet).
Phương thức (Methods): Tương ứng với các hành động của đối tượng (Ví dụ: KhoiDong(), TangToc()).
Các khả năng thiết kế của một Lớp:
Chỉ có thuộc tính, không có phương thức (Ví dụ: Lớp cấu hình chứa dữ liệu tĩnh).
Chỉ có phương thức, không có thuộc tính (Ví dụ: Lớp tiện ích tính toán toán học).
Có cả thuộc tính và phương thức (Trường hợp phổ biến nhất).
Lớp trừu tượng (Abstract Class): Lớp đặc biệt dùng làm khuôn mẫu chung và không tạo trực tiếp đối tượng tương ứng.

So sánh và Mối liên hệ giữa Lớp và Đối tượng
Dù có mối quan hệ chặt chẽ, bản chất của lớp và đối tượng hoàn toàn khác nhau:
Bản chất: lớp là một khái niệm trừu tượng, mang tính lý thuyết; trong khi đối tượng là một thực thể cụ thể, có thực và tồn tại trong hệ thống khi chương trình đang chạy.
Số lượng: một lớp chỉ cần định nghĩa một lần, nhưng từ lớp đó có thể tạo ra vô vô số đối tượng khác nhau.
Vai trò trong hệ thống: lớp định nghĩa ra khuôn mẫu chứa thông tin thuộc tính và phương thức; đối tượng sử dụng các thuộc tính và trực tiếp thực thi các phương thức/hành động đó.
