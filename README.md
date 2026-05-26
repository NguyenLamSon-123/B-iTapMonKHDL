## Nguyễn Lam Sơn_K225480106076
[Bài Tập Khoa Học Dữ Liệu](https://www.youtube.com/watch?v=xpnhHjDMBHI)
# Bài Tập Môn Khoa Học Dữ Liệu
Phân Cụm Học Lực Sinh Viên
Lớp K58KTPM
Bài toán đặt ra là cần xử lý và phân tích dữ liệu từ bảng điểm tổng hợp của lớp K58KTPM. Thay vì chỉ dựa vào điểm số trung bình tĩnh, nghiên cứu này sử dụng cấu trúc điểm chi tiết của tất cả các môn học để tìm ra các nhóm sinh viên có đặc điểm và năng lực học tập tương đồng nhau.

# Mục tiêu cốt lõi:
ETL: Tự động hóa quá trình làm sạch dữ liệu từ file Excel thô.
Modeling: Sử dụng thuật toán AI để gom cụm (Clustering) khách quan.
Visualization: Trực quan hóa dữ liệu giúp giáo viên dễ dàng đưa ra quyết định hỗ trợ.

# 2. Quy trình Xử lý & Thuật toán
# Bước 1: Tiền xử lý dữ liệu (Data Preprocessing)
Đọc file Excel TỔNG HỢP ĐIỂM K58KTP.xlsx bằng thư viện pandas. Tự động tìm dòng header chứa thông tin sinh viên, chuẩn hóa định dạng điểm số (chuyển dấu phẩy thành dấu chấm) và xử lý các giá trị khuyết thiếu (NaN được lấp bằng 0).

# Bước 2: Thuật toán Hierarchical Clustering
Sử dụng phương pháp phân cụm phân cấp với thuật toán Ward Linkage. Phương pháp này tối thiểu hóa phương sai trong mỗi cụm, giúp tạo ra các cụm đồng nhất nhất có thể. Dựa trên biểu đồ Dendrogram, hệ thống xác định cắt tại ngưỡng tối ưu để chia lớp thành 3 nhóm.

# Bước 3: Xuất bản và Báo cáo (Export)
Dữ liệu sau khi dán nhãn được lưu vào file Excel mới gồm 3 sheets: Bảng dữ liệu đã phân nhóm, Biểu đồ trực quan nhúng sẵn, và Bảng thống kê tóm tắt.

# 3. Trực quan hóa Kết quả
## Sơ đồ Cây Phân Cấp (Dendrogram)
# <img width="957" height="558" alt="image" src="https://github.com/user-attachments/assets/b4c923cd-65db-4da8-b8f2-2941be387fad" />
## Mật độ Phân bố Điểm số (Density Plot)
# <img width="958" height="593" alt="image" src="https://github.com/user-attachments/assets/a5de1402-5210-440d-8629-9408b4153154" />
## Biến thiên Điểm Chi tiết (Violin & Strip Plot)
# <img width="957" height="510" alt="image" src="https://github.com/user-attachments/assets/b3a3751a-7366-4f4b-bcee-aac77c870f1a" />
## Cơ cấu Nhóm Học lực (Donut Chart)
## <img width="962" height="918" alt="image" src="https://github.com/user-attachments/assets/9e608114-589b-4e2c-a343-f6c59517f42b" />
# 4. Bảng Số liệu Thống kê
# <img width="993" height="415" alt="image" src="https://github.com/user-attachments/assets/1b378ffe-05ef-479a-9185-8e3f1dcafe92" />
