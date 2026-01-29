# 🖥️ Remote Desktop Services - GitHub Actions Workflow

<div align="center">

![GitHub Workflow](https://img.shields.io/badge/GitHub-Actions-2088FF?style=for-the-badge&logo=github-actions&logoColor=white)
![Windows](https://img.shields.io/badge/Windows-0078D6?style=for-the-badge&logo=windows&logoColor=white)
![Ubuntu](https://img.shields.io/badge/Ubuntu-E95420?style=for-the-badge&logo=ubuntu&logoColor=white)
![License](https://img.shields.io/badge/License-MIT-green.svg?style=for-the-badge)

**Triển khai Windows & Ubuntu Desktop với Remote Desktop Protocol (RDP) trên GitHub Actions**

[🚀 Bắt đầu](#-cài-đặt) • [📖 Hướng dẫn](#-hướng-dẫn-sử-dụng) • [⚙️ Cấu hình](#️-các-phiên-bản-hỗ-trợ) • [🔧 Khắc phục](#-khắc-phục-sự-cố) • [📞 Hỗ trợ](#-hỗ-trợ)

</div>

---

## 📋 Mục lục

- [✨ Tính năng](#-tính-năng)
- [🎯 Yêu cầu](#-yêu-cầu)
- [🚀 Cài đặt](#-cài-đặt)
- [📖 Hướng dẫn sử dụng](#-hướng-dẫn-sử-dụng)
- [⚙️ Các phiên bản hỗ trợ](#️-các-phiên-bản-hỗ-trợ)
- [🔐 Thông tin đăng nhập](#-thông-tin-đăng-nhập)
- [🌐 Kết nối RDP](#-kết-nối-rdp)
- [📊 Giám sát tiến trình](#-giám-sát-tiến-trình)
- [⏱️ Thời gian sử dụng](#️-thời-gian-sử-dụng)
- [🔧 Khắc phục sự cố](#-khắc-phục-sự-cố)
- [❓ FAQ](#-faq)
- [📝 Lưu ý quan trọng](#-lưu-ý-quan-trọng)
- [🤝 Đóng góp](#-đóng-góp)
- [📞 Hỗ trợ](#-hỗ-trợ)
- [📄 License](#-license)

---

## ✨ Tính năng

### 🎯 Điểm nổi bật

- ✅ **Đa nền tảng**: Hỗ trợ Windows Server (2012-2025), Windows 10/11, Ubuntu Desktop
- ✅ **Hiệu năng cao**: 4 vCPU với 8GB-16GB RAM tùy cấu hình
- ✅ **Kết nối nhanh**: Sử dụng Kami Tunnel cho kết nối RDP công khai
- ✅ **Web Viewer**: Theo dõi trực tiếp tiến trình cài đặt qua trình duyệt (port 8006)
- ✅ **Tự động hóa hoàn toàn**: Không cần cấu hình thủ công
- ✅ **Miễn phí**: Sử dụng GitHub Actions Runners miễn phí

### 🔥 Tính năng chi tiết

| Tính năng | Mô tả |
|-----------|-------|
| **Multiple OS** | Windows Server 2012/2019/2022/2025, Windows 10/11, Ubuntu 24.04 |
| **High Performance** | Native: 4 vCPU + 16GB RAM / Docker: 4 vCPU + 8GB RAM |
| **Public IP** | Tự động tạo IP công khai với Kami Tunnel |
| **Web Console** | Xem màn hình cài đặt Windows qua HTTP (port 8006) |
| **Auto Setup** | Tự động cài đặt RDP, tạo user, cấu hình firewall |
| **Long Session** | Thời gian chạy tối đa 6 giờ (360 phút) |

---

## 🎯 Yêu cầu

### Điều kiện tiên quyết

1. **Tài khoản GitHub**
   - Tài khoản GitHub (miễn phí hoặc Pro)
   - GitHub Actions phải được bật (mặc định bật)

2. **Repository**
   - Fork hoặc tạo repository mới
   - Thêm file workflow vào `.github/workflows/`

3. **Kiến thức cơ bản**
   - Hiểu biết cơ bản về GitHub Actions
   - Biết cách kết nối RDP (Remote Desktop)

### Giới hạn GitHub Actions

| Loại tài khoản | Thời gian/tháng | Đồng thời |
|----------------|-----------------|-----------|
| **Free** | 2,000 phút | 1 job |
| **Pro** | 3,000 phút | 5 jobs |
| **Team** | 10,000 phút | 15 jobs |
| **Enterprise** | 50,000 phút | 50 jobs |

> 💡 **Lưu ý**: Mỗi lần chạy tối đa 360 phút (6 giờ)

---

## 🚀 Cài đặt

### Bước 1: Fork Repository

```bash
# Truy cập repository
https://github.com/zun209384-lgtm/window

# Nhấn nút "Fork" ở góc phải trên
```

### Bước 2: Tạo file workflow

1. Truy cập repository của bạn
2. Vào thư mục `.github/workflows/`
3. Tạo file mới: `Windows.yml`
4. Copy nội dung từ file `Windows.yml` trong repo

### Bước 3: Commit và Push

```bash
git add .github/workflows/Windows.yml
git commit -m "Add RDP workflow"
git push origin main
```

### Bước 4: Kích hoạt workflow

1. Vào tab **Actions** trong repository
2. Chọn workflow **"🖥️ REMOTE DESKTOP SERVICES"**
3. Nhấn **"Run workflow"**

---

## 📖 Hướng dẫn sử dụng

### 🎬 Khởi chạy workflow

#### Phương pháp 1: Giao diện Web (Đề xuất)

1. **Truy cập repository GitHub của bạn**
   ```
   https://github.com/[username]/[repository]
   ```

2. **Chọn tab Actions**
   - Click vào tab "Actions" ở thanh menu trên cùng

3. **Chọn workflow**
   - Tìm và click vào "🖥️ REMOTE DESKTOP SERVICES"

4. **Khởi chạy**
   - Nhấn nút **"Run workflow"** (màu xanh)
   - Chọn hệ điều hành từ dropdown menu
   - Nhấn **"Run workflow"** để xác nhận

#### Phương pháp 2: GitHub CLI

```bash
# Cài đặt GitHub CLI (nếu chưa có)
# macOS/Linux
brew install gh

# Windows
winget install GitHub.cli

# Đăng nhập
gh auth login

# Chạy workflow
gh workflow run "Windows.yml" \
  -f os_version="Windows Server 2025 (Native - 4vCPU | 16GB RAM)"
```

### 📊 Theo dõi quá trình

1. **Xem log realtime**
   - Click vào workflow run đang chạy
   - Xem các step đang thực hiện

2. **Nhận thông tin kết nối**
   - Đợi step "🌐 Connection Information" hoàn thành
   - Copy thông tin IP, username, password

3. **Kết nối RDP**
   - Sử dụng thông tin vừa nhận để kết nối

---

## ⚙️ Các phiên bản hỗ trợ

### 🪟 Windows Systems

#### 1. Windows Server 2025 (Native)
```yaml
Configuration: 4 vCPU | 16GB RAM
Runner: windows-latest
Deployment: Native GitHub Runner
Boot Time: ~3-5 minutes
Best For: Production workloads, heavy tasks
```

**Đặc điểm:**
- ⚡ Hiệu năng cao nhất
- 🚀 Khởi động nhanh nhất
- 💪 RAM lớn nhất (16GB)
- ✅ Phù hợp công việc nặng

#### 2. Windows Server 2025 (Docker)
```yaml
Configuration: 4 vCPU | 8GB RAM
Runner: ubuntu-latest
Deployment: Docker (dockurr/windows)
Boot Time: ~10-15 minutes
Best For: Testing, development
Web Viewer: Port 8006 enabled
```

**Đặc điểm:**
- 🖥️ Xem tiến trình cài đặt qua web
- 🔧 Linh hoạt cấu hình
- 📦 Dễ dàng backup/restore
- ⏱️ Thời gian khởi động lâu hơn

#### 3. Windows Server 2022 (Docker)
```yaml
Configuration: 4 vCPU | 8GB RAM
Runner: ubuntu-latest
Deployment: Docker
Version: Windows Server 2022
Stability: Production Ready
```

#### 4. Windows Server 2019 (Docker)
```yaml
Configuration: 4 vCPU | 8GB RAM
Runner: ubuntu-latest
Deployment: Docker
Version: Windows Server 2019
LTS: Long Term Support
```

#### 5. Windows Server 2012 (Docker)
```yaml
Configuration: 4 vCPU | 8GB RAM
Runner: ubuntu-latest
Deployment: Docker
Version: Windows Server 2012 R2
Legacy: For compatibility testing
```

#### 6. Windows 11 Professional (Docker)
```yaml
Configuration: 4 vCPU | 8GB RAM
Runner: ubuntu-latest
Deployment: Docker
Version: Windows 11 Pro
UI: Modern Windows 11 interface
```

#### 7. Windows 10 Professional (Docker)
```yaml
Configuration: 4 vCPU | 8GB RAM
Runner: ubuntu-latest
Deployment: Docker
Version: Windows 10 Pro
UI: Classic Windows 10 interface
```

### 🐧 Linux Systems

#### 8. Ubuntu 24.04 Desktop RDP (Native)
```yaml
Configuration: 4 vCPU | 16GB RAM
Runner: ubuntu-latest
Desktop: XFCE4 (Lightweight)
Boot Time: ~5-7 minutes
Best For: Linux development, testing
```

**Đặc điểm:**
- 🖱️ Giao diện đồ họa XFCE4
- ⚡ Nhẹ và nhanh
- 🔧 Full Ubuntu Desktop experience
- 💻 16GB RAM cho development

---

## 🔐 Thông tin đăng nhập

### Windows (Tất cả phiên bản)

| Thuộc tính | Giá trị |
|------------|---------|
| **Username** | `Admin` |
| **Password** | `Window@123456` |
| **User Type** | Administrator |
| **Access Level** | Full Control |

### Ubuntu Desktop RDP

| Thuộc tính | Giá trị |
|------------|---------|
| **Username** | `Admin` |
| **Password** | `Ubuntu@123456` |
| **User Type** | Sudo User |
| **Access Level** | Root Access |

> ⚠️ **Cảnh báo bảo mật**: Đây là thông tin đăng nhập mặc định. Không sử dụng cho môi trường production thực tế!

---

## 🌐 Kết nối RDP

### Windows (Remote Desktop Connection)

#### Cách 1: Sử dụng Remote Desktop Connection

1. **Mở Remote Desktop Connection**
   - Nhấn `Windows + R`
   - Gõ `mstsc` và Enter
   - Hoặc tìm "Remote Desktop Connection" trong Start Menu

2. **Nhập thông tin**
   ```
   Computer: [IP từ workflow log]
   Example: 123.45.67.89:3389
   ```

3. **Kết nối**
   - Click "Connect"
   - Nhập username: `Admin`
   - Nhập password: `Window@123456`
   - Click "OK"

#### Cách 2: Sử dụng Command Line

```cmd
mstsc /v:123.45.67.89:3389 /admin
```

### macOS (Microsoft Remote Desktop)

1. **Cài đặt ứng dụng**
   - Download từ Mac App Store: "Microsoft Remote Desktop"
   - Hoặc sử dụng: `brew install --cask microsoft-remote-desktop`

2. **Thêm PC mới**
   - Mở Microsoft Remote Desktop
   - Click "+" → "Add PC"
   - PC name: `[IP]:[Port]` (ví dụ: `123.45.67.89:3389`)
   - User account: Add new
     - Username: `Admin`
     - Password: `Window@123456`

3. **Kết nối**
   - Double-click vào PC vừa thêm

### Linux (Remmina / Rdesktop)

#### Sử dụng Remmina (Giao diện đồ họa)

```bash
# Cài đặt Remmina
sudo apt update
sudo apt install remmina remmina-plugin-rdp

# Chạy Remmina
remmina
```

Trong Remmina:
- Protocol: RDP
- Server: `123.45.67.89:3389`
- Username: `Admin`
- Password: `Window@123456`

#### Sử dụng Rdesktop (Command line)

```bash
# Cài đặt
sudo apt install rdesktop

# Kết nối
rdesktop -u Admin -p Window@123456 123.45.67.89:3389 -g 1920x1080 -a 32
```

**Tham số:**
- `-u`: Username
- `-p`: Password
- `-g`: Độ phân giải (width x height)
- `-a`: Color depth (bits)

#### Sử dụng FreeRDP (Nâng cao)

```bash
# Cài đặt
sudo apt install freerdp2-x11

# Kết nối
xfreerdp /u:Admin /p:Window@123456 /v:123.45.67.89:3389 /size:1920x1080 /cert:ignore
```

### Mobile (iOS / Android)

#### iOS (Microsoft Remote Desktop)

1. Download "Microsoft Remote Desktop" từ App Store
2. Tap "+" → "Add PC"
3. Nhập thông tin:
   - PC name: `[IP]:[Port]`
   - User account: `Admin` / `Window@123456`
4. Tap vào PC để kết nối

#### Android (Microsoft Remote Desktop / RD Client)

1. Download "Microsoft Remote Desktop" từ Google Play
2. Tap "+" → "Desktop"
3. Nhập thông tin:
   - PC name: `[IP]:[Port]`
   - User name: `Admin`
   - Password: `Window@123456`
4. Tap "Save" và kết nối

---

## 📊 Giám sát tiến trình

### 🖥️ Web Viewer (Chỉ Docker Windows)

Web Viewer cho phép bạn xem trực tiếp màn hình cài đặt Windows qua trình duyệt.

#### Cách sử dụng

1. **Lấy URL Web Viewer**
   - Từ workflow log, tìm dòng:
   ```
   🖥️  Web Viewer  : http://123.45.67.89:8006
   ```

2. **Truy cập qua trình duyệt**
   ```
   http://[IP]:8006
   ```

3. **Xem tiến trình**
   - BIOS screen
   - Windows boot logo
   - Installation progress
   - Setup screens

#### Tính năng Web Viewer

- 🎥 **Real-time screen**: Xem màn hình thời gian thực
- ⌨️ **Keyboard input**: Gửi lệnh keyboard nếu cần
- 🖱️ **Mouse control**: Điều khiển chuột từ xa
- 📸 **Screenshot**: Chụp màn hình hiện tại

#### Lợi ích

- ✅ Kiểm tra Windows đã boot xong chưa
- ✅ Debug các vấn đề khi cài đặt
- ✅ Không cần đợi RDP ready
- ✅ Xem được ngay từ lúc bắt đầu boot

### 📋 Workflow Logs

#### Xem logs trong GitHub Actions

1. **Truy cập workflow run**
   - Tab Actions → Click vào run đang chạy

2. **Xem từng step**
   - Click vào job (vd: `windows-docker`)
   - Click vào step để xem chi tiết

3. **Tìm thông tin kết nối**
   - Tìm step "🌐 Connection Information"
   - Copy IP, username, password

#### Log format mẫu

```
╔════════════════════════════════════════════════════════════╗
║         ✅ WINDOWS SERVER 2025 - READY FOR CONNECTION      ║
╠════════════════════════════════════════════════════════════╣
║ 🌐  RDP IP      : 123.45.67.89:3389
║ 🖥️  Web Viewer  : http://123.45.67.89:8006
║ 👤  Username    : Admin
║ 🔐  Password    : Window@123456
║ 📍  RDP Port    : 3389
║ 🌍  Web Port    : 8006 (Installation Progress)
║ 💻  Resources   : 4 vCPU | 8GB RAM
╚════════════════════════════════════════════════════════════╝

💡 Tip: Access Web Viewer to see Windows installation progress!
```

---

## ⏱️ Thời gian sử dụng

### Timeline chi tiết

#### Windows Server 2025 (Native)

```
00:00 - Khởi tạo workflow
00:01 - Tạo user Admin
00:02 - Cấu hình RDP service
00:03 - Setup Kami Tunnel
00:04 - Lấy Public IP
00:05 - Sẵn sàng kết nối ✅
...
05:40 - Workflow tự động dừng (timeout)
```

**Total runtime**: ~5 giờ 40 phút (340 phút)

#### Windows Docker Versions

```
00:00 - Khởi tạo workflow
00:01 - Pull Docker image
00:05 - Start Windows container
00:10 - Windows booting
00:15 - Windows setup
00:20 - RDP ready ✅
00:20 - Web Viewer available (port 8006)
...
05:40 - Workflow tự động dừng
```

**Total runtime**: ~5 giờ 20 phút (320 phút sử dụng thực tế)

#### Ubuntu Desktop RDP

```
00:00 - Khởi tạo workflow
00:02 - Cài đặt XFCE Desktop
00:04 - Cài đặt XRDP
00:05 - Tạo user Admin
00:06 - Setup Kami Tunnel
00:07 - Sẵn sàng kết nối ✅
...
05:40 - Workflow tự động dừng
```

**Total runtime**: ~5 giờ 33 phút (333 phút sử dụng thực tế)

### Gia hạn thời gian

Mặc định workflow chạy 6 giờ (360 phút). Để thay đổi:

```yaml
jobs:
  windows-server-2025-native:
    timeout-minutes: 360  # Thay đổi số này (tối đa 360 cho free tier)
```

> ⚠️ **Lưu ý**: GitHub Actions free tier giới hạn tối đa 6 giờ/workflow

---

## 🔧 Khắc phục sự cố

### ❌ Các vấn đề thường gặp

#### 1. Không thể lấy được IP

**Triệu chứng:**
```
🔄 Đang kiểm tra tín hiệu từ Windows Server...
(Lặp lại không có IP)
```

**Nguyên nhân:**
- Kami Tunnel không khởi động thành công
- Network bị chặn
- Port 3389 bị block

**Giải pháp:**

```bash
# Kiểm tra Kami Tunnel log
cat kami_tunnel.txt

# Thử khởi động lại tunnel
./kami-tunnel 3389
```

**Workaround:**
- Cancel workflow và chạy lại
- Thử phiên bản khác (Native → Docker hoặc ngược lại)

#### 2. RDP Connection Failed

**Triệu chứng:**
```
Remote Desktop can't connect to the remote computer
```

**Nguyên nhân:**
- IP sai hoặc hết hạn
- Port 3389 bị firewall chặn
- Windows chưa khởi động xong

**Giải pháp:**

1. **Kiểm tra IP còn hoạt động:**
   ```bash
   ping [IP]
   ```

2. **Test kết nối port:**
   ```bash
   telnet [IP] 3389
   # hoặc
   nc -zv [IP] 3389
   ```

3. **Đợi thêm vài phút:**
   - Docker Windows cần 10-15 phút để boot hoàn toàn
   - Kiểm tra Web Viewer (port 8006) xem Windows đã boot xong chưa

4. **Kiểm tra firewall local:**
   ```cmd
   # Windows
   netsh advfirewall show allprofiles
   
   # Tạm tắt firewall (test only)
   netsh advfirewall set allprofiles state off
   ```

#### 3. Authentication Failed

**Triệu chững:**
```
Your credentials did not work
Login attempt failed
```

**Nguyên nhân:**
- Username/password sai
- User chưa được tạo
- Network Level Authentication (NLA) enabled

**Giải pháp:**

1. **Kiểm tra thông tin đăng nhập:**
   - Username: `Admin` (chữ A viết hoa)
   - Password: `Window@123456` (cho Windows)
   - Password: `Ubuntu@123456` (cho Ubuntu)

2. **Tắt NLA (từ client):**
   
   **Windows:**
   - Mở Remote Desktop Connection
   - Show Options → Advanced
   - Connect even if authentication fails

   **Linux (FreeRDP):**
   ```bash
   xfreerdp /u:Admin /p:Window@123456 /v:[IP]:3389 /cert:ignore +auth-only
   ```

#### 4. Docker Container Failed

**Triệu chứng:**
```
Error response from daemon: failed to create shim task
```

**Nguyên nhân:**
- `/dev/kvm` không khả dụng
- Docker resources không đủ
- Image pull failed

**Giải pháp:**

1. **Kiểm tra KVM:**
   ```bash
   ls -la /dev/kvm
   sudo chmod 666 /dev/kvm  # Nếu cần
   ```

2. **Restart Docker:**
   ```bash
   sudo systemctl restart docker
   docker system prune -a  # Dọn dẹp
   ```

3. **Pull image thủ công:**
   ```bash
   docker pull dockurr/windows:latest
   ```

#### 5. Workflow Timeout

**Triệu chứng:**
```
The job running on runner has exceeded the maximum execution time of 360 minutes.
```

**Nguyên nhân:**
- Workflow chạy quá 6 giờ
- Step bị treo

**Giải pháp:**

1. **Cancel và chạy lại**
2. **Giảm timeout nếu chỉ test:**
   ```yaml
   timeout-minutes: 60  # 1 giờ
   ```

#### 6. Web Viewer không truy cập được

**Triệu chứng:**
```
ERR_CONNECTION_REFUSED khi truy cập http://[IP]:8006
```

**Nguyên nhân:**
- Port 8006 chưa được expose
- Kami Tunnel cho port 8006 chưa chạy
- Docker container chưa publish port

**Giải pháp:**

1. **Kiểm tra Docker ports:**
   ```bash
   docker ps
   # Kiểm tra xem có port 8006 không
   ```

2. **Kiểm tra Kami Tunnel:**
   ```bash
   cat kami_tunnel_web.txt
   ps aux | grep kami-tunnel
   ```

3. **Restart tunnel:**
   ```bash
   pkill kami-tunnel
   ./kami-tunnel 8006 > kami_tunnel_web.txt 2>&1 &
   ```

### 🔍 Debug logs

#### Xem Docker logs

```bash
# Xem logs container
docker logs windows_rdp

# Follow logs realtime
docker logs -f windows_rdp

# Xem 100 dòng cuối
docker logs --tail 100 windows_rdp
```

#### Xem Kami Tunnel logs

```bash
# RDP tunnel
cat kami_tunnel.txt
cat kami_tunnel_rdp.txt

# Web viewer tunnel
cat kami_tunnel_web.txt
```

#### Kiểm tra network

```bash
# List ports đang listen
netstat -tuln | grep -E '3389|8006'

# Kiểm tra routing
ip route

# Test connection
curl -v telnet://[IP]:3389
curl -v http://[IP]:8006
```

---

## ❓ FAQ

### Câu hỏi thường gặp

#### 1. Có mất phí không?

**Trả lời:** GitHub Actions free tier cung cấp:
- **2,000 phút/tháng** cho tài khoản Free
- **3,000 phút/tháng** cho tài khoản Pro

Mỗi lần chạy tốn ~6 giờ = 360 phút. Vậy bạn có thể chạy:
- Free: ~5-6 lần/tháng
- Pro: ~8-9 lần/tháng

> 💰 **Totally FREE** nếu sử dụng trong giới hạn!

#### 2. Có thể chạy 24/7 không?

**Trả lời:** Không. GitHub Actions có giới hạn:
- Tối đa 6 giờ/workflow
- Sau 6 giờ sẽ tự động timeout

**Workaround:**
- Chạy lại workflow sau khi timeout
- Sử dụng nhiều repository khác nhau
- Nâng cấp lên GitHub Team/Enterprise

#### 3. IP có thay đổi mỗi lần chạy không?

**Trả lời:** Có. Mỗi lần chạy workflow sẽ có:
- IP mới từ Kami Tunnel
- Machine mới từ GitHub Runners
- Tất cả dữ liệu sẽ bị xóa sau khi kết thúc

**Lưu trữ dữ liệu:**
- Sử dụng GitHub Artifacts để lưu files
- Upload lên cloud storage (Google Drive, Dropbox)
- Commit và push về repository

#### 4. Có thể cài đặt phần mềm không?

**Trả lời:** Có, bạn có full quyền Administrator:
- Cài đặt bất kỳ phần mềm nào
- Thay đổi cấu hình hệ thống
- Chạy scripts, applications

**Lưu ý:**
- Dữ liệu sẽ mất sau khi workflow kết thúc
- Không lưu trữ dữ liệu nhạy cảm

#### 5. Có thể truy cập Internet không?

**Trả lời:** 

**Windows Native:** ✅ Có, full internet access
**Windows Docker:** ⚠️ Có giới hạn:
- HTTP/HTTPS: ✅ Hoạt động
- Browsing: ✅ Hoạt động  
- Download: ✅ Hoạt động
- Một số ports có thể bị chặn

**Ubuntu Desktop:** ✅ Full internet access

#### 6. Có an toàn không?

**Trả lời:** 

**Bảo mật:**
- ✅ Chạy trên GitHub infrastructure
- ✅ Isolated environment
- ✅ Data tự động xóa sau khi chạy
- ⚠️ Không sử dụng cho production data
- ⚠️ Không lưu mật khẩu/keys nhạy cảm

**Best Practices:**
- Đổi password mặc định nếu cần
- Không commit sensitive data
- Sử dụng GitHub Secrets cho credentials
- Review logs trước khi public repository

#### 7. Có thể chơi game không?

**Trả lời:** 

**Windows Native:** 
- ❌ Không có GPU
- ❌ Graphics performance thấp
- ✅ Có thể chơi game nhẹ, cũ

**Windows Docker:**
- ❌ Không hỗ trợ GPU passthrough
- ❌ Không phù hợp cho gaming

**Khuyến nghị:**
- Chỉ dùng cho công việc, testing, development
- Không dùng cho gaming hay đồ họa nặng

#### 8. Có giới hạn băng thông không?

**Trả lời:** 

GitHub Actions có giới hạn:
- Network I/O trong limits hợp lý
- Không giới hạn cụ thể về bandwidth
- Có thể download/upload files bình thường

**Lưu ý:**
- Không abuse network
- Không dùng cho torrenting, mining
- Không dùng cho hosting services

#### 9. Có thể dùng cho mining không?

**Trả lời:** ❌ **TUYỆT ĐỐI KHÔNG**

Theo GitHub Terms of Service:
- ❌ Mining cryptocurrency là vi phạm
- ❌ Tài khoản sẽ bị ban vĩnh viễn
- ❌ Mất tất cả repositories

**Cho phép:**
- ✅ Development và testing
- ✅ CI/CD pipelines
- ✅ Automated testing
- ✅ Learning và education

#### 10. Làm sao để kéo dài thời gian?

**Trả lời:** 

Không thể vượt quá 6 giờ, nhưng có thể:

**Method 1: Auto re-run**
```yaml
# Sử dụng cron schedule
on:
  schedule:
    - cron: '0 */6 * * *'  # Chạy mỗi 6 giờ
```

**Method 2: Multiple repos**
- Tạo nhiều repos khác nhau
- Chạy luân phiên

**Method 3: Manual restart**
- Sau 6 giờ, manually chạy lại

> ⚠️ Nhưng nhớ: Dữ liệu sẽ mất mỗi lần restart!

---

## 📝 Lưu ý quan trọng

### ⚠️ Cảnh báo

#### 1. Giới hạn sử dụng

```
❌ KHÔNG SỬ DỤNG CHO:
- Cryptocurrency mining
- Torrenting / P2P file sharing
- Hosting production websites
- DDoS attacks
- Spam / phishing
- Illegal activities

✅ SỬ DỤNG CHO:
- Software development & testing
- Learning & education
- CI/CD pipelines
- Temporary workspaces
- Demo & proof of concepts
```

#### 2. Dữ liệu

- 🗑️ **Mọi dữ liệu sẽ bị XÓA** sau khi workflow kết thúc
- 💾 Không lưu trữ dữ liệu quan trọng
- ☁️ Upload lên cloud nếu cần lưu

#### 3. Bảo mật

- 🔐 Đổi password mặc định trong môi trường thực
- 🔒 Không commit sensitive data vào repo
- 🛡️ Sử dụng GitHub Secrets cho credentials
- 👀 Review logs trước khi public repo

#### 4. Performance

- ⚡ Windows Native nhanh hơn Docker
- 🐌 Docker cần 10-15 phút để boot
- 🖥️ Không có GPU - không phù hợp đồ họa nặng
- 💻 4 vCPU + 8-16GB RAM - phù hợp công việc văn phòng

#### 5. Network

- 🌐 Internet access available
- 🔌 Một số ports có thể bị restrict
- 📶 Bandwidth trong giới hạn hợp lý
- 🚫 Không abuse network resources

### 📌 Best Practices

#### 1. Tối ưu hóa thời gian

```yaml
# Giảm timeout cho testing
timeout-minutes: 60  # 1 giờ thay vì 6 giờ

# Sử dụng cache
- uses: actions/cache@v3
  with:
    path: ~/cache
    key: ${{ runner.os }}-cache
```

#### 2. Backup dữ liệu

```yaml
# Upload files trước khi kết thúc
- name: Upload workspace
  uses: actions/upload-artifact@v3
  with:
    name: workspace-backup
    path: |
      ~/**
      !~/.cache
```

#### 3. Monitoring

```yaml
# Gửi thông báo khi hoàn thành
- name: Send notification
  if: always()
  uses: actions/github-script@v6
  with:
    script: |
      github.rest.issues.createComment({
        issue_number: context.issue.number,
        owner: context.repo.owner,
        repo: context.repo.repo,
        body: '✅ Workflow completed!'
      })
```

#### 4. Cost optimization

```yaml
# Chỉ chạy khi có tag
on:
  push:
    tags:
      - 'v*'

# Hoặc manual dispatch only
on:
  workflow_dispatch:
```

### 🎯 Use Cases

#### ✅ Phù hợp cho

- 🧪 **Testing & QA**
  - Test ứng dụng Windows
  - Browser testing
  - Compatibility testing

- 💻 **Development**
  - Remote development environment
  - Build Windows applications
  - Package testing

- 📚 **Learning & Training**
  - Windows Server administration
  - RDP tutorials
  - PowerShell scripting

- 🔬 **Research & POC**
  - Proof of concepts
  - Security research (ethical)
  - Performance benchmarking

#### ❌ Không phù hợp cho

- 🎮 **Gaming** - Không có GPU
- ⛏️ **Mining** - Bị cấm và ban account
- 🌐 **Production hosting** - Không stable
- 💾 **Long-term storage** - Dữ liệu bị xóa
- 📹 **Media encoding** - Performance thấp

---

## 🤝 Đóng góp

### Cách đóng góp

Chúng tôi hoan nghênh mọi đóng góp! 

#### 1. Fork repository

```bash
# Fork qua GitHub UI hoặc
gh repo fork zun209384-lgtm/window
```

#### 2. Tạo branch mới

```bash
git checkout -b feature/your-feature-name
```

#### 3. Commit changes

```bash
git add .
git commit -m "Add: your feature description"
```

#### 4. Push và tạo Pull Request

```bash
git push origin feature/your-feature-name
# Tạo PR trên GitHub
```

### Coding Standards

- ✅ Sử dụng YAML format chuẩn
- ✅ Comment rõ ràng cho code phức tạp
- ✅ Test trước khi submit PR
- ✅ Update documentation nếu cần

### Ideas for contribution

- 🎨 Cải thiện UI/UX của logs
- ⚡ Tối ưu thời gian boot
- 🔧 Thêm configuration options
- 📝 Cải thiện documentation
- 🐛 Fix bugs
- 🆕 Thêm OS versions mới

---

## 📞 Hỗ trợ

### 💬 Kênh hỗ trợ

#### GitHub Issues (Khuyến nghị)

Tạo issue mới tại: https://github.com/zun209384-lgtm/window/issues

**Template:**
```markdown
**Describe the issue**
Mô tả chi tiết vấn đề

**To Reproduce**
Các bước để reproduce:
1. Go to '...'
2. Click on '...'
3. See error

**Expected behavior**
Hành vi mong đợi

**Screenshots**
Nếu có, attach screenshots

**Environment:**
- OS Version: [e.g. Windows Server 2025]
- Runner: [e.g. windows-latest]
- Browser: [e.g. Chrome 120]

**Additional context**
Thông tin thêm
```

#### Discussions

Tham gia thảo luận: https://github.com/zun209384-lgtm/window/discussions

- 💡 Ý tưởng mới
- ❓ Q&A
- 📢 Announcements

### 🐛 Báo cáo lỗi

Khi báo cáo lỗi, hãy bao gồm:

1. **Workflow run URL**
   ```
   https://github.com/[user]/[repo]/actions/runs/[run_id]
   ```

2. **Logs liên quan**
   - Copy relevant logs từ workflow
   - Include error messages

3. **Steps to reproduce**
   - OS version đã chọn
   - Các bước đã thực hiện
   - Kết quả mong đợi vs thực tế

4. **Environment**
   - GitHub account type (Free/Pro)
   - Repository visibility (Public/Private)
   - Region (nếu biết)

### 📧 Contact

- **Creator**: Zun
- **Repository**: https://github.com/zun209384-lgtm/window
- **Issues**: https://github.com/zun209384-lgtm/window/issues

---

## 📄 License

```
MIT License

Copyright (c) 2024 Zun

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
```

### Giải thích License

**Bạn được phép:**
- ✅ Sử dụng thương mại
- ✅ Sửa đổi
- ✅ Phân phối
- ✅ Sử dụng riêng tư

**Điều kiện:**
- 📄 Phải giữ license và copyright notice
- 📝 Changes phải được document

**Giới hạn:**
- ⚠️ Không có warranty
- ⚠️ Tác giả không chịu trách nhiệm

---

## 🙏 Credits

### Công cụ và dịch vụ

- **GitHub Actions** - CI/CD platform
- **Kami Tunnel** - Public IP tunneling
- **Dockurr/Windows** - Windows Docker images
- **Microsoft** - Windows và RDP protocol
- **Canonical** - Ubuntu Linux

### Cảm ơn

Cảm ơn tất cả contributors và users đã support project! 🎉

---

## 📊 Stats

![GitHub stars](https://img.shields.io/github/stars/zun209384-lgtm/window?style=social)
![GitHub forks](https://img.shields.io/github/forks/zun209384-lgtm/window?style=social)
![GitHub issues](https://img.shields.io/github/issues/zun209384-lgtm/window)
![GitHub pull requests](https://img.shields.io/github/issues-pr/zun209384-lgtm/window)
![GitHub last commit](https://img.shields.io/github/last-commit/zun209384-lgtm/window)

---

## 🗺️ Roadmap

### Coming Soon

- [ ] 🔐 Mã hóa kết nối nâng cao
- [ ] 📱 Mobile app support
- [ ] 🌍 Multi-region deployment
- [ ] 💾 Cloud storage integration
- [ ] 🤖 Auto-restart on timeout
- [ ] 📊 Usage dashboard
- [ ] 🎨 Custom themes
- [ ] 🔔 Notification system

### Under Consideration

- [ ] macOS support
- [ ] GPU passthrough (nếu GitHub hỗ trợ)
- [ ] Custom ISO support
- [ ] Snapshot/backup features
- [ ] Load balancing
- [ ] Team collaboration features

---

<div align="center">

**⭐ Star this repository nếu bạn thấy hữu ích! ⭐**

Made with ❤️ by [Zun](https://github.com/zun209384-lgtm)

[⬆ Về đầu trang](#️-remote-desktop-services---github-actions-workflow)

</div>
