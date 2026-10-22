# AniTV — App xem Anime (Android, Kotlin)

App xem anime lấy dữ liệu từ API công khai của cobephim (lọc sẵn thể loại
Hoạt Hình), build APK hoàn toàn bằng **GitHub Actions** — không cần cài
Android Studio.

## Tính năng

- Trang chủ: Anime mới cập nhật, Anime bộ đang chiếu, Anime lẻ (movie),
  Anime Nhật Bản, Donghua Trung Quốc
- Tab Anime lẻ / Anime bộ / Nhật Bản / Donghua — tải thêm theo trang
- Tìm kiếm anime theo tên (gõ đến đâu tìm đến đó)
- Chi tiết: thông tin phim, danh sách tập theo từng bản chiếu
  (Vietsub / Lồng tiếng / Thuyết minh...)
- Trình phát: bắt luồng trực tiếp từ trang phát chính thức, chặn popup
  quảng cáo; không bắt được luồng thì phát ngay trong trang embed đã khóa
- Yêu thích + thông báo khi có tập mới, Lịch sử xem
- Chống đổi tên miền: app đọc `config.json` trên repo này để cập nhật
  địa chỉ nguồn (sửa file đó là mọi máy đang cài tự cập nhật)

## Cách build APK

1. Tạo repo **AniTV-app**, đẩy toàn bộ mã nguồn lên (không gồm thư mục
   `.github/workflows`).
2. Dán nội dung file `WORKFLOW-PASTE.txt` vào
   `.github/workflows/build.yml` bằng trình sửa trên web GitHub.
3. Mỗi lần đẩy code lên nhánh `main`, Actions tự build; tải APK ở
   Artifacts tên **anitv-apk**.
