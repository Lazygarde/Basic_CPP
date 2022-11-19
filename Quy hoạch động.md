# Quy hoạch động
## Các khái niệm cơ bản về quy hoạch động
* Là một kĩ thuật thiết kế thuật toán theo kiểu chia bài toán lớn thành các bài toán con, sử dụng lời giải của các bài toán con để tìm lời giải cho bài toán ban đầu.
* Khác với chia để trị, quy hoạch động thay vì gọi đệ quy, sẽ tính trước lời giải của các bài toán con và lưu vào bộ nhớ (thường là một mảng), và sau đó lấy lời giải của bài toán con ở trong mảng đã tính trước để giải bài toán lớn
> Về mặt bản chất, ngoài những thuật ngữ cao cấp, thì quy hoạch động là bài toán truy hồi kết hợp ghi nhớ.
* Ví dụ: bài toán tìm số Fibonacci thứ n

  Cách tiếp cận QHĐ:
  - Số Fibonacci thứ n được tính bằng tổng của 2 số Fibonacci thứ n-1 và n-2
  - Vì vậy ta có mảng lưu kết quả là f[], f[i] = f[i-1] + f[i-2]

  ![image](https://user-images.githubusercontent.com/84316258/202840254-ea4e845f-b569-476e-9956-6a2ad33f3a87.png)

* Ví dụ: Bài toán tìm số nguyên lớn nhất của một dãy số
  
  Cách tiếp cận QHĐ:
  - Ta coi trạng thái thứ i sẽ là số nguyên lớn nhất của dãy số từ 1 -> i.
  - Vì vậy ta có công thức: f[i] = max(f[i-1], a[i]) (a[] là dãy số cho trước và f[] là mảng lưu kết quả)

  ![image](https://user-images.githubusercontent.com/84316258/202840323-c06b7da1-cd3d-44b9-828d-bd94043ac4d8.png)

## Khi nào thì sử dụng quy hoạch động?
* Đó là một câu hỏi rất khó trả lời. Không có một công thức nào cho các bài toán như vậy.
* Tuy nhiên, có một số tính chất của bài toán mà bạn có thể nghĩ đến quy hoạch động. Dưới đây là hai tính chất nổi bật nhất trong số chúng:
  * Bài toán có các bài toán con gối nhau, lặp lại.
  * Bài toán có cấu trúc con tối ưu.
 
* Có thể nhận thấy bản chất QHD là truy hồi có nhớ, nên những bài toán mà có thể làm bằng cách truy hồi, quay lui thường có thể sử dụng QHD.