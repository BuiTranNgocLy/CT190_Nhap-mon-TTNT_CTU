# I. Heuristic là gì?
* Giải quyết các bài toán lớn, phải cung cấp những `kiến thức đặc trưng ở từng lĩnh vực để nâng cao` hiệu quả của việc tìm kiếm
* Trong TK KGTT, heuristic là các luật dùng để `chọn những nhánh/ lựa chọn nào có nhiều khả năng nhất` dẫn đến một giải pháp chấp nhận được
# II. Chi tết về hàm Heuristic
## 1. Thuận toán Heuristic (2 phần)
### a. Phép đo Heuristic
* Thể hiện qua hàm đánh giá heuristic, dùng để đánh giá các đặc điểm của một trạng thái trong KGTT.
* *Ước lượng chi phí tối ưu giữa hai hoặc nhiều giải pháp*
* *Không quá tốn kém để tính toán*
* `Được xác định cụ thể trong từng bài toán`
### b. Giải thuật tìm kiếm
* Tìm kiếm tốt nhất đầu tiên (Best-first-search)
  * `Tìm kiếm háu ăn (greedy best-first search)`
  * `Giải thuật A*`
* Giải thuật leo đồi
## 2. Hàm đánh giá Heurstic
* `f(n) = g(n) + h(n)`
  *  g(n): khoảng cách thực sự từ `n đến trạng thái Start`
  *  h(n): ước lượng heuristic cho khoảng cách từ trạng thái `n đến trạng thái`
 # III. Tìm kiếm tốt nhất đầu tiên (Best-first-search)
 *  Là tiếp cận tổng quát của tìm kiếm với thông tin bổ sung.
 *  Chọn nút để triển khai dựa trên một `hàm lượng giá f(n)`. Dựa trên việc ước lượng `chi phí và nút có giá ước lượng nhỏ nhất` được ưu tiên `triển khai trước.`
 *  `Hàm h(n)` là chi phí ước lượng của `đường đi tốt nhất` từ trạng thái của nút -> trạng thái mục tiêu.
    * `f(n) = g(n) +h(n)`
    * `g(n)`: chi phí thực tế đi từ `gốc đến n`
    * `h(n)`: chi phí ước lượng đi từ `n đến nút mục tiêu`
 * `nút mục tiêu thì h(n) = 0.` 
 ## Chi tiết giải thuật:
 * Dùng mảng có sắp xếp theo hàm đánh giá
 * Dùng các danh sách để lưu trữ các trạng thái:
   * `OPEN`: lưu các trạng thái `sắp được kiểm tra`
   * `CLOSED`: lưu các trạng thái `đã duyệt qua`
 * OPEN list sẽ được sắp xếp theo thứ tự dựa trên 1 hàm Heuristic (ưu tiên cho các giá trị gần trạng thái đích)
 * Mỗi lần lặp sẽ xem xét trạng thái tiềm năng nhất trong OPEN list
