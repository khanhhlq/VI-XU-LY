Sử dụng vi điều khiển 16F887, kết nối một nút nhấn ON (RE0), một nút nhân ADJ (RE1), một LCD 16x2, một LED đơn nối RA0 và 2 LED 7 đoạn anode chung nối port B và port C. Khi chưa nhấn ON (hoặc trạng thái OFF), ta có thể điều chỉnh được số giấy đặt trước thông qua nút ADJ:
+ Phạm vi đếm giây từ 0 đến 60
+ Mỗi lần nhấn ADJ sẽ tăng số giây lên 5. Giá trị của số giây cài trước sẽ hiển thị sang 2 LED 7 đoạn (biến giây cài gọi là S_SET)

Khi nhấn ON, thì mạch bắt đầu đếm, số giây hiển thị (S_DIS) tăng từ 0 cho đến giá trị giây cìa trước và cứ lặp lại trạng thái đếm. Giá trị giây hiển thị và giá trị giây cài đặt cũng được hiển thị trên LCD theo định dạng:

\\\\\\\\\\\\\\\\\\\\\\\\\\
\ CAI DAT:            XY \
\ HIEN TAI:           ZT \
\\\\\\\\\\\\\\\\\\\\\\\\\\

Với XY và ZT lần lượt là giá trị của biến S_SET và S_DIS
Khi giá trị giây hiển thị bằng với thời gian đã cài trước thì LED đơn chớp tắt 0,5 giây
Khi vừa cấp điện các trạng thái XY ZT đều là 00 hết, màn hình hiển thị

\\\\\\\\\\\\\\\\\\\\\\\\\\
\ CAI DAT:            00 \
\ HIEN TAI:           00 \
\\\\\\\\\\\\\\\\\\\\\\\\\\
