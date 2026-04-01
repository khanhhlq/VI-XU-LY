Dùng vi điều khiển 16F887, kết nối với một nút nhấn thường hở ON/OFF (nối RE0), một nút nhấn chuyển kênh CHANNEL(nối RE1), một LED 7 đoạn Anode chung nối port B, một màn hình LCD 16x2. Khi nhấn ON/OFF, mạch sẽ hoạt động, khi mạch hoạt động nút CHANNEL có chức năng chọn lần lượt từng kênh K_1, K_2 và K_3 tương ứng mỗi lần nhấn và hiển thị số thứ tự kênh sang LED 7 đoạn. Màn hình LCD sẽ hiển thị với ố kênh đã được chọn:

Kênh 1:
///////////////////////////
/        VIETNAMESE       /
/         XIN CHAO        /
///////////////////////////

Kênh 2:
///////////////////////////
/         ENGLISH         /
/          HELLO          /
///////////////////////////

Kênh 3:
///////////////////////////
/         GERMANY         /
/          HALLO          /
///////////////////////////

KHI VỪA CẤP ĐIỆN, MÀN HÌNH LCD HIỂN THỊ
///////////////////////////
/         NHAN ON         /
/        DE BAT DAU       /
///////////////////////////

NHẤN NÚT ON/OFF MỘT LẦN NỮA THÌ CHUYỂN SANG TRẠNG THÁI OFF, KHI ĐÓ LED 7 ĐOẠN TẮT VÀ MÀN HÌNH LCD HIỂN THỊ NHƯ LÚC VỪA MỚI CẤP ĐIỆN.
NHẤN LẠI ON/OFF VỀ TRẠNG THÁI ON

TRƯỚC KHI MUỐN HIỂU THỊ KÊNH KHÁC, PHẢI XOÁ BỎ HẾT TOÀN BỘ THÔNG TIN CŨ TRÊN LCD TRƯỚC ĐÓ RỒI MỚI XUẤT CÁI TIẾP THEO RA. NÊN XUẤT 16 KHOẢNG TRẮNG RA HAI DÒNG

LCD_GOTOXY(1,1);
LCD_PUTC("                ");
LCD_GOTOXY(1,2);
LCD_PUTC("                ");