# Datathon 2026: The Gridbreakers - Sales Forecasting Pipeline
**Team:** OkChokChok | **Round:** 1

## 1. Overview
Repository này lưu trữ toàn bộ mã nguồn và quy trình xử lý dữ liệu (End-to-end Data Pipeline) của đội OkChokChok tham gia cuộc thi Datathon 2026. 

Dự án tập trung vào việc khai phá dữ liệu (EDA), đánh giá danh mục sản phẩm/khuyến mãi và xây dựng mô hình Machine Learning nhằm dự báo doanh thu, giải quyết các bài toán về tối ưu phân bổ tồn kho.

## 2. Repository Structure
Hệ thống mã nguồn được phân tách thành các module độc lập:
```text
Datathon2026_OkChokChok/
├── notebooks/
│   ├── 01_MCQ_Answers.ipynb                # Truy xuất dữ liệu giải quyết 10 câu hỏi nghiệp vụ
│   ├── 02_EDA_and_Feature_Engineering.ipynb # Phân tích xu hướng (Seasonality) & Promotion ROI
│   └── 03_Master_Pipeline_and_Forecasting.ipynb # Trích xuất đặc trưng, huấn luyện mô hình & xuất kết quả
├── submission/
│   └── submission.csv                      # File kết quả dự đoán cuối cùng
├── .gitignore                              # Cấu hình bỏ qua dữ liệu thô (*.csv)
└── README.md                               # Tài liệu hướng dẫn dự án
```
*Ghi chú: Báo cáo kỹ thuật chi tiết (Technical Report PDF) được đính kèm và nộp thông qua hệ thống của Ban tổ chức.*

## 3. Reproducibility
Để đảm bảo tính tái lập (Reproducibility) và tránh xung đột môi trường (Dependency Conflicts) trên máy tính cá nhân, pipeline được thiết lập để thực thi trực tiếp trên nền tảng Kaggle.

**Các bước thực thi:**
1. Truy cập trang chủ cuộc thi: [Datathon 2026 - Round 1](https://www.kaggle.com/competitions/datathon-2026-round-1).
2. Chuyển hướng sang tab **Code** và chọn **New Notebook**.
3. Chọn **File -> Import Notebook** để tải lên lần lượt các file `.ipynb` từ thư mục `notebooks/` của repository này.
4. Đảm bảo bộ dữ liệu chính thức của cuộc thi đã được thêm (Add Data) vào môi trường làm việc của Notebook.
5. Chọn **Run All**. Mã nguồn sẽ tự động nhận diện thư mục `/kaggle/input/`, tiến hành tiền xử lý, huấn luyện mô hình và xuất file `submission.csv`.
