# Mạch đóng ngắt tải MKE-M06 MOSFET Module

## Giới thiệu sản phẩm
Mạch đóng ngắt tải MKE-M06 MOSFET Module là mạch đóng ngắt tải một chiều (DC) sử dụng MOSFET công suất cao, cho phép điều khiển các thiết bị tiêu thụ dòng lớn với điện áp tối đa lên đến 30VDC và dòng tải tối đa 13A. Module sử dụng MOSFET kênh N AO4406AL, giúp đóng cắt tải nhanh, hoạt động bền bỉ, không gây tiếng ồn như relay cơ và có tuổi thọ rất cao.

Mạch đóng ngắt tải MKE-M06 MOSFET Module được ứng dụng rộng rãi trong nhiều hệ thống điều khiển và tự động hóa như: điều khiển dải LED công suất lớn, động cơ DC, máy bơm mini, van điện từ, quạt làm mát, hệ thống tưới cây tự động, hệ thống chiếu sáng thông minh, robot di động và nhiều thiết bị sử dụng nguồn DC khác. Khả năng đóng cắt bằng MOSFET còn cho phép điều khiển tốc độ động cơ hoặc điều chỉnh độ sáng LED thông qua tín hiệu PWM.

Mạch đóng ngắt tải MKE-M06 MOSFET Module được thiết kế đặc biệt phù hợp cho các mô hình robot, dự án STEM, đồ án học tập và thực hành điện – điện tử, giúp người học dễ dàng tiếp cận nguyên lý điều khiển tải công suất bằng MOSFET, kỹ thuật PWM và các ứng dụng tự động hóa thực tế. Đây là công cụ lý tưởng cho học sinh, sinh viên, giáo viên giảng dạy STEM và những người yêu thích sáng tạo công nghệ.

Mạch đóng ngắt tải MKE-M05 1-Relay Module hỗ trợ điện áp giao tiếp 3.3V và 5VDC, cho phép kết nối trực tiếp và an toàn với hầu hết các bo mạch điều khiển phổ biến hiện nay như Arduino, Raspberry Pi, Jetson Nano, Micro:bit và nhiều nền tảng khác. Sản phẩm đi kèm cáp kết nối 3P XH2.54 – Dupont, đảm bảo kết nối chắc chắn, ổn định và thuận tiện trong quá trình lắp đặt và sử dụng.

## Thông số kỹ thuật
- Điện áp cấp nguồn: Max 30VDC
- Điện áp tải tối đa: Max 30VDC
- Dòng tải tối đa: Max 13A
- Chuẩn tín hiệu điều khiển: Digital / PWM
- Điện áp giao tiếp: TTL 3.3/5VDC
- Loại MOSFET: AO4406AL N-Channel 30V 13A
- Mạch bảo vệ:
  - Tích hợp diode bảo vệ cho MOSFET
  - Bảo vệ an toàn cho chân GPIO của vi điều khiển
- Khả năng tương thích:
  - Arduino
  - Raspberry Pi
  - Jetson Nano
  - Micro:bit
  - Và các board điều khiển 3.3/5VDC khác
- Thiết kế mạch:
  - Hoạt động ổn định, chống nhiễu tốt
  - Hỗ trợ điều khiển tải công suất lớn
- Phù hợp cho ứng dụng học tập và thực tế
- Đi kèm cáp kết nối: 3P XH2.54 – Dupont

## Các chân tín hiệu
<table><thead>
  <tr>
    <th>MKE-M06</th>
    <th>Ghi chú</th>
  </tr></thead>
<tbody>
  <tr>
    <td>-</td>
    <td>Chân cấp nguồn âm 0VDC</td>
  </tr>
  <tr>
    <td>+</td>
    <td>Chân cấp nguồn dương Max 30VDC</td>
  </tr>
  <tr>
    <td>S</td>
    <td>Chân tín hiệu điều khiển Digital In</td>
  </tr>
</tbody>
</table>

## Hướng dẫn sử dụng
### Hướng dẫn kết nối
- Cấp nguồn 5VDC cho mạch qua hai chân GND và 5V.
- Điều khiển Relay qua chân tín hiệu S (SIGNAL).
<table><thead>
  <tr>
    <th>SIG (Digital In)</th>
    <th>Trạng thái</th>
  </tr></thead>
<tbody>
  <tr>
    <td>TTL HIGH (3.3/5VDC)</td>
    <td>Hoạt động (On)</td>
  </tr>
  <tr>
    <td>TTL LOW (0VDC)</td>
    <td>Không hoạt động (Off)</td>
  </tr>
</tbody>
</table>

### Hướng dẫn sử dụng với Arduino Uno / Vietduino Uno / ESP32
- Trong **Tools / Library Manager**, tìm và cài đặt bộ thư viện tổng hợp **"MKE_ONE" by MakerEdu.vn**
- Mở chương trình mẫu **"MKE_M05_Relay_Serial_XXX"** tại **File / Examples / MAKEREDU / Module / MKE_M05_Relay**
- Cấu hình board mạch tương ứng là **Arduino Uno / ESP32**, chọn đúng cổng **COM Port** của mạch và nhấn **Upload** để nạp chương trình.
- Cấp nguồn 5VDC cho mạch, kết nối chân S (SIGNAL) của module với chân điều khiển được khai báo trong chương trình.
- Xem kết quả mạch hoạt động theo chương trình đã nạp.

### Hướng dẫn lập trình với Micro:bit (kéo thả khối)

- Khởi động [Microsoft MakeCode](https://makecode.microbit.org/) và **Import** chương trình theo đường link sau: `https://github.com/makereduvn/mke_m05_relay_microbit/`
- Kết nối mạch Micro:bit và **Download** chương trình.
- Cấp nguồn 5VDC cho mạch, kết nối chân S (SIGNAL) của module với chân điều khiển được khai báo trong chương trình.
- Xem kết quả mạch hoạt động theo chương trình đã nạp.

Nếu bắt đầu tự án mới cần cài đặt Extension **MKE_ONE_MICROBIT** trên [Microsoft MakeCode](https://makecode.microbit.org/) theo [hướng dẫn tại đây](https://github.com/makereduvn/MKE_ONE_MICROBIT). Sau khi cài đặt thành công, các khối lệnh của Extension **MKE_ONE_MICROBIT** sẽ xuất hiện trong danh sách block và sẵn sàng để sử dụng.

## Kích thước sản phẩm
![MKE-M05 Relay](/extras/MKE-M05_1.jpg)

## Hình ảnh sản phẩm
![MKE-M05 Relay](/extras/MKE-M05_2.png)
![MKE-M05 Relay](/extras/MKE-M05_3.png)


