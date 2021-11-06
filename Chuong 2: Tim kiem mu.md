# 1. Tìm kiếm rộng (Breath-first-search)
* [Giải thuật & Ví dụ.pdf](https://github.com/BuiTranNgocLy/Nhap-mon-TTNT_CT190_CTU/files/7489751/BFS.pdf)
# 2. Tìm kiếm sâu (Depth-first-search)
* [Giải thuật & Ví dụ.pdf](https://github.com/BuiTranNgocLy/Nhap-mon-TTNT_CT190_CTU/files/7489752/Tim.ki.m.sau-DFS.pdf)
# 3. Tìm kiếm theo độ sâu có giới hạn (depth-limited search)
* Tương tự như tìm kiếm theo độ sâu, tuy nhiên chỉ tìm đến một `độ sâu d` nhất định nào đó
# 4.Tìm kiếm theo chiều sâu lặp (iterative deepening depth-first search)
* Tương tự như tìm kiếm theo độ sâu, tuy nhiên lặp lại việc tìm kiếm với `độ sâu giới hạn được tăng dần` cho đến khi tìm được trạng thái đích
* `Nút gốc có độ sâu = 0`
# 5. Tìm kiếm giá thành đồng nhất (Uniform-cost search)
* Tìm kiếm theo chiều rộng
  * Đảm bảo tìm ra giải pháp cho bài toán
  * Không chắc tìm ra đường đi chi phí thấp nhất
* Tìm kiếm giá thành đồng nhất (rất giống GT Dijsktra)
  * `Chọn nút` có giá thành `đường đi đến nó thấp nhất mà triển khai`
  * Đảm bảo tìm được giải pháp với chi phí thấp nhất nếu biết rằng chi phí tăng khi chiều dài đường đi tăng
  * Tối ưu và đầy đủ
  * Nhưng có thể rất chậm


[BFS.pdf](https://github.com/BuiTranNgocLy/Nhap-mon-TTNT_CT190_CTU/files/7489778/BFS.pdf)
