# Datathon 2026 - Round 1: The Gridbreakers 🚀
**Team:** NewtonMethod (VNU-UET)
**Competition:** Datathon 2026 - Hosted by Vin Telligence & VinUni DS&AI Club

## 👥 Đội ngũ NewtonMethod
* **Phạm Thành Trung** 
* **Phương Mai Anh**
* **Nguyễn Trung Đức Dũng**

## 💡 Tổng quan Dự án (Project Overview)
Dự án này giải quyết trọn vẹn bài toán vận hành của một doanh nghiệp thương mại điện tử thời trang thông qua 3 phần chính:
1. **Phân tích Tổng quan (MCQ):** Giải mã các chỉ số kinh doanh cốt lõi.
2. **Khai phá Dữ liệu (EDA & Data Storytelling):** Đưa ra góc nhìn Prescriptive (Tái cấu trúc vận hành) nhằm tối ưu hóa dòng tiền, vạch trần nghịch lý khuyến mãi và lỗ hổng logistics.
3. **Mô hình Dự báo (Sales Forecasting):** Xây dựng pipeline LightGBM với cơ chế học đặc trưng (Feature Re-calibration) thông qua độ trễ lưu lượng truy cập (Web Traffic Lags) để dự báo chính xác Revenue và COGS.


## ⚙️ Hướng dẫn Cài đặt và Chạy mã nguồn (Reproducibility)

Để Ban giám khảo có thể đánh giá và kiểm chứng toàn bộ pipeline phân tích cũng như mô hình dự báo của đội NewtonMethod một cách trơn tru nhất, vui lòng thực hiện theo các bước dưới đây.

### 1. Yêu cầu hệ thống (Prerequisites)
* Python 3.9 trở lên.
* Jupyter Notebook hoặc Jupyter Lab.

### 2. Thiết lập môi trường (Environment Setup)
Chúng tôi khuyến nghị chạy dự án trong môi trường ảo (Virtual Environment) để đảm bảo các phiên bản thư viện hoạt động chính xác. Mở Terminal/Command Prompt và chạy lần lượt các lệnh sau:

# Clone repository về máy local
git clone [https://github.com/Trunglizabeth/Vin_AI_data_competitions_NewtonMethod](https://github.com/Trunglizabeth/Vin_AI_data_competitions_NewtonMethod.git)
cd Vin_AI_data_competitions_NewtonMethod

# Tạo môi trường ảo (đặt tên là .venv)
python -m venv .venv

# Kích hoạt môi trường ảo
# -> Đối với Windows:
.venv\Scripts\activate
# -> Đối với macOS/Linux:
source .venv/bin/activate

# Cài đặt toàn bộ thư viện phụ thuộc
pip install -r requirements.txt
## 📁 Cấu trúc Thư mục (Repository Structure)
Dự án được tổ chức theo chuẩn Data Science Workspace:
```text
Vin_AI_data_competitions_NewtonMethod/
│
├── data/
│   ├── raw/               <- Chứa dữ liệu gốc tải từ BTC
│   └── processed/         <- Dữ liệu đã qua làm sạch và xử lý
│
├── figures/               <- Nơi lưu trữ các biểu đồ EDA (.png, .pdf) đưa vào Report
│
├── notebooks/
│   ├── Part 1 - Multiple Choice.ipynb    <- Code giải quyết bộ câu hỏi trắc nghiệm
│   ├── Part 2 - EDA.ipynb                <- Dashboard trực quan hóa và phân tích giả thuyết
│   ├── DataCleaning.ipynb                <- Tiền xử lý, merge bảng và chuẩn bị đặc trưng
│   └── baseline.ipynb                    <- Mô hình LightGBM dự báo Revenue & COGS
│
├── reports/
│   └── Report_NewtonMethod_Datathon.pdf  <- Báo cáo kỹ thuật định dạng NeurIPS
│
├── .gitignore
├── README.md              <- Tài liệu bạn đang đọc
└── requirements.txt       <- Danh sách các thư viện Python phụ thuộc



