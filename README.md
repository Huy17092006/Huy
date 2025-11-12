<title>Thiên Hà</title>
/* Thiết lập cơ bản cho trang */ html, body { Height: 100%; lề: 0; phần đệm: 0; tràn: ẩn; /* Ẩn thanh cuộn */ }
/* "Khung" chứa thiên hà */
.galaxy {
position: relative;
width: 100%;
height: 100%;
background: radial-gradient(ellipse at bottom, #1b2735 0%, #090a0f 100%);
z-index: 1;
}

/* Hàm tạo hoạt ảnh cho sao chuyển từ trên xuống dưới */
@Keyframesdi chuyển các ngôi sao {
từ {
biến đổi: translateY(-2000px);
}
đến {
biến đổi: translateY(0);
}
}

/* Lớp cơ sở cho các ngôi sao /
.stars, .stars2, .stars3 {
location: tuyệt đối;
trên cùng: -2000px; / Bắt đầu từ bên ngoài màn hình */
width: 100%;
chiều cao: 2000px;
lặp lại nền: lặp lại;
kích thước nền: chứa;
tên hoạt hình: ngôi sao di chuyển;
chức năng hoạt hình-thời gian: tuyến tính;
hoạt hình-lặp-đếm: vô hạn;
}

/* Lớp sao nhỏ và nhanh nhất (gần nhất) /
.stars {
nền-image: url(" https://www.transparenttextures.com/patterns/stardust.png ");
chỉ số z: 2;
thời lượng hoạt ảnh: 50 giây; / Chuyển tốc độ */
}

/* Lớp sao kích thước vừa /
.stars2 {
hình nền: url(" https://www.transparenttextures.com/patterns/stardust.png ");
kích thước nền: 80%; / Kích thước nhỏ hơn một chút /
z-index: 3;
độ mờ: 0,7;
thời lượng hoạt ảnh: 100 giây; / Chậm hơn */
}

/* Lớp sao lớn và chậm nhất (xa nhất) /
.stars3 {
hình nền: url(" https://www.transparenttextures.com/patterns/stardust.png ");
kích thước nền: 60%; / Kích thước nhỏ hơn nữa /
z-index: 4;
độ mờ: 0,4;
thời lượng hoạt ảnh: 150 giây; / Luồng nhất */
}
