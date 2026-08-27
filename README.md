# Nh-m-7.1-LTDHDT
Tính đa hình
- Cho phép các lớp được định nghĩa các phương
thức trùng nhau: cùng tên, cùng số lượng và
kiểu tham số, cùng kiểu trả về.
-  Việc định nghĩa phương thức trùng nhau của
các lớp kế thừa nhau còn được gọi là sự nạp
chồng phương thức.
-  Khi gọi các phương thức trùng tên, dựa vào đối
tượng đang gọi mà chương trình sẽ thực hiện
phương thức của lớp tương ứng
Ví dụ: tôi có một lớp animal gồm Dog và Cat
Tôi muốn chương trình xuất ra âm thanh của chúng.
-Lớp animal có phương thức sound, dog và cat cũng đều có định nghĩa sound.
animal.sound() -> động vật kêu
dog.sound(); -> tiếng chó kêu
cat.sound(); -> tiếng mèo kêu.
=> điều này giải thích cho :“Khi gọi các phương thức trùng tên, dựa vào đối tượng đang gọi mà chương trình sẽ thực hiện phương thức của lớp tương ứng.”
- chương trình c minh họa cho tính kế thùa : 
#include <stdio.h>

typedef struct Animal Animal;

struct Animal {
    void (*sound)(Animal*);
};

void dog_sound(Animal* a) {
    printf("Gau gau\n");
}

void cat_sound(Animal* a) {
    printf("Meo meo\n");
}

int main() {
    Animal dog;
    Animal cat;

    dog.sound = dog_sound;
    cat.sound = cat_sound;

    dog.sound(&dog);
    cat.sound(&cat);

    return 0;
}

Kết quả nhận được sẽ là : gâu gâu và meo meo. Vì trong animal có void sound mà Dog và Cat cũng có void sound nhưng cách thực hiện nó khác nhau.
từ trong chương trình c ta thấy :
Animal có phương thức sound(). Dog và Cat kế thừa từ Animal và ghi đè phương thức sound() với cách thực hiện riêng. Khi gọi dog.sound() thì chương trình thực hiện Dog::sound(), còn khi gọi cat.sound() thì thực hiện Cat::sound(). Đây là ghi đè phương thức (overriding) và là một biểu hiện của đa hình (polymorphism).
