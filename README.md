# CoSoDuLieu
PASSWORD: is.fit.hcmus.vn

THI LÝ THUYẾT
  1/ ER --> MH Quan hệ
    Tập thực thể sang quan hệ
    Tập mối kết hợp 2 ngôi sang quan hệ
    Tập mối kết hợp có 2 chỉ số max trên 2 bản số tương ứng là 1-n
    Tập mối kết hợp có 2 chỉ số max trên 2 bản số tương ứng là n-m
    Tập thực thể yếu sang quan hệ
    Thuộc tính đa trị
  2/ MH Quan hệ: 
    2 Ngôn ngữ Đại số quan hệ 
        + Phép gán (<-), phép chọn (Sigma), phép chiếu (Pi), phép đổi tên (Rho)
        + Phép giao INTERSECT (U), phép hội UNION (V), phép trừ EXTRACT (-) (Điều kiện để thực hiện được các phép toán này: khả hợp). Kết quả thu được là thuộc tính của quan hệ bên trái
            Khả hợp: 2 quan hệ cùng bậc ( cùng số lượng thuộc tính)
                    Các thuộc tính cùng kiểu dữ liệu tương ứng
        + Phép nhân (x) (Thuộc tính bằng tổng thuộc tính 2 quan hệ, dữ liệu = nhân ma trận)
        + Phép kết JOIN
            Phép kết bằng (
            Phép kết tự nhiên (2 thuộc tính để kết hợp phải giống tên nhau)
            Phép kết ngoài, kết trong, kết 2 bên
            Phép kết 1 nửa
            Phép gom nhóm (Tau) + hàm tính toán (Count, Max, Min, Sum, Avg)
    2 Phép tính quan hệ
      Biến là bộ, cú pháp {t | P(t)}
    1 Ràng buộc toàn vẹn

THI THỰC HÀNH 
45-60 phút
  0/ Cho CSDL Script --> Tạo CSDL
  1/ Viết câu truy vấn cho các yêu cầu: 4-5 câu
    Chỉ viết 1 câu SQL (Cho phép viết SQL lồng, (cấm Select,From)), (cho phép where,having))
      New query --> Save as Encoding UTF-8
      -- Comment : Ghi lại thông tin MSSV, Tên, câu hỏi đề bài
      -- Phân tích đề bài, kết quả, điều kiện, quan hệ
      Ngôn ngữ SQL:
        Select (Pi)
        From (Bảng quan hệ) (Ex: From sinhvien s inner join lophoc l on (s.hoclop = l.malop)
        Where (Sigma) (Ex: like N'L%')
        Group by (Tau)
        Having
        Order by;
  2/ Kết nối vào server
   user: sa
   password: svcntt
 Lưu *.sql
Note: Fk should be "allow NULLs"

Tools --> Options --> Designers --> Prevent saving changes that require table re-creation
Condition: Right click --> Check constraint --> Identity: Name , Expression: SLTon >= 0, and, or

Note: Cách lưu:
.SQL			:	Right click --> Task --> Generate scripts --> Advanced: Types of data to script: Schema and data --> Save as .sql Encoding-UTF8
.MDF and .LDF	: 	Right click --> Task --> Detach, check: Drop and Update	--> Save to another folder
