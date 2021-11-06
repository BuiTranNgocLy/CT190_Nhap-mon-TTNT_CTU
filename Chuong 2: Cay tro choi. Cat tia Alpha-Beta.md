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
***All this text is important***
