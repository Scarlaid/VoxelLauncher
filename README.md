# VoxelLauncher

<img width="258" height="258" alt="serve_logor" src="https://github.com/user-attachments/assets/a8eaa9e6-644d-4165-a763-f745ee12cbed" />


**VoxelLauncher** là **launcher Minecraft Java Edition** được xây dựng bằng **WinUI 3** và **Windows App SDK**, sử dụng thư viện **[CmlLib.Core](https://github.com/CmlLib/CmlLib.Core)** để hỗ trợ đầy đủ các tính năng Minecraft chính thức.

> **Phát triển bởi:** [FoxStudio]([https://github.com/ShadowZa982](https://discord.gg/ThEFtBxpRf))  
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

<img width="1177" height="697" alt="{412C7C5B-620A-4B11-9655-CBAC18A1D416}" src="https://github.com/user-attachments/assets/6198b18c-3968-4814-914e-6afeccf32254" />


---

## **Chức Năng Chính**

### 1. **Đăng Nhập & Quản Lý Tài Khoản**
- **Microsoft Account** – Xác thực Xbox Live qua **MSAL**, tự động đăng nhập  
- **Offline Mode** – Chơi không cần internet, tên tùy chỉnh  
- **Quản lý tài khoản** – Lưu nhiều tài khoản, xem avatar, thời gian đăng nhập, loại tài khoản  
- **Xóa tài khoản** – Dễ dàng xóa vĩnh viễn  
- **Thông báo** – Toast + avatar khi đăng nhập thành công

  <img width="1182" height="701" alt="{B67E377A-B22A-4CB5-96C5-0AB5C4ADFB5A}" src="https://github.com/user-attachments/assets/844ae444-427e-4236-8c7b-c558a811a4ae" />

  <img width="1170" height="699" alt="{74E90BB9-E778-4AA6-800D-CB5146C411A8}" src="https://github.com/user-attachments/assets/2c7f8515-3e00-40d7-afbf-929862b1d75d" />



### 2. **Tải & Chạy Minecraft**
- **Danh sách phiên bản** – Tải từ Mojang, hiển thị **release + snapshot**  
- **Tải song song** – Dùng `GameInstaller`, tải nhanh assets, libraries, client  
- **Java tự động** – Phát hiện Java 8+, **tối thiểu Java 17** cho phiên bản mới  
- **Tùy chỉnh RAM** – Sửa `-Xmx`, JVM args trong Settings

  <img width="1174" height="700" alt="{50926480-4EA9-4416-AE9A-4BD674210943}" src="https://github.com/user-attachments/assets/6021e6d7-75af-46bd-8d0f-15064800a135" />

<img width="1172" height="690" alt="{905F850A-2E99-4B23-948D-40741E541F95}" src="https://github.com/user-attachments/assets/1a4b6487-0e1c-4b73-ac41-b7f935ea456a" />


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

  <img width="1175" height="696" alt="{6623C5BC-011E-458A-8F9B-3C2B6EB27A43}" src="https://github.com/user-attachments/assets/53968097-6482-47b1-ad1a-767fae940de1" />

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
