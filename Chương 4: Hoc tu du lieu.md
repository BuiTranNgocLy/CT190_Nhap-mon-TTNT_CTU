# Máy học là gì?
- Là chương trình máy tính cho phép `học tự động` từ `dữ liệu` để nhận biểt các mẫu phức tạp, tạo ra hành vi ứng xử thông minh với các trường hợp mới đến.
- Một chương trình máy tính gọi là `học từ kinh nghiệm E` với 1 vài lớp của `vấn đề T` và `độ đo hiệu quả P` nếu `hiệu năng của vấn đề T` đánh giá theo `tiêu chí P` cải thiện từ `kinh nghiệm E`.
  - `Cải thiện tác vụ T`
  - `Độ đo hiệu quả P`
  - `Dựa trên kinh nghiệm E`
# Phân loại máy học
  ## 1. Học không giám sát - Unsupervised Learning
- Là thuật toán `mô hình hóa` 1 tập dữ liệu đầu vào `không được gán nhãn` ( lớp, giá trị cần dự báo), `gom cụm nhóm` (clustering, unsupervised learning) xây dựng mô hình gom cụm (không có nhãn). `Dữ liệu cùng nhóm có tính chất tương tự u`.
- Xây dựng` mô hình H` từ `tập dữ liệu (X1,X2,..,Xm)`

 ## 2. Học có giám sát – supervised learning
 - Thuật toán học tạo ra một hàm ánh xạ dữ liệu đầu vào tới kết quả đích mong muốn. Tập dữ liệu dùng để huấn luyện phải `được gán nhãn, lớp hay giá trị cần dự báo`
   - `Bài toán Hồi quy` (Regression): xây dựng mô hình phân loại dựa trên `dữ liệu` tập học đã có nhãn (lớp) là `giá trị liên tục.`
   - `Bài toàn phân lớp` (classification, supervised learning): xây dựng mô hình phân loại dựa trên `dữ liệu` tập học đã có nhãn (lớp) là `kiểu liệt kê`
 
  ## 3. Học bán giám sát- semi- supervised learning
  - Dữ liệu thu thập một `phần nhỏ đã được gán nhãn`, `phần lớn` còn lại chưa được `gán nhãn trong quá trình học`
    - `LU learning`: Học với một `bộ nhỏ các ví dụ được gắn nhãn` và một `bộ lớn các ví dụ không được gắn nhãn`
    - `PU learning`: Học với các ví dụ `Tích cực và Không gắn nhãn` (không có ví dụ phủ định được gắn nhãn)


  ## 4. Học củng cố / học tăng cường: reinforcement learning
  - Là một cách tiếp cận tập trung vào việc học để `hoàn thành được mục tiê` bằng việc `tương tác trực tiếp với môi trường.`
  - Đây là các bài toán giúp cho một hệ thống `tự động xác định hành động` dựa vào `môi trường cụ thể` để đạt được `hiệu quả cao nhất.`
  - `Bản chất` của học tăng cường là trial-and-error, nghĩa là `thử đi thử lại và rút ra kinh nghiệm` sau mỗi lần thử như vậy. Đây là một nhánh học khá hấp dẫn trong máy học.
