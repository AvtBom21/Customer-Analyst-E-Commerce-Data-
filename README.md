# 🛍️ Customer Analyst - E-Commerce Data

Phân tích hành vi khách hàng từ dữ liệu giao dịch thương mại điện tử để khám phá những thông tin quan trọng phục vụ cho hoạt động tiếp thị, phân khúc khách hàng và tối ưu hóa doanh thu.

---

## 📊 Mục tiêu dự án

- Phân tích dữ liệu mua hàng để xác định các phân khúc khách hàng (Customer Segmentation).
- Khám phá các yếu tố ảnh hưởng đến hành vi mua hàng.
- Đưa ra gợi ý chiến lược marketing phù hợp theo từng nhóm khách hàng.

---

## 📁 Cấu trúc thư mục

| Tên file                  | Mô tả                                                                 |
|--------------------------|------------------------------------------------------------------------|
| `data.csv`               | Dữ liệu gốc gồm các giao dịch thương mại điện tử                      |
| `Data_PreProcessing.csv` | Dữ liệu đã qua xử lý, sẵn sàng cho phân tích                         |
| `PreProcessing.ipynb`    | Notebook xử lý dữ liệu: làm sạch, định dạng, trích xuất thông tin     |
| `Visual_data.pbix`       | File Power BI: trực quan hóa dữ liệu và biểu đồ phân tích            |

---

## 📈 Dữ liệu sử dụng

- **Nguồn:** Dữ liệu bán hàng E-Commerce (giả lập hoặc thực tế tuỳ theo bạn).
- **Các trường chính:**
  - `InvoiceNo`, `StockCode`, `Description`
  - `Quantity`, `InvoiceDate`, `UnitPrice`
  - `CustomerID`, `Country`

---

## 🔍 Quy trình xử lý & phân tích

1. **Tiền xử lý dữ liệu** với Python:
   - Làm sạch dữ liệu trùng, null, lỗi định dạng
   - Tạo cột `TotalPrice = Quantity * UnitPrice`
   - Phân loại khách hàng theo quốc gia, tần suất mua

2. **Phân tích & trực quan hóa** với Power BI:
   - Tổng doanh thu theo tháng/quốc gia
   - Nhóm khách hàng theo RFM (Recency - Frequency - Monetary)
   - Biểu đồ heatmap, bar chart, pie chart

3. **Phân khúc khách hàng (Segmentation)**:
   - Sử dụng phương pháp KMeans / RFM Analysis
   - Gợi ý chiến lược phù hợp từng nhóm

---

## 🛠️ Công cụ & công nghệ

- `Python`: Tiền xử lý dữ liệu (pandas, numpy)
- `Jupyter Notebook`: Lưu quá trình xử lý
- `Power BI`: Trực quan hóa dữ liệu & Dashboard
- `Git`: Quản lý phiên bản

---

## 🚀 Cách sử dụng dự án

1. Clone repo:
   ```bash
   git clone https://github.com/AvtBom21/Customer-Analyst-E-Commerce-Data-.git
