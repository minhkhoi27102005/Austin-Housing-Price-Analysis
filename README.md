# 🏡 Austin Housing Market Analysis (2018 - 2021)

Báo cáo phân tích chuyên sâu dữ liệu thị trường bất động sản tại thành phố Austin, Texas dựa trên bộ dữ liệu giao dịch giai đoạn 2018–2021.

---

## 📌 1. Giới thiệu (Introduction)

Dự án thực hiện phân tích hiệu suất giao dịch, định giá bất động sản, cấu trúc phân khúc sản phẩm và các đặc tính nhà ở tại thị trường Austin, Texas. Mục tiêu chính nhằm tối ưu hóa chiến lược đầu tư, đánh giá hiệu quả các tiêu chí bất động sản và nâng cao tỷ suất lợi nhuận cho các nhà đầu tư và đơn vị phát triển tài sản.

**Bộ dữ liệu gồm 15.171 bản ghi với 47 thuộc tính, tập trung vào 3 nhóm dữ liệu trọng tâm:**
* **Thông tin giao dịch & Giá:** Giá bán (`latestPrice`), thời gian bán (`latest_saledate`, `latest_saleyear`), số lần điều chỉnh giá (`numPriceChanges`).
* **Đặc điểm bất động sản:** Loại hình (`homeType`), vị trí (`city`, `zipcode`), diện tích nhà (`livingAreaSqFt`), diện tích đất (`lotSizeSqFt`), năm xây dựng (`yearBuilt`), số phòng ngủ/phòng tắm.
* **Tiện ích & Tiêu chuẩn sống:** Số lượng ảnh (`numOfPhotos`), đánh giá trường học (`avgSchoolRating`), khoảng cách trường học (`avgSchoolDistance`), gara, tiện ích đi kèm (hồ bơi/spa, hệ thống sưởi/làm mát, view).

---

## 📊 2. Tổng quan Thị trường (Overview Metrics)

### Các chỉ số hiệu suất thị trường chung
* **Tổng số lượng bất động sản (Total Properties):** 15.171 căn
* **Giá niêm yết trung bình (Average Price):** $512.768
* **Giá niêm yết trung vị (Median Price):** $405.000
* **Đơn giá trung bình theo diện tích (Avg Price/SqFt):** $238,54 / sqft (~$2.568 / m²)
* **Diện tích nhà trung bình (Avg Living Area):** 2.208 sqft (~205 m²)
* **Năm xây dựng trung bình (Avg Year Built):** 1989
* **Số lần thay đổi giá trung bình (Avg Price Changes):** 3,03 lần / căn

---

## 📈 3. Phân bố Chi tiết (Detailed Distributions)

### Phân bố lượng bất động sản theo loại hình sản phẩm (Home Type)

| Loại hình nhà ở | Số lượng bất động sản | Tỷ trọng | Giá bán trung bình | Diện tích nhà trung bình |
| :--- | :---: | :---: | :---: | :---: |
| **Single Family** | 14.241 | 93,9% | $516.388 | 2.235 sqft |
| **Condo** | 470 | 3,1% | $406.016 | 1.498 sqft |
| **Townhouse** | 174 | 1,1% | $424.720 | 1.728 sqft |
| **Multiple Occupancy** | 96 | 0,6% | $429.664 | 2.215 sqft |
| **Khác (Land, MultiFamily...)** | 190 | 1,3% | $628.122 | 2.502 sqft |
| **Tổng cộng** | **15.171** | **100%** | **$512.768** | **2.208 sqft** |

### Phân bố bất động sản theo khoảng giá (Price Tiers)

| Khoảng giá | Số lượng bất động sản | Tỷ trọng | Đơn giá trung bình ($/sqft) |
| :--- | :---: | :---: | :---: |
| **Dưới $250k** | 1.996 | 13,2% | $151,39 |
| **$250k - $400k** | 5.580 | 36,8% | $206,13 |
| **$400k - $600k** | 4.355 | 28,7% | $240,86 |
| **$600k - $1M** | 2.298 | 15,1% | $298,61 |
| **Trên $1M** | 942 | 6,2% | $457,83 |
| **Tổng cộng** | **15.171** | **100%** | **$238,54** |

---
## 🖥️ 4. POWER BI DASHBOARD PREVIEW

<img width="100%" alt="Austin Housing Executive Overview" src="https://github.com/user-attachments/assets/f59900b9-8677-42a1-a812-2b08a2d06452" />
<p align="center"><i>Hình 1: Trang Executive Overview - Tổng quan Thị trường, Xu hướng Giá bán & Cấu trúc Phân khúc Sản phẩm</i></p>

<br/>
<hr/>
<br/>

<img width="100%" alt="Austin Housing Location Intelligence" src="https://github.com/user-attachments/assets/460fc746-78d9-4642-a660-d8fb3de778fb" />
<p align="center"><i>Hình 2: Trang Location Intelligence - Phân tích Yếu tố Vị trí, Yếu tố Trường học & Phân bố Giá theo Khu vực</i></p>

<br/>
<hr/>
<br/>

<img width="100%" alt="Austin Housing Property Features" src="https://github.com/user-attachments/assets/c5cb309c-1214-428f-8875-251a15ad94da" />
<p align="center"><i>Hình 3: Trang Property Features - Phân tích Tương quan Đặc tính Nhà ở, Tiện ích & Tiêu chuẩn Sống</i></p>

---

## 💡 5. INSIGHTS

### Yếu tố Vị trí & Dòng tiền Đầu tư
Phân tích mặt bằng giá bán cho thấy vị trí địa lý là yếu tố quyết định phân khúc giá bất động sản tại thị trường Austin. Mức giá trung bình tại West Lake Hills đạt $1.425.000, cao gấp khoảng 2,8 lần so với trung bình khu vực Austin ($514.785) và gấp 7,2 lần so với khu vực Del Valle ($197.036).
Mặc dù khu vực có phân khúc giá cao mang lại giá trị tài sản lớn, dư địa tăng trưởng thường hẹp hơn. Ngược lại, phân khúc tầm trung ($250.000 – $400.000) chiếm tỷ trọng giao dịch lớn nhất thị trường với 36,8% (5.580 căn), kết hợp cùng phân khúc $400.000 – $600.000 chiếm 28,7% (4.355 căn). Điều này chứng minh các sản phẩm thuộc khoảng giá $250.000 – $600.000 nắm giữ tính thanh khoản cao nhất và có chu kỳ giao dịch ngắn hơn.

### Tiêu chí Bất động sản: Diện tích vs. Chất lượng Trường học
Tương quan dữ liệu cho thấy quyết định định giá nhà ở bị chi phối trực tiếp bởi không gian sống thực tế hơn là các tiện ích giáo dục lân cận. Diện tích sinh hoạt (`livingAreaSqFt`) và số lượng phòng tắm (`numOfBathrooms`) có mối tương quan thuận mạnh mẽ nhất đối với giá bán: nhóm nhà giá trên $1M có diện tích trung bình 4.081 sqft, so với 1.503 sqft ở nhóm dưới $250k.
Trái lại, điểm đánh giá trường học (`avgSchoolRating`) và khoảng cách tới trường (`avgSchoolDistance`) thể hiện mức độ ảnh hưởng thứ yếu. Người mua sẵn sàng chi trả mức thặng dư giá lớn hơn cho các bất động sản sở hữu công năng vượt trội và không gian rộng rãi thay vì chỉ thuần túy dựa vào chất lượng hay khoảng cách tới các trường học xung quanh.

### Chiến lược Gia tăng Giá trị cho Phân khúc Cao cấp
Ở phân khúc cao cấp và siêu sang (trên $600.000 đến $1M+), yếu tố quyết định thặng dư giá nằm ở "phong cách sống" thay vì chỉ dựa vào mở rộng diện tích thô. Đơn giá trung bình trên mỗi sqft của phân khúc trên $1M đạt $457,83/sqft, cao gấp 3 lần so với phân khúc dưới $250k ($151,39/sqft).
Sự chênh lệch đơn giá này xuất phát từ việc tích hợp các tiện ích gia tăng giá trị như hướng nhìn (`hasView`), không gian spa/hồ bơi (`hasSpa`), hệ thống sưởi/làm mát cao cấp, gara đỗ xe rộng rãi và các tiện ích nội khu (`numOfCommunityFeatures`). Đây chính là chìa khóa tạo nên giá trị khác biệt và thiết lập mặt bằng giá bán cao vượt trội cho tài sản.

---

## 🚀 6. ĐỀ XUẤT (RECOMMENDATIONS)

### Tối ưu danh mục đầu tư theo Mã bưu chính và Phân khúc tầm trung
* **Tập trung ngân sách vào khoảng giá thanh khoản cao ($250k - $400k):** Ưu tiên phân bổ vốn vào các mã bưu chính thuộc phân khúc tầm trung có nền tảng hạ tầng tốt. Đây là nhóm chiếm tới 36,8% thị phần, giúp cân bằng tối ưu giữa chi phí vốn đầu tư, tính thanh khoản nhanh và tiềm năng tăng giá bền vững trong dài hạn.
* **Đánh giá bộ tiêu chí hạ tầng bổ trợ:** Chọn lọc các mã bưu chính có tỷ lệ nguồn cung ổn định, giá trị giao dịch tăng trưởng đều qua các năm và sở hữu mặt bằng trường học từ mức khá trở lên để làm nền tảng bảo toàn giá trị tài sản.

### Chuẩn hóa tiêu chí lựa chọn bất động sản dựa trên Công năng thực tế
* **Ưu tiên cấu trúc công năng và diện tích:** Đặt diện tích sinh hoạt (`livingAreaSqFt`), số lượng phòng tắm (`numOfBathrooms`) và bố cục mặt bằng làm tiêu chí lọc định lượng hàng đầu khi khảo sát tài sản đầu tư.
* **Tối ưu hóa vị trí trường học làm yếu tố bổ trợ:** Xem chỉ số đánh giá trường học (`avgSchoolRating`) là đòn bẩy cộng hưởng để gia tăng giá trị khi bán lại, tuyệt đối không sử dụng làm điều kiện quyết định tiên quyết để chấp nhận mức giá chênh lệch quá cao.

### Triển khai chiến lược Cải tạo/Nâng cấp tạo Giá trị gia tăng (Value-Add Strategy)
* **Tập trung cải tạo tiện ích phục vụ lối sống:** Tối ưu hóa chi phí đầu tư bằng cách nâng cấp nội thất, tích hợp các tiện ích không gian sống (sân vườn/patio, hệ thống làm mát/sưởi hiện đại, tối ưu hóa tầm nhìn) cho bất động sản sau khi mua lại thay vì thuần túy chi tiền nới rộng diện tích xây dựng thô.
* **Tối đa hóa đơn giá bán/sqft khi thoát hàng:** Định hình gói cải tạo theo tiêu chuẩn phân khúc cao cấp nhằm đẩy mạnh đơn giá/sqft khi bán lại, rút ngắn thời gian niêm yết trên thị trường và tối ưu hóa tỷ suất lợi nhuận trên vốn đầu tư (ROI).

---

## 🛠️ 7. Công nghệ sử dụng (Tech Stack)

* **Business Intelligence & Visualization:** Microsoft Power BI (DAX, Power Query, Interactive Dashboards)
* **Data Source:** CSV Dataset (Austin Housing Market Data)

---

## 📂 8. Cấu trúc thư mục (Project Structure)

```text
.
├── austinHousingData.csv           # File dữ liệu bất động sản gốc
├── Austin_Housing_Dashboard.pbix   # Báo cáo trực quan hóa & Phân tích Dashboard trên Power BI
└── README.md                       # Báo cáo tổng quan, Insights & Đề xuất dự án
