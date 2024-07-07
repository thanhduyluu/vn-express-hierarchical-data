# Báo cáo Khoa học về Dataset từ VnExpress

## 1. Giới thiệu
Dataset được thu thập từ trang báo điện tử VnExpress, 
một trong những trang báo phổ biến nhất tại Việt Nam.
Dữ liệu bao gồm nhiều lĩnh vực khác nhau với số lượng mẫu lớn,
được chia thành các nhãn chính và nhãn phụ. Dữ liệu có cấu trúc phân cấp với
hai cấp độ nhãn. Dữ liệu được loại bỏ các dòng bị trùng lặp và được lưu trữ dưới dạng CSV.
Quá trình làm sạch dữ liệu bao gồm loại bỏ các dòng bị trùng lặp, loại bỏ các 
nhãn có số lượng mẫu quá ít (Dưới 200 mẩu) và chuyển đổi dữ liệu về dạng chuẩn.

Phân bố dữ liệu trước và sau khi làm sạch được thể hiện qua các biểu đồ sau:
- Dữ liệu thô: [tại đây](./docs/raw/README.md)
- Dữ liệu đã làm sạch: [tại đây](./docs/clean/README.md)

## 2. Thông tin Tổng quan về Dataset
### 2.1. Dataset trước khi làm sạch ([data-vn-express.clean.csv](./data-vn-express.clean.csv))
- **Tổng số mẫu**: 47,772
- **Số lượng nhãn chính**: 22
- **Số lượng nhãn phụ**: 108

### 2.2. Dataset sau khi làm sạch ([data-vn-express.raw.csv](./data-vn-express.raw.csv))
- **Tổng số mẫu**: 46,412
- **Số lượng nhãn chính**: 21
- **Số lượng nhãn phụ**: 95

## 3. Phân phối Dữ liệu
### 3.1. Phân phối theo Nhãn Chính
Dưới đây là phân phối của một số nhãn chính trong dataset:

| Nhãn Chính       | Trước Làm Sạch | Sau Làm Sạch |
|------------------|----------------|--------------|
| Giải trí         | 4,184          | 4,184        |
| Góc nhìn         | 3,699          | 3,699        |
| Du lịch          | 2,299          | 2,279        |
| Giáo dục         | 3,671          | 3,512        |
| Khoa học         | 3,264          | 3,262        |
| Sức khoẻ         | 3,599          | 3,599        |
| Kinh doanh       | 4,743          | 4,743        |
| Thể thao         | 2,742          | 2,696        |
| Thời sự          | 3,016          | 3,000        |
| Pháp luật        | 1,205          | 1,200        |
| Số hoá           | 2,259          | 2,259        |
| Podcast          | 2,178          | 1,179        |
| Bất động sản     | 113            | Không còn    |

### 3.2. Phân phối theo Nhãn Phụ
Mỗi nhãn chính được chia thành nhiều nhãn phụ. Dưới đây là phân phối của một số nhãn phụ trong các nhãn chính:

**Giải trí:**
- Sân khấu - Mỹ thuật: 600
- Thời trang: 600
- Giới sao: 598
- Sách: 587
- Làm đẹp: 600
- Nhạc: 600
- Phim: 599

**Giáo dục:**
- Giáo dục 4.0: 600
- Chân dung: 523
- Tin tức: 600
- Du học: 600
- Tuyển sinh: 589
- Học tiếng Anh: 600

**Sức khoẻ:**
- Các bệnh: 600
- Tư vấn: 600
- Tin tức: 599
- Đàn ông: 600
- Dinh dưỡng: 600
- Khỏe đẹp: 600

## 4. Chất lượng Dữ liệu
- **Trước làm sạch**: Tổng số mẫu là 47,772. Dữ liệu chứa một số dòng bị trùng lặp.
- **Sau làm sạch**: Tổng số mẫu giảm xuống còn 46,412. Các dòng bị trùng lặp đã được loại bỏ, giúp cải thiện chất lượng dữ liệu.

## 5. Phân tích và Đánh giá
### 5.1. Sự Đa dạng và Phân phối Dữ liệu
- Dataset bao gồm nhiều lĩnh vực khác nhau, từ giải trí, giáo dục, khoa học đến sức khoẻ, kinh doanh và thể thao.
- Phân phối dữ liệu khá đồng đều giữa các nhãn chính, với một số nhãn như giải trí và kinh doanh có số lượng mẫu cao.

### 5.2. Chất lượng Dữ liệu Sau Khi Làm Sạch
- Việc loại bỏ các dòng bị trùng lặp đã giúp giảm tổng số mẫu từ 47,772 xuống còn 46,412, cho thấy rằng quá trình thu thập dữ liệu ban đầu đã có một số dòng bị trùng lặp.
- Chất lượng dữ liệu được cải thiện, giúp tăng độ tin cậy cho các phân tích và mô hình học máy.

---
