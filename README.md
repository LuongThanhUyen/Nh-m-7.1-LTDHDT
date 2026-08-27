# Nh-m-7.1-LTDHDT
## Thành viên nhóm 7
1. Lương Thanh Uyên - Nhóm trưởng
2. Nông Thị Thanh Hiền
3. Sỹ Bảo Châu
4. Ngô Thu Hương
5. Đào Hương Ly
## Nội dung
- Đối tượng // Đào Hương Ly
- Lớp đối tượng // Đào Hương Ly
- Trừu tượng hóa đối tượng theo chức năng // Ngô Thu Hương
- Trừu tượng hóa đối tượng theo dữ liệu // Ngô Thu Hương
- Khái niệm kế thừa // Nông Thị Thanh Hiền
- Khái niệm đóng gói // Lương Thanh Uyên
- Khái niệm đa hình // Sỹ Bảo Châu

#Đóng gói có thể hiểu đơn giản là:

Che giấu dữ liệu và cách cài đặt bên trong đối tượng, chỉ cho phép truy cập theo cách phù hợp.

Tài liệu nêu hai ý chính:

Che giấu sự cài đặt chi tiết bên trong phương thức.
Che giấu dữ liệu bên trong đối tượng.

Ví dụ:

          SINH VIÊN
     ┌─────────────────┐
     │ private         │
     │ - điểm          │
     │ - mã SV         │
     ├─────────────────┤
     │ public          │
     │ + nhập()        │
     │ + xuất()        │
     └─────────────────┘

Người bên ngoài không tùy ý truy cập dữ liệu private.
