# Nh-m-7.1-LTDHDT
# sự kế thừa: lớp dẫn xuất kế thừa lớp cơ 
# lớp dẫn xuất có thể sử dụng các thuộc tính và phương thức của lớp cơ sở 
# chỉ cần cài đặt thuộc tính ở lớp cơ sở=lớp dẫn xuất có thể sử dụng tất cả các thuộc tính đó 
# tránh sự cài đặt trùng lặp mã nguồn của chương trình (các lớp dẫn xuất cần sử dụng cùng thuộc tính=chỉ cần thêm thuộc tính ở 1 lớp cơ sở)
# nếu muốn thay đổi dữ liệu ở nhiều lớp dẫn xuất cùng 1 lúc=chỉ cần thay dổi ở lớp cơ sở
#include <iostream>
class Animal
{
public:
    void eat()
    {
        cout << "an" << endl;
    }
    void sleep()
    {
        cout << "ngu" << endl;
    }
};

class Dog : public Animal
{
public:
    void bark()
    {
        cout << "Gau gau" << endl;
    }
};

int main()
{
    Dog dog;
    dog.eat();
    dog.sleep();
    dog.bark();

    return 0;
}
