# VoxelLauncher

**VoxelLauncher** là **launcher Minecraft Java Edition** được xây dựng bằng **WinUI 3** và **Windows App SDK**, sử dụng thư viện **[CmlLib.Core](https://github.com/CmlLib/CmlLib.Core)** để hỗ trợ đầy đủ các tính năng Minecraft chính thức.

> **Phát triển bởi:** [ShadowZa982](https://github.com/ShadowZa982)  
> **GitHub:** [ShadowZa982/VoxelLauncher](https://github.com/ShadowZa982/VoxelLauncher)

---

## **Hệ thống:** 
**Yêu cầu hệ thống:**  
- **Windows 10** (version **1803 trở lên**)  
- **Windows 11** (version **21H2 trở lên**)

---

## **Mô Tả Tổng Quan**

**VoxelLauncher** là **launcher miễn phí, mã nguồn mở**, giúp bạn chơi **Minecraft Java Edition** **một cách dễ dàng** mà **không cần tải thủ công** file từ Mojang.

### **Đặc điểm nổi bật**

- **Giao diện hiện đại** – WinUI 3, theme tối, animation mượt mà, sidebar điều hướng nhanh  
- **Hỗ trợ đa tài khoản** – Microsoft (Xbox Live) + Offline, lưu nhiều tài khoản, chuyển đổi nhanh  
- **Tải phiên bản tự động** – Hỗ trợ **tất cả phiên bản** từ `0.1.0` → `Mói nhất` (bao gồm snapshot, release, rc, old version, Pre-Release)
- **Tích họp loader `Fabric, Forger, Quilt, NeoFoger, Vanilla`
- **Tích hợp Java** – Tự động phát hiện, hỗ trợ **Java 8+**, tải **Java 17+** nếu thiếu  
- **Cập nhật tự động** – Kiểm tra GitHub Releases, tải ZIP + progress bar chi tiết  
- **Thông báo thông minh** – Toast khi đăng nhập, badge cho cập nhật bị bỏ qua  
- **Tùy chỉnh mạnh mẽ** – Sidebar (Mods, Servers, Changelog)
- **Bảo mật cao** – Lưu session an toàn, hỗ trợ **XboxAuth**

> **Không cần tài khoản Premium để chơi Offline**  
> **Cần Premium để chơi online với server chính thức**

---

## **Chức Năng Chính**

### 1. **Đăng Nhập & Quản Lý Tài Khoản**
- **Microsoft Account** – Xác thực Xbox Live qua **MSAL**, tự động đăng nhập  
- **Offline Mode** – Chơi không cần internet, tên tùy chỉnh  
- **Quản lý tài khoản** – Lưu nhiều tài khoản, xem avatar, thời gian đăng nhập, loại tài khoản  
- **Xóa tài khoản** – Dễ dàng xóa vĩnh viễn  
- **Thông báo** – Toast + avatar khi đăng nhập thành công

### 2. **Tải & Chạy Minecraft**
- **Danh sách phiên bản** – Tải từ Mojang, hiển thị **release + snapshot**  
- **Tải song song** – Dùng `GameInstaller`, tải nhanh assets, libraries, client  
- **Java tự động** – Phát hiện Java 8+, **tối thiểu Java 17** cho phiên bản mới  
- **Tùy chỉnh RAM** – Sửa `-Xmx`, JVM args trong Settings

### 3. **Cập Nhật Launcher**
- **Kiểm tra tự động**
- **Dialog cập nhật** – Hiển thị **chi tiết**  
- **Tải Cập nhật** – Progress bar (dung lượng, tốc độ KB/s), kiểm tra **tính toàn vẹn**  
- **Cài đặt** – Chạy `VoxelUpdater.exe`, tự động khởi động lại  
- **Pending Updates** – Bỏ qua → badge hiện, cài sau

### 4. **Giao Diện & Tùy Chỉnh**
- **Sidebar** – Menu trượt: **Info, Mods, Servers, Partners**  
- **Bottom Bar** – Nút **Play lớn**, Changelog, Settings  
- **Loading Screen** – Video animation + progress bar  
- **Notification** – Badge + toast

### 5. **Hỗ Trợ Mods & Servers**
- **Mods** – Tab tải mod qua **[modthrim](http://modrinth.com/)** có sẵn và **CurseForge** (sắp có)  
- **Servers** – Danh sách server, **ping tự động**  
- **Changelog** – Hiển thị notes cập nhật phiên bản minecraft 
---

## **Hướng Dẫn Cài Đặt**

### **Yêu Cầu Hệ Thống**
| Yêu cầu | Chi tiết |
|--------|--------|
| **Hệ điều hành** | Windows 10 (1803+) hoặc Windows 11 (21H2+) |
| **CPU** | Intel Core i3+ (khuyến nghị i5/i7) |
| **RAM** | Tối thiểu 4GB (khuyến nghị 8GB+) |
| **Lưu trữ** | 2GB (launcher) + 4GB+ (Minecraft) |
| **Đồ họa** | Intel HD 4000+ hoặc GPU rời |
| **Java** | Tự động tải **OpenJDK 17+** |
| **.NET** | Windows App SDK 1.4+ (tự cài) |

> **Chỉ hỗ trợ Windows** – Không hỗ trợ macOS/Linux

---

### **Bước Cài Đặt**

1. **Tải Launcher**  
   → Truy cập: [GitHub Releases](https://github.com/ShadowZa982/VoxelLauncher/releases/latest)  
   → Tải file: `VoxelLauncher.exe` (**self-contained**)

2. **Chạy Launcher**  
   → Double-click `VoxelLauncher.exe`  
   → Nếu thiếu **WebView2/.NET**, Windows sẽ tự động cài

3. **Đăng Nhập**  
   - **Microsoft** → Tài khoản Premium (Xbox Live)  
   - **Offline** → Chơi không cần tài khoản

4. **Chọn Phiên Bản & Chơi**  
   → Chọn `1.20.1` (ví dụ) → Bấm **Play**  
   → Launcher tự động tải nếu thiếu

5. **Cập Nhật**  
   → Tự động kiểm tra khi khởi động  
   → Nếu có bản mới → **dialog hiện ngay** với notes

---

### **Cài Đặt Thủ Công (nếu cần)**

| Mục | Hướng dẫn |
|-----|-----------|
| **Java** | Tải từ [Adoptium](https://adoptium.net/) (Temurin 17+) |
| **Mods** | Tải từ CurseForge hoặc Fabric, các loader khác → đặt vào `.minecraft/mods` |
| **Thư mục Minecraft** | `%APPDATA%\.minecraft` |

---

### **Khắc Phục Lỗi Thường Gặp**

| Lỗi | Cách khắc phục |
|-----|----------------|
| **WebView2 lỗi** | Cài [WebView2 Runtime](https://developer.microsoft.com/en-us/microsoft-edge/webview2/) |
| **Java lỗi** | Mở CMD → `java -version` |
| **Cập nhật lỗi** | Kiểm tra firewall/antivirus chặn GitHub |
| **Launcher treo** | Kill `VoxelLauncher.exe` trong Task Manager |
| **Không tải game** | Kiểm tra internet, thử VPN nếu Mojang bị chặn |
| **Lỗi đăng nhập** | Xóa `ms_accounts.json` trong `.minecraft` |

---

## **Hướng Dẫn Sử Dụng Nâng Cao**

### **Quản Lý Phiên Bản**
- **Tải Snapshot** → Chọn trong danh sách  
- **Tùy chỉnh RAM** → Sửa `-Xmx2G` trong Settings  
- **Server Favorites** → Thêm vào tab Servers → ping tự động

### **Mods & Resource Packs**
- **Mods** → Dùng Fabric/Forge → tải từ CurseForge hoặc Modrinth
- **Resource Packs** → Đặt vào `.minecraft/resourcepacks`

### **Cập Nhật & Backup**
- **Pending Updates** → Badge ở nút Notification  
- **Backup** → Sao lưu `.minecraft` trước khi mod

---

## **Liên Kết Hữu Ích**

- **GitHub Repo:** [github.com/ShadowZa982/VoxelLauncher](https://github.com/ShadowZa982/VoxelLauncher)  
- **Minecraft Wiki:** [minecraft.wiki](https://minecraft.wiki)  
- **CurseForge Mods:** [curseforge.com/minecraft/mc-mods](https://www.curseforge.com/minecraft/mc-mods)
- **Modrinth Mods:** [modrinth.com/mods](https://modrinth.com/mods)
- **Hỗ Trợ:** Mở Issue trên GitHub hoặc Discord [FoxStudio](https://discord.gg/ThEFtBxpRf)

---

## **Giấy Phép & Góp Ý**

- **License:** [MIT License](LICENSE)  
- **Góp Ý:** Fork repo → Submit PR hoặc mở Issue  
- **Đóng Góp:** **Star repo**, chia sẻ với bạn bè!

---

> **Cảm ơn bạn đã sử dụng VoxelLauncher!**  
> **Phát triển bởi ShadowZa982-FoxStudio** – Hẹn gặp lại ở phiên bản tiếp theo!

---
