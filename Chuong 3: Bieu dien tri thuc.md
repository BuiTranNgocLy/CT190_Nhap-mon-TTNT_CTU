
# 1. Tại sao phải biểu diễn tri thức?
- Sử dụng ngôn ngữ BDTT & trao đổi tri thức
- Giữ vai trò quan trọng trong AI. SỬ dụng trong:
   - Biểu diễn bài toán
   - Tìm kiếm lời giải của bài toán
- Mục tiêu: máy tính có thể thao tác trên các tri thức được biểu diễn tìm lời giải bài toán
# 2. Tri thức là gì?
- Dữ kiện có nhờ `trải nghiệm` hay `thông qua học tập`
- `Sự hiểu biết`
- Chia thành 2 lớp
   - `Tri thức sự kiện` mô tả sự kiện trong thế giới
   - `Tri thức suy diễn` mô tả 'quy luật' mối quan hệ giữa các sự
  ![image](https://user-images.githubusercontent.com/88178841/141438484-85a91c3b-b3c7-4872-a13d-ffc9effa732c.png)

# 3. Biểu diễn ánh xạ
![image](https://user-images.githubusercontent.com/88178841/141438396-8d31a09e-069a-498c-b6d8-943f7b8da049.png)
# 4. Các phương pháp biểu diễn tri thức cơ bản
- `Mô hình logic`Logic based representation – first order predicate logic, Prolog
- `Mô hình thủ tục` Procedural representation – rules, production system
- `Mô hình mạng` Network representation – semantic networks, conceptual graphs
- `Mô hình cấu trúc` Structural representation – scripts, frames, objects 

# 5. Logic mệnh đề
- `Mệnh đề`: là một khẳng định có tính chất đúng (true) hoặc sai (false).
![image](https://user-images.githubusercontent.com/88178841/141440439-748316ec-b44b-428a-85e3-be8064717cdb.png)
- `Ngữ nghĩa của phép toán mệnh đề`được diễn giải bằng cách gán chân trị cho các mệnh đề (một ánh xạ từ các ký hiệu mệnh đề vào tập {T,F})
![image](https://user-images.githubusercontent.com/88178841/141441334-c6a76c91-34f7-4847-8b8e-e45e69435cdc.png)
- `Ngữ nghĩa của một biểu thức mệnh đề` là `giá trị` của biểu thức mệnh đề đó.
- `Giá trị của biểu thức mệnh đề` là có khả năng `tính toán được`
- Trong đó:
   - `Mỗi mệnh đề` được gán một giá trị True hay False.
   - Mỗi toán tử được đánh giá theo bảng chân trị và thứ tự ưu tiên của toán tử.
- `Mệnh đề tương đương`
![image](https://user-images.githubusercontent.com/88178841/141443175-67ae9ccb-2e08-41e3-8612-225f225b4550.png)
![image](https://user-images.githubusercontent.com/88178841/141443218-70ed791a-b593-4aac-874a-1811d07810a2.png)
![image](https://user-images.githubusercontent.com/88178841/141443259-2abbdc86-fb5b-4990-ac06-73ec0ca63477.png)
![image](https://user-images.githubusercontent.com/88178841/141443398-c9751954-70be-4748-9c10-4a6a74118f6d.png)
## Chứng minh logic
- `Chứng minh dựa trên bảng chân trị`
![image](https://user-images.githubusercontent.com/88178841/141443838-4b36601d-1764-4540-b571-93907b7ab8f2.png)
- `Chứng minh dựa trên các luật suy diễn`
![image](https://user-images.githubusercontent.com/88178841/141444074-69b60b8b-c033-4791-b06c-6dc85ae3eff3.png)
![image](https://user-images.githubusercontent.com/88178841/141444100-c74281ae-b799-4bed-8d13-edb549c6e43f.png)
![image](https://user-images.githubusercontent.com/88178841/141444118-4d4dd28b-46e7-4278-930c-fffe9205bb67.png)

- `Chứng minh bằng hợp giải`
   - `Hợp giải` là kỹ thuật lập luận dựa trên nguyên lý `chứng minh phản chứng`: để chứng minh một phát biểu, hợp giải chứng tỏ rằng phủ định của phát biểu đó làm phát sinh một mâu thuẫn với những phát biểu đã biết.
