# demo-nh-m-2
#include <iostream>
#include <cmath>

using namespace std;

int main() {
    // Nhập các hệ số a, b, c từ người dùng
    double a, b, c;
    cout << "Nhap he so a: ";
    cin >> a;
    cout << "Nhap he so b: ";
    cin >> b;
    cout << "Nhap he so c: ";
    cin >> c;

    // Tính delta
    double delta = b * b - 4 * a * c;

    // Kiểm tra giá trị của delta
    if (delta > 0) {
        // Hai nghiệm phân biệt
        double x1 = (-b + sqrt(delta)) / (2 * a);
        double x2 = (-b - sqrt(delta)) / (2 * a);
        cout << "Phuong trinh co hai nghiem phan biet: x1 = " << x1 << " va x2 = " << x2 << endl;
    } else if (delta == 0) {
        // Hai nghiệm kép
        double x = -b / (2 * a);
        cout << "Phuong trinh co nghiem kep: x = " << x << endl;
    } else {
        // Không có nghiệm thực
        cout << "Phuong trinh vo nghiem." << endl;
    }

    return 0;
}
