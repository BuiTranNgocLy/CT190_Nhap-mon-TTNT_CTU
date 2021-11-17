# I. Ứng dụng Heuristic trong các trò chơi
* Sử dụng không gian trạng thái để giải quyết bài toán
* Tìm kiếm mù
* Tìm kiếm heuristic – có thông tin bổ sung
* Sử dụng heuristic cho trò chơi
* Có 2 người tham gia
* Bạn tạo ra trạng thái này, `đối thủ tạo trạng thái đánh bại bạn`

# II. GIải thuật Mini_Max
## 1. Chi tiết MiniMax
* 1 đối thủ là `MIN`: người chơi cố gắng cho MAX giành điểm thấp
* Đối thủ còn lại `MAX`: người chơi luôn muốn thắng
* Giá trị nút lá
  * `1` : MAX thắng
  * `0` : MIN thắng (MAX thua)
* MiniMax truyền các giá trị lên cao dần trên đồ thị, qua các nút cha kế tiếp theo luật:
  * `Trạng thái cha là MAX`: gán nó giá trị `lớn nhất` có trong các trạng thái con
  * `Trạng thái cha là MIN`: gán nó giá trị `nhỏ nhất` có trong các trạng thái con
## 2. Minimax với độ sâu lớp cố định
* Trò chơi phức tạp -> KGTT không đến các nút lá
* KGTT triển khai -> 1 mức xác định => Tính n bước đi
* Các nút lá của đồ thị con không phải Goal kết thúc => Không xác định giá trị Thắng-thua
* `Cần hàm đánh giá Heuristic nào đó`
* Giá trị nút lá là các giá trị Heuristic đạt được sau n bước đi kể từ nút xuất phát
* Giá trị này truyền ngược về nút gốc => Giá trị trạng thái tốt nhất
***Hàm Heuristic***
* `E(n) = M(n) – O(n)`
  * M(n) là tổng số đường thắng có thể của tôi
  * O(n) là tổng số đường thắng có thể của đối thủ
  * E(n) là trị số đánh giá tổng cộng cho trạng thái n

[Ví dụ Bài toán lá bài.pdf](https://github.com/BuiTranNgocLy/Nhap-mon-TTNT_CT190_CTU/files/7490848/Bai.toan.la.bai.pdf)

# III. Cắt tỉa Alpha-Beta
* Tìm kiếm alpha – beta thực hiện theo kiểu tìm kiếm sâu.
* Cắt tỉa Alpha - Beta
  * `Alpha` gắn vơi các nút `MAX`, không giảm
  * `Beta` gắn với các nút `MIN`, không tăng
* Luật cắt tỉa
* `Alpha cut` nút MIN có Beta `<=` nút cha MAX alpha bất kỳ
* `Beta cut` nút MAX có alpha `>=` nút cha MIN beta bất kỳ 

![image](https://user-images.githubusercontent.com/88178841/140618045-37c0d3b8-c456-413d-8d29-22ce431394c2.png)
![image](https://user-images.githubusercontent.com/88178841/140618098-5276ac4f-910d-46b9-9133-ca06e10daf60.png)

# IV. Bài toán thỏa mãn ràng buộc - Constraint satisfaction problem
* Sử dụng phương pháp `biểu diễn có cấu trúc` để biểu diễn các trạng thái, `mỗi trạng thái là một tập biến`, `mỗi biến có một giá trị`
* Bài toán được giải quyết khi mỗi biến đều được gán trị thỏa
mãn tất cả ràng buộc
* 1 bài toán gồm 3 thành phần:
  * ***X: tập hợp các biến {X1, X2 , … , Xn }***
  * ***D: tập hợp các miền giá trị {D1, D2, … , Dn}, Di = {v1, v2,...,vk} gán vào biến Xi tương ứng***
  * ***C: tập hợp các ràng buộc, `<scope, rel>` scope là
một bộ biến tham gia vào quan hệ rel***
* Cách giải quyết bài toán:
  * Dùng các ràng buộc để giảm số giá trị hợp lệ cho một biến
  * các giá trị này lại có thể làm giảm các giá trị hợp lệ cho biến
khác…
* Ý tưởng:
  * Mỗi biến là một nút trong đồ thị
  * Mỗi ràng buộc nhị phân (trên 2 biến) như một cung
  * 
![image](https://user-images.githubusercontent.com/88178841/140619038-fb752f03-545e-4a49-bb77-3f028316da17.png) ![image](https://user-images.githubusercontent.com/88178841/140619053-3a707251-253a-4fe5-863f-948d9feb0e5b.png)

<hr>

**Author Bui Tran Ngoc Ly**  
  
  
