
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

# 5. Biểu diễn Logic
## Logic mệnh đề
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
### Chứng minh dựa trên bảng chân trị

![image](https://user-images.githubusercontent.com/88178841/141443838-4b36601d-1764-4540-b571-93907b7ab8f2.png)
### Chứng minh dựa trên các luật suy diễn

![image](https://user-images.githubusercontent.com/88178841/141444074-69b60b8b-c033-4791-b06c-6dc85ae3eff3.png)
![image](https://user-images.githubusercontent.com/88178841/141444100-c74281ae-b799-4bed-8d13-edb549c6e43f.png)
![image](https://user-images.githubusercontent.com/88178841/141444118-4d4dd28b-46e7-4278-930c-fffe9205bb67.png)

### Chứng minh bằng hợp giải
#### Cơ sở của Hợp giải
   - `Hợp giải` là kỹ thuật lập luận dựa trên nguyên lý `chứng minh phản chứng`: để chứng minh một phát biểu, hợp giải chứng tỏ rằng phủ định của phát biểu đó làm phát sinh một mâu thuẫn với những phát biểu đã biết.
   - Các mệnh đề phải ở `dạng chuẩn CNF`
#### Dạng chuẩn CNF & DNF
- `Tuyển cơ bản` : `DNF` *là thành phần cơ bản hay sự kết hợp của các thành phần cơ bản bằng phép tuyển(v)* 
- `Hội cơ bản` : `CNF` *là thành phần cơ bản hay sự kết hợp của các thành phần cơ bản bằng phép hội (^)*
##### Dạng chuẩn hội CNF
- `Hội cơ bản` A^B
- `Một biểu thức tuyển cơ bản`¬(BvC)
- `Hội của các tuyển cơ bản.` (AvB)^(¬BvCv¬D)^(Dv¬E)
- ![image](https://user-images.githubusercontent.com/88178841/141481631-5d4627a9-8cdd-4e7a-8b92-14961e832f77.png)

##### Giải thuật hợp giải cho Logic mệnh đề
- `Áp dụng  biểu thức logic ở dạng chuẩn CNF`
- ![image](https://user-images.githubusercontent.com/88178841/141487172-e6a2886d-e2da-4910-a67f-e4b9e8a4eccb.png)

VÍ DỤ

![image](https://user-images.githubusercontent.com/88178841/141487414-0914ca9a-df13-4dc2-8610-00abe045f342.png)

![image](https://user-images.githubusercontent.com/88178841/141487452-745c4221-bdc3-4351-af0c-c37acb163577.png)

![image](https://user-images.githubusercontent.com/88178841/141487470-450707f3-f638-457d-9519-4bd09613f15c.png)

# 6. Biểu diễn thủ tục (Procedural representation)
## a. Biểu diễn thủ tục
- Sử dụng tri thức thủ tục để biểu diễn tri thức:
    - Biểu diễn tri thức như `tập các chỉ thị lệnh` để giải quyết vấn đề
    - `Các chỉ thị lệnh` trong lược đồ thủ tục chỉ ra `bằng cách nào giải quyết vấn đề.`
- Tri thức thủ tục `mô tả làm thế nào để thực hiện 1 tác vụ`
    - Tập trung vào các nhiệm vụ cần thực hiện để đạt được 1 mục tiêu cụ thể.
    - Gồm 1 `tập các chỉ thị lệnh` để giải quyết.
- Ví dụ điển hình: `Hệ luật sinh`.
## b. Hệ luật sinh
- `Biểu diễn tri thức` dưới dạng `các luật`, tư vấn những `điều nên làm` hoặc đưa ra `kết luận những tình huống cụ thể.`
- Gồm 1 tập các luật `IF - THEN` chứa cặp `<condition , action>`, mô tả các sự kiện & trình biên dịch, điều khiển việc áp dụng các luật & các sự kiện được cho.
- Sử dụng `luật suy diễn tiến` ( dữ liệu -> mục tiêu ) ; `luật suy diễn lùi` ( mục tiêu về dữ liệu )
- VD:

![image](https://user-images.githubusercontent.com/88178841/144354380-7c7f04e5-b042-4023-9e02-f28103f0bed9.png)

# 7. Biểu diễn mạng (Network representation)
## a. Biểu diển mạng
- Tri thức biểu diễn dưới `dạng đồ thị`:
    - `Đỉnh`: các `đối tượng` hoặc `khái niệm`
    - `Các cung`: quan hệ giữa chúng
- Ví dụ về lược đồ này: mạng ngữ nghĩa, phụ thuộc khái niệm, đồ thị khái niệm,...
## b. Biểu diễn tri thức mạng ngữ nghĩa
- `Định nghĩa`: Là lược đồ biểu diễn kiểu mạng, dùng `đồ thị` biểu diễn tri thức:
    - `Các đỉnh`: biểu diễn cád đố tượng
    - `Các cung`: biểu diễn quan hệ giữa  
- Ví dụ:

![image](https://user-images.githubusercontent.com/88178841/144355028-217991f8-f3a0-4aff-8c81-330fbc7b29ee.png)

# 8. Biểu diễn cấu trúc (Structural representation)
- `Là 1 mở rộng của lược đồ mạng`: bằng cách cho phép `các Node` có thể là `1 CTDL phức tạp` gồm các khe (slot) có tên và giá trị hay 1 thủ tục.
- Tích hợp cả dạng `khai báo & thủ tục`
- Ví dụ về lược đồ này: Khung(frame), đối tượng(Object)
## Biểu diễn tri thức bằng frame

![image](https://user-images.githubusercontent.com/88178841/144435759-c9b2bd4d-85e0-4b31-8203-340e268de6e7.png)

- `Frame-khung`: là 1 `cấu trúc dữ liệu` chứa tất cả tri thức về 1 đối tượng cụ thể. Là cấu trúc `dạng hướng đối tượng trong AI` và các hệ chuyên gia.
- Cấu trúc của Frame:
    - `Frame name`: tên cá thể; tên lớp
    - `Class`:  cho biết Frame đang biểu diễn có trường Class -> `cho phép thành lập quan hệ thừa kế`
    - `Các thuộc tính (Property)`: khi biểu diễn 1 Frame có thể thiết lập 1 hay nhiều thuộc tính cho nó.

![image](https://user-images.githubusercontent.com/88178841/144437219-8fcba02c-79da-4d60-8cc1-40daa4dfd2a8.png)
![image](https://user-images.githubusercontent.com/88178841/144437267-98ed1fae-cf64-4485-a920-de6813b0e177.png)



<hr>

**Author Bui Tran Ngoc Ly**
