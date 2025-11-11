VoxelLauncher - Hướng Dẫn Sử Dụng & README
VoxelLauncher là launcher Minecraft tùy chỉnh được xây dựng bằng WinUI 3 và Windows App SDK, sử dụng thư viện CmlLib.Core để hỗ trợ đầy đủ các tính năng Minecraft Java Edition. Launcher được phát triển bởi ShadowZa982 (GitHub: ShadowZa982/VoxelLauncher).
Launcher tập trung vào giao diện đẹp, dễ sử dụng, hỗ trợ đăng nhập Microsoft/Offline, tải phiên bản Minecraft tự động, và cập nhật launcher qua GitHub Releases.
Phiên bản hiện tại: v1.0.0 (cập nhật ngày 11/11/2025)
Yêu cầu hệ thống: Windows 10 (version 1803 trở lên) hoặc Windows 11 (version 21H2 trở lên).

📋 Mô Tả Tổng Quan
VoxelLauncher là launcher miễn phí, mã nguồn mở, giúp người dùng dễ dàng chơi Minecraft Java Edition mà không cần tải thủ công các file từ Mojang.
Đặc điểm nổi bật:

Giao diện hiện đại: Sử dụng WinUI 3 với theme tối, animation mượt mà, sidebar dễ điều hướng.
Hỗ trợ tài khoản: Đăng nhập Microsoft (Xbox Live) hoặc chơi Offline với tên tùy chỉnh. Lưu nhiều tài khoản, dễ chuyển đổi.
Quản lý phiên bản: Tải tự động danh sách phiên bản từ Mojang, hỗ trợ tất cả phiên bản Java Edition (1.7.10 - 1.21+).
Tích hợp Java: Tự động phát hiện và sử dụng Java cài sẵn, hỗ trợ tải Java nếu thiếu.
Cập nhật tự động: Kiểm tra và tải cập nhật launcher từ GitHub, với progress bar chi tiết (tốc độ tải, dung lượng).
Thông báo: Hiển thị toast notification khi đăng nhập thành công, và badge cho cập nhật bị bỏ qua.
Tùy chỉnh: Sidebar với các tab (Changelog, Mods, Servers, Đối tác), hỗ trợ WebView2 để hiển thị nội dung web.
Bảo mật: Sử dụng MSessionFileStorage để lưu tài khoản an toàn, hỗ trợ XboxAuthNet cho xác thực Microsoft.

Launcher không yêu cầu tài khoản Mojang Premium để chơi Offline, nhưng cần Premium để chơi online với server.

🎮 Chức Năng Chính
1. Đăng Nhập & Quản Lý Tài Khoản

Microsoft Account: Hỗ trợ xác thực Xbox Live qua MSAL (Microsoft Authentication Library). Lưu session tự động, tự động đăng nhập khi mở launcher.
Offline Mode: Chơi với tên tùy chỉnh, không cần internet.
Quản lý: Lưu nhiều tài khoản, xem avatar Minecraft, thời gian đăng nhập cuối, loại tài khoản. Hỗ trợ xóa tài khoản.
Thông báo: Toast notification khi đăng nhập thành công với avatar.

2. Tải & Chạy Minecraft

Danh sách phiên bản: Tải metadata từ Mojang, hiển thị tất cả phiên bản (release, snapshot).
Tải game: Sử dụng ParallelGameInstaller để tải song song assets, libraries, client JAR. Hỗ trợ Mojang servers.
Java tích hợp: Phát hiện Java tự động, hỗ trợ Java 8+ (tối thiểu Java 17 cho phiên bản mới).
Chạy game: Sử dụng MinecraftLauncherParameters, hỗ trợ tùy chỉnh RAM, JVM args.

3. Cập Nhật Launcher

Kiểm tra tự động: Sử dụng appcast.xml từ GitHub Releases, so sánh version assembly.
Dialog cập nhật: Hiển thị notes HTML qua WebView2, với nút "Cập nhật ngay" / "Để sau".
Tải ZIP: Tải release ZIP với progress bar (dung lượng, tốc độ KB/s), kiểm tra tính toàn vẹn ZIP.
Cài đặt: Chạy VoxelUpdater.exe để giải nén, kill launcher cũ, khởi động lại. Hỗ trợ pending updates (cập nhật bị bỏ qua).

4. Giao Diện & Tùy Chỉnh

Sidebar: Menu trượt với các trang (Info, Mods, Servers, Partners).
Bottom Bar: Nút Play lớn, Changelog, Settings.
Custom Title Bar: Hỗ trợ drag, theme tối.
Loading Screen: Video animation + progress bar cho khởi tạo.
Notification: Badge cho pending updates, toast cho login.

5. Hỗ Trợ Mods & Servers

Mods: Tab hỗ trợ tải mods qua CurseForge (sắp tới).
Servers: Danh sách server tùy chỉnh, ping tự động.
Changelog: Hiển thị notes cập nhật qua WebView2.


📥 Hướng Dẫn Cài Đặt
Yêu Cầu Hệ Thống

Hệ điều hành:
Windows 10: Phiên bản tối thiểu 1803 (Build 17134) hoặc cao hơn (hỗ trợ tốt nhất từ 1903).
Windows 11: Phiên bản tối thiểu 21H2 (Build 22000) hoặc cao hơn.

CPU: Intel Core i3 hoặc tương đương (khuyến nghị i5/i7 cho modpack lớn).
RAM: Tối thiểu 4GB (khuyến nghị 8GB+ cho Minecraft).
Lưu trữ: 2GB trống cho launcher + 4GB+ cho Minecraft.
Đồ họa: Integrated Graphics (Intel HD 4000+) hoặc Discrete GPU (NVIDIA/AMD).
Java: Tự động tải Java 17+ (tích hợp OpenJDK).
.NET: Windows App SDK 1.4+ (tự động cài khi chạy installer).

Lưu ý: Launcher chỉ hỗ trợ Windows (không hỗ trợ macOS/Linux).
Bước Cài Đặt

Tải Launcher:
Truy cập GitHub Releases.
Tải file VoxelLauncher.exe (self-contained, không cần cài đặt).

Chạy Launcher:
Double-click VoxelLauncher.exe.
Nếu thiếu .NET hoặc WebView2, Windows sẽ tự động cài (chấp nhận prompt).

Đăng Nhập:
Chọn "Microsoft" cho tài khoản Premium (Xbox Live).
Chọn "Offline" cho chơi không cần tài khoản.

Chọn Phiên Bản & Chơi:
Chọn phiên bản Minecraft (ví dụ: 1.20.1).
Bấm "Play" – launcher sẽ tải tự động nếu thiếu.

Cập Nhật:
Launcher tự kiểm tra cập nhật khi khởi động.
Nếu có bản mới, dialog sẽ hiện với notes chi tiết.


Cài Đặt Thủ Công (nếu cần)

Java: Tải từ Adoptium (Temurin 17+).
Mods: Tải từ CurseForge, đặt vào .minecraft/mods.
Thư mục Minecraft:%APPDATA%\.minecraft (mặc định).

Khắc Phục Lỗi Thường Gặp:

Lỗi WebView2: Cài Microsoft Edge WebView2 Runtime.
Lỗi Java: Chạy java -version trong CMD để kiểm tra.
Lỗi Cập Nhật: Kiểm tra firewall/antivirus chặn GitHub.


⚙️ Hướng Dẫn Sử Dụng Nâng Cao
Quản Lý Phiên Bản

Tải Snapshot: Chọn phiên bản "snapshot" trong danh sách.
Tùy Chỉnh RAM: Sửa JVM args trong Settings (mặc định: -Xmx2G).
Server Favorites: Thêm server vào tab "Servers" để ping tự động.

Mods & Resource Packs

Mods: Sử dụng Fabric/Forge qua tab "Mods". Tải modpack từ CurseForge.
Resource Packs: Đặt vào .minecraft/resourcepacks.

Cập Nhật & Backup

Pending Updates: Nếu bỏ qua, badge sẽ hiện ở nút Notification.
Backup: Sao lưu .minecraft trước khi mod.

Troubleshooting

Launcher Treo: Kill process VoxelLauncher.exe trong Task Manager.
Không Tải Game: Kiểm tra kết nối internet, thử VPN nếu Mojang bị chặn.
Lỗi Đăng Nhập: Xóa ms_accounts.json trong .minecraft.


🔗 Liên Kết Hữu Ích

GitHub Repo:github.com/ShadowZa982/VoxelLauncher
Minecraft Wiki:minecraft.wiki
CurseForge Mods:curseforge.com/minecraft/mc-mods
Hỗ Trợ: Mở Issue trên GitHub hoặc Discord (sắp có).


📄 Giấy Phép & Góp Ý

License: MIT License (xem LICENSE file).
Góp Ý: Fork repo, submit PR hoặc mở Issue.
Đóng Góp: Star repo, chia sẻ với bạn bè!

Cảm ơn bạn đã sử dụng VoxelLauncher!
Phát triển bởi ShadowZa982 – Hẹn gặp lại ở phiên bản tiếp theo.
