# CNJAVA
DOWNLOAD FILE RAR CỦA GAME BẰNG CÁCH ẤN VÀO CODE RỒI DOWNLOAD ZIP

HƯỚNG DẪN CÀI ĐẶT
1-CÁCH CÀI ĐẶT PONGGAME VÀO MÁY TÍNH KHÁC CHỈ CÓ JDK
Để chạy game Pong trên máy tính của bạn, bạn cần thực hiện các bước sau:
1.Tải xuống và giải nén file zip chứa mã nguồn của game Pong.
2.Tạo cơ sở dữ liệu trên máy tính của bạn. Bạn có thể sử dụng một hệ quản trị cơ sở dữ liệu như MySQL hoặc PostgreSQL. Nếu game của bạn đã đi kèm với tệp cơ sở dữ liệu, bạn có thể bỏ qua bước này.
3.Mở cửa sổ Command Prompt hoặc Terminal và di chuyển đến thư mục chứa mã nguồn của game bằng lệnh cd
4.Biên dịch mã nguồn của PongGame.java thành mã bytecode bằng lệnh javac:
javac -cp .;Lib/Mysql-connection-java-8.0.30.jar;Lib/Protobuf-java-3.19.4.jar PONG_GAME/PongGame.java
5.Chạy game bằng lệnh java –cp :
java -cp .;Lib/Mysql-connection-java-8.0.30.jar;Lib/Protobuf-java-3.19.4.jar PONG_GAME/PongGame
 Lưu ý rằng bạn cần thay thế <đường dẫn đến thư viện> bằng đường dẫn đến thư mục chứa các tệp .jar trên máy tính của bạn. Nếu bạn không thực hiện việc này, Java sẽ không tìm thấy các thư viện cần thiết để chạy game và sẽ báo lỗi.
Sau khi chạy lệnh trên, game sẽ được khởi chạy và hiển thị trên màn hình. Bạn có thể sử dụng các phím mũi tên để di chuyển thanh trượt và chơi game như bình thường.

2.	CÁCH ĐỂ TẠO CSDL CỦA PONGGAME
-Tạo một cơ sở dữ liệu mới với tên "baitaplon" chứa bảng "scores" có hai thuộc tính "player_name" và "score" có thể làm theo các bước sau:
1.	Tạo một cơ sở dữ liệu mới với tên "baitaplon" bằng cách chọn tùy chọn "Create new database" hoặc "New database" trong giao diện của phần mềm.
2.	Sau khi tạo cơ sở dữ liệu mới, bạn có thể tạo bảng mới bằng cách chọn tùy chọn "Create new table" hoặc "New table" trong giao diện của phần mềm.
3.	Đặt tên cho bảng mới là "scores" và thêm hai cột cho bảng là "player_name" với kiểu dữ liệu VARCHAR và "score" với kiểu dữ liệu INTEGER.
4.	Lưu ý không đặt khóa cho cả hai thuộc tính do có thể có hai người chơi có tên giống nhau
    // TÙY THEO MÁY MÀ CỔNG CỦA MYSQL SẼ KHÁC NHAU
 3.	ĐỂ ĐỔI CỔNG KẾT NỐI CỦA MYSQL TỪ CỔNG BẤT KÌ THÀNH 3306 TRONG XAMPP, BẠN CẦN THỰC HIỆN CÁC BƯỚC SAU:
1.	Mở XAMPP Control Panel và bật Apache và MySQL.
2.	Truy cập vào phpMyAdmin bằng cách nhấp vào nút "Admin" của MySQL trên XAMPP Control Panel.
3.	Trong giao diện phpMyAdmin, nhấp vào tab "Variables" để mở trang cấu hình biến của MySQL.
4.	Tìm kiếm biến có tên "port" và nhấp vào nút "Edit" ở bên cạnh nó.
5.	Nhập số cổng mới là 3306 vào ô "Value" và nhấp vào nút "Go" để lưu thay đổi.
6.	Khởi động lại dịch vụ MySQL bằng cách nhấp vào nút "Stop" và sau đó là nút "Start" trên XAMPP Control Panel.

