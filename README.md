# Nhóm 14 - Phân tích dữ liệu thị trường chứng khoán sử dụng mô hình hồi quy tuyến tính

## Mô tả

`yfin14.py` là một công cụ phân tích chứng khoán sử dụng Streamlit để hiển thị biểu đồ giá, truy xuất dữ liệu lịch sử và dự báo giá cổ phiếu. Đây là một phần của hệ thống tổng thể phân tích tài chính nhằm cung cấp cho người dùng các công cụ để theo dõi và dự đoán xu hướng giá của một số công ty lớn trên thị trường.

## Tính năng

- **Hiển thị Biểu đồ Giá**: Sử dụng Plotly để hiển thị biểu đồ giá theo ngày cho các mã cổ phiếu được chọn.
- **Dữ liệu Lịch sử**: Truy xuất và tải dữ liệu lịch sử từ Yahoo Finance.
- **Dự báo Giá Cổ Phiếu**: Sử dụng mô hình học máy đã được huấn luyện để dự đoán giá cổ phiếu cho các mã công ty như AAPL, AMZN, META, GOOGL, và MSFT.
- **Chuẩn hóa Dữ liệu**: Sử dụng mô hình chuẩn hóa đã được huấn luyện để xử lý dữ liệu đầu vào trước khi dự báo.

## Yêu cầu

- Python 3.6+
- Streamlit
- Plotly
- Pandas
- Pickle
- Matplotlib

Cài đặt các gói yêu cầu có thể được thực hiện thông qua pip:

```bash
pip install streamlit plotly pandas matplotlib pickle5
```

## Cách Sử Dụng

1. **Khởi chạy Ứng dụng**: Chạy script Python bằng cách sử dụng lệnh sau:
   
   ```bash
   streamlit run yfin14.py
   ```

2. **Chọn Mã Cổ Phiếu**: Sử dụng menu dropdown để chọn mã cổ phiếu bạn muốn phân tích.

3. **Nhập Dữ liệu Giao dịch**: Nhập các giá trị mở, cao, thấp, và đóng trong sidebar như được hướng dẫn.

4. **Xem Thông Tin Mô Hình Huấn Luyện**: Bấm nút để xem thông tin về mô hình huấn luyện liên quan đến mã cổ phiếu đã chọn.

5. **Dự báo Giá Cổ Phiếu**: Sử dụng nút "Dự báo" để thực hiện dự báo giá và xem kết quả.

6. **Xem Biểu đồ Dự báo**: Thấy biểu đồ của các lần dự báo trước đó sau khi nhấn "Dự báo" nhiều lần.

7. **Reset Ứng dụng**: Sử dụng nút 'Reset' để xóa tất cả thông tin và đặt lại các giá trị mặc định.

## Nội dung File

- `yfin14.py`: Script chính cho ứng dụng Streamlit.
- `Model_data/` & `Scaler_data/`: Thư mục chứa các mô hình huấn luyện và tham số chuẩn hóa cho từng mã cổ phiếu.
