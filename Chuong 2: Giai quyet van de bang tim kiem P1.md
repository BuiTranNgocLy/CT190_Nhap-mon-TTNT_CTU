## A. Biểu diễn bài toán trong Không gian trạng thái (KGTT)
### 1. Không gian trạng thái
- SỬ dụng KGTT để biểu diễn tri thức
- Biểu diễn KGTT: `Trạng thái` kết nối với nhau bằng các `hành động`
- KGTT bao gồm:
  - `N(node)`: tập các trạng thái
  - `S(start)`: Trạng thái ban đầu (# rỗng)
  - `GD (goal desciption)`: Trạng thái đích, bộ mô tả mục tiêu
  - `Op (Operation)`: toán tử biến đổi trạng thái
### 2. Biểu diễn bài toán trên KGTT (VD trò cờ caro)
- Cần xác định
  - Các trạng thái: mỗi lượt đi sẽ tạo nên 1 trạng thái mới
  - Các hành động: đi X hoặc O
  - Mục tiêu: dãy 3 ký hiệu giống nhau (ngang, dọc hoặc chéo)
  - Chi phí: 1 (mỗi lượt đi)
### 3. Giải quyết bài toán bằng tìm kiếm
- Bài toán đã được biểu diễn bằng KGTT => Tìm kiếm một đường đi lời giải/ một trạng thái đích mong ước
  - Đường đi lời giải (Solution path) Là đường đi trong đồ thị/cây trạng thái:  trạng thái bắt đầu -> trạng thái đích
  - Trạng thái đích mong ước: trạng thái cuối cùng thõa mãn mục tiêu yêu cầu
### 4. Giải pháp
- Biểu diễn bài toán trên KGTT để thực hiện tìm kiếm
- Các bước xầy dựng KGTT
  - Bắt đầu từ 1 trạng thái đã cho
  - Kiểm tra có phải trạng thái đích
  - Mỏ rộng 1 trong các trạng thái
  - Nếu có nhiều khả năng, chọn 1 khả năng nào đó
 - Tập trạng thái được mở rộng có nhiều lựa chọn, chọn  thái nào mở rộng -> chiến lược tìm kiếm
### 5. Các phương pháp tìm kiếm
- `Tìm kiếm mù (uninformed/blind search)`: *Trạng thái được chọn để phát triển chỉ dựa theo cấu trúc của KGTT mà không dùng thêm thông tin hỗ trợ.*
- `Tìm kiếm dựa trên kinh nghiệm (informed/ heuristic search)`: *Dựa vào kinh nghiệm và sự hiểu biết để xây dựng hàm đánh giá hướng dẫn tìm kiếm*

[Chương 2: Biểu diễn bài toán trong KGTT.pdf](https://github.com/BuiTranNgocLy/Nhap-mon-TTNT_CT190_CTU/files/7496829/Chuong2_Search_NMTTNT_2021_08_p1-trang-1-8.pdf)
