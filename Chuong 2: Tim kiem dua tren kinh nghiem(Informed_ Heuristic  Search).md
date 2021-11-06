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
