<p align="center">
  <img src="assets/icon.png" width="128" alt="Biểu tượng Device Hub for Android">
</p>

<h1 align="center">Device Hub for Android</h1>

<p align="center"><b>Duyệt tệp, chép tệp và xem/điều khiển màn hình nhiều điện thoại Android ngay trên Mac — trong một cửa sổ.</b><br>
Ứng dụng macOS thuần, kết nối USB hoặc Wi‑Fi. Không tài khoản, không đám mây, không thu thập dữ liệu.</p>

<p align="center">
  <a href="https://github.com/hoangvunam/afs-for-mac/releases/latest"><img alt="Tải về" src="https://img.shields.io/badge/T%E1%BA%A3i%20v%E1%BB%81-GitHub%20Releases-2ea44f?style=for-the-badge&logo=apple&logoColor=white"></a>
  <img alt="Mac App Store: sắp có" src="https://img.shields.io/badge/Mac%20App%20Store-s%E1%BA%AFp%20c%C3%B3-lightgrey?style=for-the-badge&logo=appstore&logoColor=white">
</p>

<p align="center"><a href="README.md">🇬🇧 English</a></p>

<p align="center">
  <img src="assets/files-dark.png" alt="Trình duyệt tệp có xem trước ảnh (giao diện tối)">
</p>

## Tính năng

**Tệp**
- Nhiều điện thoại cùng lúc; thanh bên có thư mục yêu thích (Tải về, Camera, Ảnh, Phim, Nhạc, Tài liệu), bộ nhớ trong và thư mục ứng dụng
- Duyệt, đổi tên, tạo thư mục, xóa, hiện tệp ẩn, lịch sử tiến/lùi/lên
- Xem trước ảnh và video ngay trong khung thông tin, kèm dung lượng, quyền và đường dẫn
- Kéo tệp từ Finder thả vào cửa sổ (hoặc lên màn hình điện thoại), bấm nút **Nhập** (⇧⌘I) hoặc dán từ Finder bằng ⌘V để chép sang điện thoại; tải về Mac chỉ một cú bấm
- Khi không chọn gì, khung thông tin hiện thư mục đang mở: số mục, dung lượng và nút Nhập

**Truyền tệp**
- Truyền trực tiếp nhanh, có hàng đợi, tiến độ thật, hủy, xử lý trùng tên (hỏi / giữ cả hai / thay thế / bỏ qua)
- Hai điện thoại cạnh nhau (chia đôi cửa sổ)
- Nhập ảnh/video: quét DCIM / Pictures / Movies, chỉ chép mục mới vào thư mục `YYYY/YYYY-MM`, không bao giờ ghi đè

**Kết nối**
- **Ghép nối qua Wi‑Fi** bằng mã QR hoặc mã 6 số (Android 11+); USB và Wi‑Fi của cùng một máy hiện thành một thiết bị, mất một đường thì ứng dụng đề nghị chuyển sang đường kia
- **Chép tệp không cần Gỡ lỗi USB:** để điện thoại ở chế độ *Truyền tệp* (MTP) hoặc *Truyền ảnh* (PTP) là duyệt, chép, đổi tên, xoá và xem trước được ngay. Bật Gỡ lỗi USB khi cần xem màn hình và quản lý ứng dụng — ứng dụng tự chuyển và giữ nguyên thư mục đang mở
- **Máy ảo Android:** bật và tắt máy ảo Android Studio ngay ở thanh bên, xem màn hình và đổi trạng thái gập của máy ảo màn hình gập

**Xem và điều khiển màn hình**
- Màn hình điện thoại hiển thị cạnh danh sách tệp (hoặc tách thành cửa sổ riêng); cảm ứng, bàn phím, cuộn, gõ tiếng Việt (Telex)
- Clipboard hai chiều, âm thanh thiết bị, xoay màn hình, chụp màn hình, quay video
- Nút Quay lại / Trang chủ / Đa nhiệm / âm lượng / nguồn

**Ứng dụng và thiết bị**
- Quản lý ứng dụng: danh sách, cài APK, gỡ cài đặt
- Xem pin và dung lượng nhanh

**Dành riêng cho Mac**
- SwiftUI, Liquid Glass trên macOS 26, Sáng/Tối, giao diện 20 ngôn ngữ
- Kèm sẵn `adb` và `scrcpy-server` — không cần cài thêm gì

| Màn hình (sáng) | Màn hình (tối) |
|---|---|
| <img src="assets/mirror-light.png" alt="Xem màn hình, giao diện sáng"> | <img src="assets/mirror-dark.png" alt="Xem màn hình, giao diện tối"> |

> Ảnh chụp dùng ảnh mẫu từ [Unsplash](https://unsplash.com).

## Yêu cầu

- macOS 14 Sonoma trở lên (Apple silicon và Intel)
- Điện thoại Android và cáp USB truyền dữ liệu. Chép tệp chỉ cần chế độ *Truyền tệp*; xem màn hình và quản lý ứng dụng cần bật **Gỡ lỗi USB**
- Ghép nối Wi‑Fi cần Android 11+ và điện thoại cùng mạng với Mac
- Thu âm thanh cần Android 11+; đã thử trên Android 12 và 17

## Cài đặt

1. Tải `Device-Hub-for-Android-x.y.z.dmg` mới nhất ở [Releases](https://github.com/hoangvunam/afs-for-mac/releases/latest), mở ra và kéo **Device Hub for Android** vào Applications. Ứng dụng được ký Developer ID và Apple notarize.
2. Chỉ chép tệp: cắm điện thoại, mở khoá và chọn **Truyền tệp** trong thông báo USB là xong. Muốn xem màn hình và quản lý ứng dụng thì bật thêm Gỡ lỗi USB: **Cài đặt → Giới thiệu điện thoại →** chạm *Số bản dựng* 7 lần, rồi **Cài đặt → Hệ thống → Tùy chọn nhà phát triển → Gỡ lỗi USB**.
3. Cắm USB và chạm **Cho phép** ở hộp thoại "Cho phép gỡ lỗi USB?" (chọn *Luôn cho phép*).

**Bản Mac App Store:** chạy trong App Sandbox với khóa adb riêng, nên lần đầu kết nối bạn phải chạm **Cho phép gỡ lỗi USB** thêm một lần nữa trên điện thoại.

## Câu hỏi thường gặp

**Điện thoại báo "Chưa cấp quyền" hoặc không hiện.** Mở khóa máy, cắm lại cáp và chấp nhận hộp thoại gỡ lỗi USB. Nếu hộp thoại không bao giờ hiện, thử *Thu hồi ủy quyền gỡ lỗi USB* trong Tùy chọn nhà phát triển. Kiểm tra cáp có truyền dữ liệu và chế độ USB không phải "chỉ sạc".

**Có cần cài adb hay scrcpy không?** Không, đã kèm sẵn. Nếu máy đang chạy một `adb` khác phiên bản, adb sẽ khởi động lại server một lần — bình thường.

**Có dùng qua Wi‑Fi được không?** Có. Chọn *Kết nối qua Wi‑Fi…* rồi ghép bằng mã QR hoặc mã 6 số trong *Tùy chọn nhà phát triển → Gỡ lỗi không dây* (Android 11+). Tệp không bao giờ rời khỏi mạng nội bộ.

**Có bắt buộc bật Gỡ lỗi USB không?** Không, nếu chỉ chép tệp. Ở chế độ *Truyền tệp* ứng dụng dùng giao thức MTP chuẩn qua macOS. Xem màn hình và quản lý ứng dụng mới cần Gỡ lỗi USB.

**Dữ liệu của tôi có bị gửi đi đâu không?** Không. Mọi thứ đi thẳng giữa Mac và điện thoại qua USB hoặc mạng nội bộ; không có tài khoản, thống kê hay kết nối tới máy chủ của chúng tôi.

**Tên tệp có dấu tiếng Việt hoặc emoji?** Hỗ trợ đầy đủ (giữ nguyên Unicode).

**Vì sao một số ứng dụng hiện màn hình đen?** Ứng dụng chặn chụp màn hình (ví dụ ngân hàng dùng `FLAG_SECURE`) sẽ đen — do Android áp đặt.

## Quyền riêng tư

Device Hub for Android không thu thập dữ liệu. Xem [Chính sách quyền riêng tư](PRIVACY.md) và [Điều khoản sử dụng](TERMS.md).

## Phần mềm bên thứ ba

- Server [scrcpy](https://github.com/Genymobile/scrcpy) (v3.1) — © Genymobile, giấy phép Apache 2.0
- Android SDK Platform-Tools (`adb`) — © The Android Open Source Project, giấy phép Apache 2.0; tải từ kênh phân phối chính thức của Google

Thông báo đầy đủ nằm trong app (*Cài đặt → Giới thiệu → Mở thông báo bản quyền*).

## Hỗ trợ

Email [namhv.cntt@gmail.com](mailto:namhv.cntt@gmail.com) hoặc [trang hỗ trợ](SUPPORT.md).

---

Repo này chỉ chứa bản tải và tài liệu; không chứa mã nguồn.
© 2026 Hoàng Vũ Nam. Android là nhãn hiệu của Google LLC. Device Hub for Android là sản phẩm độc lập, không liên kết hay được Google bảo trợ.
