# Toán tử so sánh
- `==`: Toán tử so sánh =
- `&&`: Toán tử và
- `!`: Toán tử sai
- `||`: Toán tử hoặc
- `>`, `<`, `>=`, `<=`


| A | B | `A&&B` | `A\|\|B` | `!A`|
|---|---|---|---|---|
|0|0|0|0|1|
|0|1|0|1|1|
|1|0|0|1|0|
|1|1|1|1|0|

# Câu điều kiện
## Câu điều kiện thiếu `if`
```cpp
if(<điều kiện>) {
    <khối lệnh>
}
```
## Câu điều kiện đủ `if` `else`
```cpp
if(<điều kiện>) {
    <khối lệnh>
}
else {
    <khối lệnh>
}
```
## Câu điều kiện `if` và `else if`
```cpp
if(<điều kiện>) {
    <khối lệnh>
}
else if(<điều kiện>) {
    <khối lệnh>
}
else if(<điều kiện>) {
    <khối lệnh>
}
else if(<điều kiện>) {
    <khối lệnh>
}
else {
    <khối lệnh>
}
```
## Điều kiện switch case
```c++
switch (<biến xét điều kiện>)
    {
    case <giá trị 1>:
    {
        <khối lệnh>
        break;
    }
    case <giá trị 2>:
    {
        <khối lệnh>
        break;
    }
    default: // giá trị còn lại
    {
        <khối lệnh>
        break;
    }
}
```
Lưu ý:
- Những từ khoá switch và break phải luôn có
- Biến xét điều kiện và các giá trị phải cùng kiểu dữ liệu
## Tìm giá trị lớn nhất giữa các số
```cpp
#include <iostream>
using namespace std;
int main()
{
    int a, b, c;
    cin >> a >> b >> c;
    int max_value = 0;
    if (max_value < a)
    {
        max_value = a;
    }
    if (max_value < b)
    {
        max_value = b;
    }
    if (max_value < c)
    {
        max_value = c;
    }
    cout << max_value;
}
```
## Thư viện cmath trong c++
- sqrt(<giá trị>): Trả về căn
- sin, cos, tan
- abs(<giá trị>): trị tuyệt đối
- min(<giá trị1>, <giá trị 2>): trả về giá trị nhỏ hơn
- max(<giá trị1>, <giá trị 2>): trả về giá trị lớn hơn