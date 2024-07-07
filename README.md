# Báo cáo Khoa học về Dataset từ VnExpress

## 1. Giới thiệu

Dataset được thu thập từ trang báo điện tử VnExpress,
một trong những trang báo phổ biến nhất tại Việt Nam.
Dữ liệu bao gồm nhiều lĩnh vực khác nhau với số lượng mẫu lớn,
được chia thành các nhãn chính và nhãn phụ. Dữ liệu có cấu trúc phân cấp với
hai cấp độ nhãn, dữ liệu được loại bỏ các dòng bị trùng lặp và được lưu trữ dưới dạng CSV.
Quá trình làm sạch dữ liệu bao gồm loại bỏ các dòng bị trùng lặp, loại bỏ các
nhãn có số lượng mẫu quá ít (Dưới 200 mẩu) và chuyển đổi dữ liệu về dạng chuẩn.

Phân bố dữ liệu trước và sau khi làm sạch được thể hiện qua các biểu đồ sau:

- Dữ liệu thô: [tại đây](./docs/raw/README.md)
- Dữ liệu đã làm sạch: [tại đây](./docs/clean/README.md)

Dataset bao gồm:

- Nhãn cấp độ 1
- Nhãn cấp độ 2
- Tiêu đề của bài báo
- Mô tả tóm tắt của bài báo

## 2. Thông tin Tổng quan về Dataset

### 2.1. Dataset sau khi làm sạch ([data-vn-express.raw.csv](./data-vn-express.raw.csv)) 

- **Tổng số mẫu**: 45,600
- **Số lượng nhãn chính**: 22
- **Số lượng nhãn phụ**: 108

### 2.2. Dataset trước khi làm sạch ([data-vn-express.clean.csv](./data-vn-express.clean.csv))

- **Tổng số mẫu**: 43,777
- **Số lượng nhãn chính**: 21
- **Số lượng nhãn phụ**: 95

## 3. Phân phối Dữ liệu

### 3.1. Phân phối theo Nhãn Chính

Dưới đây là phân phối của một số nhãn chính trong dataset:

| Nhãn Chính       | Trước Làm Sạch | Sau Làm Sạch | Ghi chú        |
|------------------|----------------|--------------|----------------|
| Giải trí         | 4,149          | 4,149        |                |
| Thể thao         | 2,692          | 2,647        |                |
| Pháp luật        | 1,204          | 1,199        |                |
| Giáo dục         | 3,448          | 3,322        |                |
| Sức khoẻ         | 3,513          | 3,513        |                |
| Du lịch          | 2,104          | 2,084        |                |
| Số hoá           | 2,234          | 2,234        |                |
| Thời sự          | 2,994          | 2,986        |                |
| Podcast          | 2,178          | 1,179        |                |
| Xe               | 1,199          | 1,199        |                |
| Ý kiến           | 1,196          | 1,196        |                |
| Thư giãn         | 2,894          | 2,894        |                |
| Góc nhìn         | 2,464          | 1,954        |                |
| Khoa học         | 3,248          | 3,246        |                |
| Kinh doanh       | 4,587          | 4,587        |                |
| Đời sống         | 2,398          | 2,398        |                |
| Thế giới         | 2,990          | 2,990        |                |
| **Bất động sản** | **108**        | **0**        | **Bị loại bỏ** |

### 3.2. Phân phối theo Nhãn Phụ

Mỗi nhãn chính được chia thành nhiều nhãn phụ. Dưới đây là phân phối của một số nhãn phụ trong các nhãn chính:

### Giải trí

| Nhãn Phụ            | Trước Làm Sạch | Sau Làm Sạch |
|---------------------|----------------|--------------|
| Giới sao            | 598            | 598          |
| Làm đẹp             | 576            | 576          |
| Sách                | 587            | 587          |
| Sân khấu - Mỹ thuật | 596            | 596          |
| Phim                | 598            | 598          |
| Thời trang          | 598            | 598          |
| Nhạc                | 596            | 596          |

### Thể thao

| Nhãn Phụ     | Trước Làm Sạch | Sau Làm Sạch | Ghi chú    |
|--------------|----------------|--------------|------------|
| Tennis       | 600            | 600          |            |
| Các môn khác | 598            | 598          |            |
| Hậu trường   | 572            | 572          |            |
| Ảnh          | 583            | 583          |            |
| Tin tức      | 294            | 294          |            |
| Euro 2024    | 37             | Bị loại bỏ   | Bị loại bỏ |
| Marathon     | 8              | Bị loại bỏ   | Bị loại bỏ |

### Pháp luật

| Nhãn Phụ     | Trước Làm Sạch | Sau Làm Sạch | Ghi chú    |
|--------------|----------------|--------------|------------|
| Video        | 599            | 599          |            |
| Hồ sơ phá án | 600            | 600          |            |
| Tư vấn       | 5              | Bị loại bỏ   | Bị loại bỏ |

### Giáo dục

| Nhãn Phụ      | Trước Làm Sạch | Sau Làm Sạch |
|---------------|----------------|--------------|
| Tuyển sinh    | 561            | 561          |
| Giáo dục 4.0  | 600            | 600          |
| Chân dung     | 498            | 498          |
| Học tiếng Anh | 588            | 588          |
| Tin tức       | 594            | 594          |
| Du học        | 481            | 481          |

### Sức khoẻ

| Nhãn Phụ   | Trước Làm Sạch | Sau Làm Sạch |
|------------|----------------|--------------|
| Đàn ông    | 563            | 563          |
| Dinh dưỡng | 582            | 582          |
| Tư vấn     | 600            | 600          |
| Khỏe đẹp   | 582            | 582          |
| Các bệnh   | 593            | 593          |
| Tin tức    | 593            | 593          |

### Du lịch

| Nhãn Phụ | Trước Làm Sạch | Sau Làm Sạch | Ghi chú    |
|----------|----------------|--------------|------------|
| Điểm đến | 599            | 599          |            |
| Ảnh      | 301            | 301          |            |
| Dấu chân | 588            | 588          |            |
| Ẩm thực  | 596            | 596          |            |
| Tư vấn   | 20             | Bị loại bỏ   | Bị loại bỏ |

### Thời sự

| Nhãn Phụ            | Trước Làm Sạch | Sau Làm Sạch | Ghi chú    |
|---------------------|----------------|--------------|------------|
| Lao động - Việc làm | 596            | 596          |            |
| Chính trị           | 598            | 598          |            |
| Dân sinh            | 600            | 600          |            |
| Giao thông          | 595            | 595          |            |
| Quỹ hy vọng         | 597            | 597          |            |
| Mekong              | 8              | Bị loại bỏ   | Bị loại bỏ |

### Số hoá

| Nhãn Phụ    | Trước Làm Sạch | Sau Làm Sạch |
|-------------|----------------|--------------|
| Kinh nghiệm | 596            | 596          |
| Công nghệ   | 589            | 589          |
| Sản phẩm    | 590            | 590          |
| Blockchain  | 459            | 459          |

### Thế giới

| Nhãn Phụ          | Trước Làm Sạch | Sau Làm Sạch |
|-------------------|----------------|--------------|
| Tư liệu           | 600            | 600          |
| Người Việt 5 châu | 595            | 595          |
| Quân sự           | 597            | 597          |
| Phân tích         | 599            | 599          |
| Cuộc sống đó đây  | 599            | 599          |

### Podcast

| Nhãn Phụ          | Trước Làm Sạch | Sau Làm Sạch | Ghi chú    |
|-------------------|----------------|--------------|------------|
| Điểm tin          | 590            | 590          |            |
| VnExpress hôm nay | 589            | 589          |            |
| Thầm thì          | 170            | Bị loại bỏ   | Bị loại bỏ |
| Kế hoạch lạc quan | 7              | Bị loại bỏ   | Bị loại bỏ |
| Tâm điểm kinh tế  | 10             | Bị loại bỏ   | Bị loại bỏ |
| Tài chính cá nhân | 90             | Bị loại bỏ   | Bị loại bỏ |
| Bạn ổn không?     | 178            | Bị loại bỏ   | Bị loại bỏ |
| Ly hôn            | 47             | Bị loại bỏ   | Bị loại bỏ |
| Úp mở 18+         | 12             | Bị loại bỏ   | Bị loại bỏ |
| Tiền làm gì?      | 69             | Bị loại bỏ   | Bị loại bỏ |
| Họ nói gì?        | 89             | Bị loại bỏ   | Bị loại bỏ |
| Giải mã           | 89             | Bị loại bỏ   | Bị loại bỏ |
| 360° World Cup    | 10             | Bị loại bỏ   | Bị loại bỏ |
| Hộp đen           | 101            | Bị loại bỏ   | Bị loại bỏ |
| Tôi trong gương   | 24             | Bị loại bỏ   | Bị loại bỏ |
| Chuyện đi làm     | 10             | Bị loại bỏ   | Bị loại bỏ |
| Nguy - Cơ         | 55             | Bị loại bỏ   | Bị loại bỏ |
| Tôi kể            | 38             | Bị loại bỏ   | Bị loại bỏ |

### Bất động sản

| Nhãn Phụ        | Trước Làm Sạch | Sau Làm Sạch | Ghi chú    |
|-----------------|----------------|--------------|------------|
| Không gian sống | 16             | Bị loại bỏ   | Bị loại bỏ |
| Tư vấn          | 92             | Bị loại bỏ   | Bị loại bỏ |

## 4. Chất lượng Dữ liệu

- **Trước làm sạch**: Tổng số mẫu là 45,600. Dữ liệu chứa một số dòng bị trùng lặp.
- **Sau làm sạch**: Tổng số mẫu giảm xuống còn 43,777. Các dòng bị trùng lặp và các nhãn có số mẫu dưới 200 đã được loại bỏ, giúp cải thiện chất lượng dữ liệu.

## 5. Phân tích và Đánh giá

### 5.1. Sự Đa dạng và Phân phối Dữ liệu

- Dataset bao gồm nhiều lĩnh vực khác nhau, từ giải trí, giáo dục, khoa học đến sức khoẻ, kinh doanh và thể thao.
- Phân phối dữ liệu khá đồng đều giữa các nhãn chính, với một số nhãn như giải trí và kinh doanh có số lượng mẫu cao.
- Câu dài nhất: 
  - Lòng biết ơn. Klanarong Srisakul là một cái tên xa lạ và khó đọc với ai không phải là cư dân Thái. Nhưng tên của chàng thanh niên này đã được hàng triệu người trên thế giới biết đến khi trong lễ tốt nghiệp, anh bận lễ phục của Đại học Chualongkorn danh tiếng nhất nước Thái, tìm người cha của mình và quỳ rạp xuống để lạy ông bên chiếc xe tải chở đầy rác bẩn. Anh bày tỏ lòng biết ơn với người cha mới chỉ học qua lớp 4 đã dành cả cuộc đời để nuôi dạy mình
- Câu ngắn nhất: 
  - Điểm thi. Học hết lớp tám khác gì học hết lớp năm?


### 5.2. Chất lượng Dữ liệu Sau Khi Làm Sạch

- Việc loại bỏ các dòng bị trùng lặp đã giúp giảm tổng số mẫu từ 45,600 xuống còn 43,777, cho thấy rằng quá trình thu thập dữ liệu ban đầu đã có một số dòng bị trùng lặp.
- Chất lượng dữ liệu được cải thiện, giúp tăng độ tin cậy cho các phân tích và mô hình học máy.

---
