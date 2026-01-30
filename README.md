# 🖥️ Remote Desktop Services - GitHub Actions Workflow

<div align="center">

![Version](https://img.shields.io/badge/Version-2.0-blue?style=for-the-badge)
![License](https://img.shields.io/badge/License-Proprietary-red?style=for-the-badge)
![Status](https://img.shields.io/badge/Status-Production-green?style=for-the-badge)
![Platform](https://img.shields.io/badge/Platform-GitHub%20Actions-2088FF?style=for-the-badge&logo=github-actions)

**🚀 Triển khai Windows & Ubuntu Desktop với Remote Desktop Protocol (RDP) trên GitHub Actions**

**⚠️ PHIÊN BẢN CHÍNH THỨC - BẢN QUYỀN BẢO HỘ**

[📖 Hướng dẫn](#-hướng-dẫn-sử-dụng) • [⚡ Cài đặt](#-cài-đặt-nhanh) • [🔐 Bản quyền](#-thông-báo-bản-quyền) • [⚠️ Cảnh báo](#️-cảnh-báo-quan-trọng) • [📞 Hỗ trợ](#-hỗ-trợ)

</div>

---

## 🔐 **THÔNG BÁO BẢN QUYỀN**

```
╔════════════════════════════════════════════════════════════════════════╗
║                    ⚠️  COPYRIGHT NOTICE  ⚠️                            ║
╠════════════════════════════════════════════════════════════════════════╣
║                                                                        ║
║  📜 COPYRIGHT © 2024-2026 ZUN209384-LGTM                              ║
║  🏢 ALL RIGHTS RESERVED                                                ║
║                                                                        ║
║  Phần mềm này được bảo hộ bởi luật bản quyền quốc tế.                ║
║  Việc sao chép, phân phối, sửa đổi hoặc sử dụng không được phép      ║
║  là NGHIÊM CẤM và có thể dẫn đến hậu quả pháp lý nghiêm trọng.       ║
║                                                                        ║
╚════════════════════════════════════════════════════════════════════════╝
```

### 📋 **Điều khoản sử dụng**

#### ✅ **ĐƯỢC PHÉP:**

<table>
<tr>
<th>Hành động</th>
<th>Điều kiện</th>
</tr>
<tr>
<td>✅ Sử dụng cá nhân</td>
<td>Cho mục đích học tập, testing, development</td>
</tr>
<tr>
<td>✅ Fork repository</td>
<td>Giữ nguyên thông báo bản quyền và credits</td>
</tr>
<tr>
<td>✅ Chia sẻ link</td>
<td>Link đến repository gốc, không reupload</td>
</tr>
<tr>
<td>✅ Báo cáo lỗi</td>
<td>Qua GitHub Issues chính thức</td>
</tr>
<tr>
<td>✅ Đề xuất cải tiến</td>
<td>Qua Pull Requests với credit đầy đủ</td>
</tr>
</table>

#### ❌ **NGHIÊM CẤM:**

<table>
<tr>
<th>Hành động</th>
<th>Hậu quả</th>
</tr>
<tr>
<td>❌ Xóa/thay đổi thông tin bản quyền</td>
<td>Vi phạm DMCA - Report tức thì</td>
</tr>
<tr>
<td>❌ Sửa đổi code và claim là của bạn</td>
<td>Vi phạm bản quyền - Khóa repository</td>
</tr>
<tr>
<td>❌ Phân phối thương mại</td>
<td>Yêu cầu license - Pháp lý nếu vi phạm</td>
</tr>
<tr>
<td>❌ Reupload lên platform khác</td>
<td>DMCA Takedown - Khóa tài khoản</td>
</tr>
<tr>
<td>❌ Xóa credits/attribution</td>
<td>Vi phạm nghiêm trọng - Pháp lý</td>
</tr>
</table>

### 🏛️ **Bảo vệ pháp lý**

```
Workflow này được bảo hộ bởi:

📜 DMCA (Digital Millennium Copyright Act)
   → Mọi vi phạm sẽ bị report và takedown tức thì

🌐 Berne Convention
   → Bản quyền tự động có hiệu lực quốc tế

⚖️ GitHub Terms of Service
   → Vi phạm bản quyền = Khóa repository/account

🔒 Intellectual Property Rights
   → Code, design, documentation đều được bảo hộ
```

### 📝 **Cách sử dụng hợp pháp**

**Bước 1: Fork với credits đầy đủ**
```bash
# Fork repository từ GitHub UI
# KHÔNG được xóa/thay đổi thông báo bản quyền trong README
# KHÔNG được xóa credits trong code comments
```

**Bước 2: Giữ nguyên attribution**
```yaml
# ❌ KHÔNG XÓA các dòng comment này:
# Copyright © 2024-2026 Zun209384-lgtm
# Original: https://github.com/zun209384-lgtm/window
# All rights reserved

# ✅ PHẢI GIỮ NGUYÊN trong mọi phiên bản fork
```

**Bước 3: Link về repository gốc**
```markdown
# Trong README của bạn, PHẢI có:

## Credits
This project is forked from [zun209384-lgtm/window](https://github.com/zun209384-lgtm/window)

Original Author: [Zun209384-lgtm](https://github.com/zun209384-lgtm)

All rights reserved to the original author.
```

---

## ⚠️ **CẢNH BÁO QUAN TRỌNG**

### 🚨 **CẢNH BÁO BẢO MẬT VÀ PHÁP LÝ**

```
╔════════════════════════════════════════════════════════════════════════╗
║                  ⚠️  CRITICAL WARNINGS  ⚠️                             ║
╠════════════════════════════════════════════════════════════════════════╣
║                                                                        ║
║  🔴 KHÔNG SỬA ĐỔI FILE .YML WORKFLOW NẾU KHÔNG HIỂU RÕ                ║
║     → Có thể gây lỗi nghiêm trọng hoặc vi phạm bản quyền              ║
║                                                                        ║
║  🔴 KHÔNG XÓA/THAY ĐỔI THÔNG BÁO BẢN QUYỀN                            ║
║     → Vi phạm DMCA, sẽ bị report và takedown                          ║
║                                                                        ║
║  🔴 KHÔNG SỬ DỤNG CHO MỤC ĐÍCH BẤT HỢP PHÁP                            ║
║     → Mining, hacking, spam, DDoS, illegal activities                 ║
║     → GitHub sẽ khóa account vĩnh viễn                                ║
║                                                                        ║
║  🔴 KHÔNG LƯU TRỮ DỮ LIỆU NHẠY CẢM                                     ║
║     → Mọi dữ liệu sẽ BỊ XÓA sau 6 giờ                                 ║
║     → Không có backup, không thể khôi phục                            ║
║                                                                        ║
║  🔴 KHÔNG CHIA SẺ IP CÔNG KHAI VỚI NGƯỜI LẠ                            ║
║     → Password mặc định ai cũng biết                                  ║
║     → Có thể bị truy cập trái phép                                    ║
║                                                                        ║
╚════════════════════════════════════════════════════════════════════════╝
```

### ⛔ **NGHIÊM CẤM TUYỆT ĐỐI**

| Hành vi | Hậu quả | Mức độ nghiêm trọng |
|---------|---------|---------------------|
| **Cryptocurrency Mining** | Ban account GitHub vĩnh viễn | 🔴 CRITICAL |
| **DDoS / Network attacks** | Report lên GitHub + Police | 🔴 CRITICAL |
| **Hosting malware/virus** | Legal action + Account ban | 🔴 CRITICAL |
| **Spam / Phishing operations** | Permanent ban | 🔴 CRITICAL |
| **Torrenting / P2P sharing** | Account suspension | 🟠 HIGH |
| **Running game servers** | Waste resources - Warning | 🟡 MEDIUM |
| **Production website hosting** | Against ToS - Warning | 🟡 MEDIUM |

### 🛡️ **GitHub Actions - Terms of Service**

```
Bạn PHẢI tuân thủ GitHub Actions Usage Limits:

✅ ĐƯỢC PHÉP:
   • Development & testing
   • CI/CD pipelines
   • Temporary workspaces
   • Learning & education
   • POC (Proof of Concepts)

❌ KHÔNG ĐƯỢC PHÉP:
   • Mining (crypto hoặc bất kỳ loại nào)
   • Long-running production services
   • Content delivery / file hosting
   • Website hosting
   • Proxy / VPN services
   • Bất kỳ hoạt động vi phạm GitHub ToS

Vi phạm = Account ban vĩnh viễn, không thể khôi phục!
```

### 💾 **Cảnh báo về dữ liệu**

```
╔════════════════════════════════════════════════════════════════════════╗
║                     💾 DATA LOSS WARNING                               ║
╠════════════════════════════════════════════════════════════════════════╣
║                                                                        ║
║  ⚠️  MỌI DỮ LIỆU SẼ BỊ XÓA HOÀN TOÀN SAU KHI WORKFLOW KẾT THÚC       ║
║                                                                        ║
║  • Tối đa 6 giờ/session                                               ║
║  • Không có backup tự động                                            ║
║  • Không thể khôi phục sau khi xóa                                    ║
║  • Không có warning trước khi kết thúc                                ║
║                                                                        ║
║  📋 CHECKLIST TRƯỚC KHI KẾT THÚC:                                     ║
║  ☐ Upload files quan trọng lên cloud (Google Drive, Dropbox, etc)    ║
║  ☐ Push code lên GitHub repository                                    ║
║  ☐ Export databases nếu có                                            ║
║  ☐ Save screenshots/logs nếu cần                                      ║
║  ☐ Download mọi files cần thiết                                       ║
║                                                                        ║
╚════════════════════════════════════════════════════════════════════════╝
```

---

## 📚 **MỤC LỤC**

- [🔐 Thông báo bản quyền](#-thông-báo-bản-quyền)
- [⚠️ Cảnh báo quan trọng](#️-cảnh-báo-quan-trọng)
- [✨ Tính năng](#-tính-năng)
- [⚡ Cài đặt nhanh](#-cài-đặt-nhanh)
- [📖 Hướng dẫn sử dụng](#-hướng-dẫn-sử-dụng)
- [🖥️ Các phiên bản hệ điều hành](#️-các-phiên-bản-hệ-điều-hành)
- [🔑 Thông tin đăng nhập](#-thông-tin-đăng-nhập)
- [🌐 Kết nối RDP](#-kết-nối-rdp)
- [🖥️ Web Viewer](#️-web-viewer)
- [🔧 Khắc phục sự cố](#-khắc-phục-sự-cố)
- [❓ FAQ](#-faq)
- [📞 Hỗ trợ](#-hỗ-trợ)
- [🙏 Credits](#-credits)

---

## ✨ **TÍNH NĂNG**

### 🎯 **Điểm nổi bật chính**

```
╔════════════════════════════════════════════════════════════════════════╗
║                         ⭐ KEY FEATURES                                ║
╠════════════════════════════════════════════════════════════════════════╣
║                                                                        ║
║  🌟 8 HỆ ĐIỀU HÀNH                                                     ║
║     • Windows Server 2025, 2022, 2019, 2012                           ║
║     • Windows 11 & 10 Professional                                     ║
║     • Ubuntu 24.04 Desktop                                             ║
║                                                                        ║
║  ⚡ HIỆU NĂNG CAO                                                       ║
║     • Native: 4 vCPU + 16GB RAM                                        ║
║     • Docker: 4 vCPU + 8GB RAM                                         ║
║     • SSD Storage: 60-120GB                                            ║
║                                                                        ║
║  🌐 PUBLIC IP TỰ ĐỘNG                                                  ║
║     • Kami Tunnel integration                                          ║
║     • Kết nối từ mọi nơi trên thế giới                                ║
║     • Không cần VPN hay port forwarding                               ║
║                                                                        ║
║  🖥️ WEB VIEWER (Docker versions)                                       ║
║     • Xem màn hình Windows qua browser                                ║
║     • Monitor installation progress                                    ║
║     • Port 8006 - HTTP access                                          ║
║                                                                        ║
║  🤖 TỰ ĐỘNG HÓA 100%                                                   ║
║     • Zero manual configuration                                        ║
║     • Auto RDP setup                                                   ║
║     • Auto user creation                                               ║
║     • Auto firewall config                                             ║
║                                                                        ║
║  💰 HOÀN TOÀN MIỄN PHÍ                                                 ║
║     • GitHub Actions Free Tier                                         ║
║     • 2,000 phút/tháng (Free account)                                 ║
║     • Không cần credit card                                           ║
║                                                                        ║
╚════════════════════════════════════════════════════════════════════════╝
```

### 🔥 **Tính năng Version 2.0**

<table>
<tr>
<th width="30%">Tính năng</th>
<th width="70%">Mô tả chi tiết</th>
</tr>
<tr>
<td><b>🔄 Dual Tunnel Support</b></td>
<td>
• Xử lý chính xác 2 tunnel đồng thời<br>
• RDP Port 3389 + Web Viewer Port 8006<br>
• Smart IP detection và phân biệt IP<br>
• Automatic backup mechanism
</td>
</tr>
<tr>
<td><b>🛡️ Error Handling</b></td>
<td>
• 60x Retry mechanism (120s timeout)<br>
• IP validation với regex<br>
• Comprehensive logging<br>
• Intelligent fallback strategies
</td>
</tr>
<tr>
<td><b>🎨 Professional UI</b></td>
<td>
• Beautiful box design với Unicode<br>
• Clear sections: RDP / Web / Resources<br>
• Real-time status với timestamp<br>
• Color-coded information
</td>
</tr>
<tr>
<td><b>⚡ Performance</b></td>
<td>
• Optimized timing giữa các bước<br>
• Faster boot time<br>
• Stable connections<br>
• Better resource management
</td>
</tr>
</table>

---

## ⚡ **CÀI ĐẶT NHANH**

### 🚀 **Quick Start - 3 Bước**

#### **BƯỚC 1: Fork Repository**

```bash
# Truy cập:
https://github.com/zun209384-lgtm/window

# Click nút "Fork" ở góc phải trên

# ⚠️ LƯU Ý: 
# - KHÔNG được xóa thông báo bản quyền
# - KHÔNG được thay đổi credits
# - GIỮ NGUYÊN tất cả comments về author
```

#### **BƯỚC 2: Kích Hoạt Workflow**

```
1. Vào repository đã fork
2. Tab "Actions"
3. Click "I understand my workflows, go ahead and enable them"
4. Chọn "🖥️ REMOTE DESKTOP SERVICES"
5. Click "Run workflow"
```

#### **BƯỚC 3: Chọn OS và Chạy**

```
1. Dropdown "📀 Select Operating System"
2. Chọn 1 trong 8 options
3. Click "Run workflow" để confirm
4. Đợi 3-15 phút tùy OS
5. Lấy thông tin kết nối từ logs
```

### 📋 **Chi tiết từng phương pháp**

<details>
<summary><b>Phương pháp 1: Fork (Đề xuất cho người mới)</b></summary>

**Bước 1: Fork**
```
https://github.com/zun209384-lgtm/window
→ Click "Fork"
→ Chọn owner là tài khoản của bạn
→ Giữ nguyên repository name hoặc đổi tên
→ Click "Create fork"
```

**Bước 2: Enable Actions**
```
Vào repository đã fork
→ Tab "Actions"
→ "I understand my workflows, go ahead and enable them"
```

**Bước 3: Run**
```
→ "🖥️ REMOTE DESKTOP SERVICES"
→ "Run workflow"
→ Chọn OS
→ "Run workflow" để confirm
```

</details>

<details>
<summary><b>Phương pháp 2: Tạo Repository mới</b></summary>

**Bước 1: Tạo repo**
```bash
# Trên GitHub.com
New repository
→ Name: rdp-services
→ Public hoặc Private
→ Add README
→ Create repository
```

**Bước 2: Clone về máy**
```bash
git clone https://github.com/[your-username]/rdp-services.git
cd rdp-services
```

**Bước 3: Tạo workflow**
```bash
mkdir -p .github/workflows
curl -o .github/workflows/rdp.yml \
  https://raw.githubusercontent.com/zun209384-lgtm/window/main/Windows_Fixed.yml
```

**Bước 4: Commit và push**
```bash
git add .github/workflows/rdp.yml
git commit -m "Add RDP workflow v2.0"
git push origin main
```

**⚠️ QUAN TRỌNG: Giữ nguyên credits**
```yaml
# PHẢI thêm vào đầu file README.md:

## Credits
Forked from: https://github.com/zun209384-lgtm/window
Author: Zun209384-lgtm
All rights reserved.
```

</details>

<details>
<summary><b>Phương pháp 3: GitHub CLI (Advanced)</b></summary>

```bash
# Cài đặt gh CLI
brew install gh  # macOS
winget install GitHub.cli  # Windows

# Đăng nhập
gh auth login

# Fork repository
gh repo fork zun209384-lgtm/window --clone

# Hoặc tạo mới
gh repo create rdp-services --public --clone
cd rdp-services

# Download workflow
mkdir -p .github/workflows
curl -o .github/workflows/rdp.yml \
  https://raw.githubusercontent.com/zun209384-lgtm/window/main/Windows_Fixed.yml

# Commit
git add .
git commit -m "Add RDP workflow"
git push

# Run workflow
gh workflow run rdp.yml \
  -f os_version="Windows Server 2025 (Native - 4vCPU | 16GB RAM)"
```

</details>

---

## 📖 **HƯỚNG DẪN SỬ DỤNG**

### 🎬 **Quy trình sử dụng đầy đủ**

```
╔════════════════════════════════════════════════════════════════════════╗
║                     📋 WORKFLOW EXECUTION STEPS                        ║
╠════════════════════════════════════════════════════════════════════════╣
║                                                                        ║
║  STEP 1: Khởi chạy Workflow                                           ║
║    ├─ Vào tab Actions                                                 ║
║    ├─ Chọn "🖥️ REMOTE DESKTOP SERVICES"                               ║
║    └─ Click "Run workflow"                                            ║
║                                                                        ║
║  STEP 2: Chọn Hệ điều hành                                            ║
║    ├─ Dropdown: 8 options available                                   ║
║    ├─ Windows Server: 2025/2022/2019/2012                             ║
║    ├─ Windows Desktop: 11/10 Pro                                      ║
║    └─ Linux: Ubuntu 24.04 Desktop                                     ║
║                                                                        ║
║  STEP 3: Đợi hệ thống khởi động                                       ║
║    ├─ Native: 3-7 phút                                                ║
║    └─ Docker: 10-15 phút                                              ║
║                                                                        ║
║  STEP 4: Lấy thông tin kết nối                                        ║
║    ├─ Click vào step "🌐 Connection Information"                      ║
║    ├─ Copy: IP:Port, Username, Password                              ║
║    └─ Copy: Web Viewer URL (nếu có)                                   ║
║                                                                        ║
║  STEP 5: Kết nối RDP                                                  ║
║    ├─ Mở RDP Client                                                   ║
║    ├─ Nhập thông tin                                                  ║
║    └─ Connect                                                         ║
║                                                                        ║
║  STEP 6: Sử dụng hệ thống                                             ║
║    ├─ Max: 6 giờ (360 phút)                                           ║
║    └─ Session tự động kết thúc sau 6h                                 ║
║                                                                        ║
║  STEP 7: Backup dữ liệu                                               ║
║    ├─ Upload lên cloud storage                                        ║
║    ├─ Push code lên GitHub                                            ║
║    └─ Download files quan trọng                                       ║
║                                                                        ║
╚════════════════════════════════════════════════════════════════════════╝
```

### 📊 **Timeline chi tiết**

```
Minute 0-1    ┌──────────────────────────────────────┐
              │ 🚀 Workflow Queued & Starting        │
              └──────────────────────────────────────┘

Minute 1-15   ┌──────────────────────────────────────┐
              │ 🔧 System Initialization             │
              │ • Install packages                   │
              │ • Configure RDP                      │
              │ • Start tunnels                      │
              │ • Boot OS (if Docker)                │
              └──────────────────────────────────────┘

Minute 15-16  ┌──────────────────────────────────────┐
              │ 🌐 Connection Info Ready             │
              │ • RDP IP:Port available              │
              │ • Web Viewer URL (Docker)            │
              └──────────────────────────────────────┘

Minute 16-360 ┌──────────────────────────────────────┐
              │ ⏰ Active Session                    │
              │ • Status update every 5 min          │
              │ • User can connect & work            │
              └──────────────────────────────────────┘

Minute 360    ┌──────────────────────────────────────┐
              │ 🛑 Workflow End                      │
              │ • All data deleted                   │
              │ • Connection closed                  │
              └──────────────────────────────────────┘
```

---

## 🖥️ **CÁC PHIÊN BẢN HỆ ĐIỀU HÀNH**

### 📊 **Bảng so sánh nhanh**

| OS | Type | RAM | Boot Time | Web Viewer | Performance |
|----|------|-----|-----------|------------|-------------|
| **Win Server 2025** | Native | 16GB | 3-5 min | ❌ | ⭐⭐⭐⭐⭐ |
| **Win Server 2025** | Docker | 8GB | 10-15 min | ✅ | ⭐⭐⭐⭐ |
| **Win Server 2022** | Docker | 8GB | 10-12 min | ✅ | ⭐⭐⭐⭐ |
| **Win Server 2019** | Docker | 8GB | 10-12 min | ✅ | ⭐⭐⭐⭐ |
| **Win Server 2012** | Docker | 8GB | 10-12 min | ✅ | ⭐⭐⭐ |
| **Windows 11 Pro** | Docker | 8GB | 12-15 min | ✅ | ⭐⭐⭐⭐ |
| **Windows 10 Pro** | Docker | 8GB | 10-12 min | ✅ | ⭐⭐⭐⭐ |
| **Ubuntu 24.04** | Native | 16GB | 5-7 min | ❌ | ⭐⭐⭐⭐⭐ |

### 🪟 **Windows Systems**

<details>
<summary><b>1. Windows Server 2025 (Native) - ⭐ RECOMMENDED</b></summary>

```yaml
╔══════════════════════════════════════════════════════════╗
║         WINDOWS SERVER 2025 (NATIVE)                     ║
╠══════════════════════════════════════════════════════════╣
║  Runner      : windows-latest                            ║
║  CPU         : 4 vCPU                                     ║
║  RAM         : 16GB DDR4                                  ║
║  Storage     : ~120GB SSD                                 ║
║  Boot Time   : 3-5 minutes                                ║
║  Performance : ⭐⭐⭐⭐⭐ (Highest)                           ║
╚══════════════════════════════════════════════════════════╝
```

**Ưu điểm:**
- ⚡ Hiệu năng cao nhất - Native performance
- 🚀 Boot nhanh nhất - Sẵn sàng trong 3-5 phút
- 💪 RAM lớn nhất - 16GB cho multitasking
- ✅ Ổn định tuyệt đối - Ít lỗi nhất

**Hạn chế:**
- 🌐 Không có Web Viewer
- 🔧 Không linh hoạt như Docker

**Phù hợp cho:**
- Production workloads
- Development cần compile code
- Tasks cần RAM > 8GB

</details>

<details>
<summary><b>2. Windows Server 2025 (Docker) - 🌐 WEB VIEWER</b></summary>

```yaml
╔══════════════════════════════════════════════════════════╗
║         WINDOWS SERVER 2025 (DOCKER)                     ║
╠══════════════════════════════════════════════════════════╣
║  Runner      : ubuntu-latest                             ║
║  Deployment  : Docker Container                          ║
║  CPU         : 4 vCPU                                     ║
║  RAM         : 8GB                                        ║
║  Storage     : 60GB                                       ║
║  Boot Time   : 10-15 minutes                              ║
║  Web Viewer  : ✅ Port 8006                               ║
║  Performance : ⭐⭐⭐⭐                                      ║
╚══════════════════════════════════════════════════════════╝
```

**Ưu điểm:**
- 🖥️ Web Viewer - Xem installation qua browser
- 🔧 Linh hoạt - Custom disk size, RAM
- 📦 Isolated - Chạy trong container
- 🎨 Latest - Windows Server 2025 mới nhất

**Hạn chế:**
- ⏱️ Boot lâu hơn - 10-15 phút
- 🐌 Performance thấp hơn ~10-15%
- 💻 RAM chỉ 8GB

**Phù hợp cho:**
- Testing & Development
- Theo dõi installation progress
- Learning Windows Server 2025

</details>

<details>
<summary><b>3-7. Các phiên bản Windows khác</b></summary>

**Windows Server 2022 (Docker):**
- Production-ready, Stable
- Wide compatibility
- Security updates regular

**Windows Server 2019 (Docker):**
- LTS (Long Term Support)
- Very stable and well-tested
- Legacy app compatibility

**Windows Server 2012 (Docker):**
- End of support
- Chỉ dùng cho compatibility testing
- Lightweight

**Windows 11 Professional (Docker):**
- Modern UI
- Latest Windows features
- DirectStorage, Auto HDR

**Windows 10 Professional (Docker):**
- Classic UI
- Most compatible
- Lighter than Win 11

</details>

<details>
<summary><b>8. Ubuntu 24.04 Desktop (Native) - 🐧 LINUX</b></summary>

```yaml
╔══════════════════════════════════════════════════════════╗
║         UBUNTU 24.04 DESKTOP (NATIVE)                    ║
╠══════════════════════════════════════════════════════════╣
║  Runner      : ubuntu-latest                             ║
║  Desktop     : XFCE4                                      ║
║  RDP Server  : XRDP                                       ║
║  CPU         : 4 vCPU                                     ║
║  RAM         : 16GB                                       ║
║  Storage     : ~120GB                                     ║
║  Boot Time   : 5-7 minutes                                ║
║  Performance : ⭐⭐⭐⭐⭐                                     ║
╚══════════════════════════════════════════════════════════╝
```

**Ưu điểm:**
- 🖱️ Full Desktop - XFCE4 lightweight
- ⚡ Cực nhanh - Linux native performance
- 💪 16GB RAM - Development powerhouse
- 🔧 Developer-friendly - Full package management

**Phù hợp cho:**
- Linux development
- Web development (Node, Python, PHP)
- DevOps practice
- Docker & Kubernetes development

</details>

---

## 🔑 **THÔNG TIN ĐĂNG NHẬP**

### 🪟 **Windows (Tất cả phiên bản)**

```
╔════════════════════════════════════════════════════════════╗
║              WINDOWS LOGIN CREDENTIALS                     ║
╠════════════════════════════════════════════════════════════╣
║  Username : Admin                                          ║
║  Password : Window@123456                                  ║
║  Type     : Administrator                                  ║
║  Rights   : Full Control                                   ║
╚════════════════════════════════════════════════════════════╝

⚠️ LƯU Ý:
• Password có @ (at symbol)
• Phân biệt chữ hoa/thường
• Chữ W viết HOA
```

### 🐧 **Ubuntu Desktop**

```
╔════════════════════════════════════════════════════════════╗
║              UBUNTU LOGIN CREDENTIALS                      ║
╠════════════════════════════════════════════════════════════╣
║  Username : Admin                                          ║
║  Password : Ubuntu@123456                                  ║
║  Type     : Sudo User                                      ║
║  Rights   : Root Access                                    ║
╚════════════════════════════════════════════════════════════╝

⚠️ LƯU Ý:
• Password có @ (at symbol)
• Case-sensitive trên Linux
• Chữ U viết HOA
```

### 🔒 **Cảnh báo bảo mật**

```
⚠️⚠️⚠️ QUAN TRỌNG ⚠️⚠️⚠️

• Đây là password MẶC ĐỊNH
• KHÔNG dùng cho production
• KHÔNG lưu dữ liệu nhạy cảm
• ĐỔI password nếu cần bảo mật cao

Cách đổi password:
Windows: net user Admin <new_password>
Ubuntu:  sudo passwd Admin
```

---

## 🌐 **KẾT NỐI RDP**

### 🪟 **Windows - Remote Desktop**

<details>
<summary><b>Phương pháp 1: GUI</b></summary>

**Bước 1: Mở RDP**
```
Windows + R
→ Gõ: mstsc
→ Enter
```

**Bước 2: Nhập thông tin**
```
Computer: 123.45.67.89:3389
Username: Admin
Password: Window@123456
```

**Bước 3: Connect**
```
Click "Connect"
→ Accept certificate warning
→ Done!
```

</details>

<details>
<summary><b>Phương pháp 2: Command Line</b></summary>

```cmd
# Basic
mstsc /v:123.45.67.89:3389

# Admin mode
mstsc /v:123.45.67.89:3389 /admin

# Fullscreen
mstsc /v:123.45.67.89:3389 /f

# Custom resolution
mstsc /v:123.45.67.89:3389 /w:1920 /h:1080
```

</details>

### 🍎 **macOS - Microsoft Remote Desktop**

<details>
<summary><b>Cài đặt và sử dụng</b></summary>

**Cài đặt:**
```bash
# Từ App Store
Mac App Store → "Microsoft Remote Desktop"

# Hoặc Homebrew
brew install --cask microsoft-remote-desktop
```

**Sử dụng:**
```
1. Mở app
2. Click "+" → Add PC
3. PC name: 123.45.67.89:3389
4. User account: Admin / Window@123456
5. Double-click để connect
```

</details>

### 🐧 **Linux - Remmina**

<details>
<summary><b>Cài đặt và sử dụng</b></summary>

**Cài đặt:**
```bash
# Ubuntu/Debian
sudo apt install remmina remmina-plugin-rdp

# Fedora
sudo dnf install remmina

# Arch
sudo pacman -S remmina freerdp
```

**Sử dụng:**
```
1. Chạy: remmina
2. Click "+" → New connection
3. Protocol: RDP
4. Server: 123.45.67.89:3389
5. Username: Admin
6. Password: Window@123456
7. Connect
```

</details>

---

## 🖥️ **WEB VIEWER**

### 🌟 **Giới thiệu**

```
╔════════════════════════════════════════════════════════════╗
║              🌐 WEB VIEWER - REAL-TIME MONITOR             ║
╠════════════════════════════════════════════════════════════╣
║                                                            ║
║  Web Viewer cho phép XEM MÀN HÌNH Windows qua BROWSER     ║
║  mà KHÔNG CẦN RDP client!                                 ║
║                                                            ║
║  ✅ Xem installation progress real-time                   ║
║  ✅ Không cần cài RDP client                              ║
║  ✅ Hoạt động trên mọi thiết bị                           ║
║  ✅ Port 8006 - HTTP access                               ║
║                                                            ║
║  ⚠️ CHỈ có trên Docker versions                           ║
║  ⚠️ KHÔNG có trên Native versions                         ║
║                                                            ║
╚════════════════════════════════════════════════════════════╝
```

### 🚀 **Cách sử dụng**

**Bước 1: Lấy URL**
```
Trong workflow log, tìm:
🔗 Web Address: http://123.45.67.89:8006
```

**Bước 2: Truy cập**
```
1. Mở browser
2. Paste URL: http://123.45.67.89:8006
3. Enter
```

**Bước 3: Xem màn hình**
```
Bạn sẽ thấy màn hình Windows real-time:
• Boot process
• Installation progress
• Desktop khi ready
```

### 📊 **So sánh Web Viewer vs RDP**

| Tiêu chí | Web Viewer | RDP |
|----------|------------|-----|
| Cài đặt | Không cần | Cần client |
| Performance | ⭐⭐⭐ | ⭐⭐⭐⭐⭐ |
| Xem Boot | ✅ YES | ❌ NO |
| Production | ❌ NO | ✅ YES |
| Clipboard | ❌ NO | ✅ YES |
| File transfer | ❌ NO | ✅ YES |

---

## 🔧 **KHẮC PHỤC SỰ CỐ**

### 🐛 **Common Issues**

<details>
<summary><b>1. Workflow stuck ở "Queued"</b></summary>

**Nguyên nhân:**
- Hết quota GitHub Actions
- Runners đang bận
- Actions bị disable

**Giải pháp:**
```bash
# Check quota
Settings → Billing → Actions

# Enable Actions
Settings → Actions → Allow all actions

# Retry
Cancel workflow → Run lại
```

</details>

<details>
<summary><b>2. Không lấy được IP</b></summary>

**Nguyên nhân:**
- Tunnel chưa start
- Network issue
- File kami_tunnel.txt không tồn tại

**Giải pháp:**
```
1. Kiểm tra workflow logs
2. Đợi thêm 2-3 phút
3. Check tunnel process đang chạy
4. Run lại workflow nếu cần
```

</details>

<details>
<summary><b>3. RDP connection refused</b></summary>

**Nguyên nhân:**
- Sai IP:Port
- RDP service chưa start
- Firewall blocking

**Giải pháp:**
```
1. Kiểm tra format IP:3389
2. Đợi thêm vài phút
3. Check firewall trên máy bạn
4. Thử từ network khác
```

</details>

<details>
<summary><b>4. Web Viewer không load</b></summary>

**Nguyên nhân:**
- Docker chưa start xong
- Port 8006 chưa ready

**Giải pháp:**
```
1. Đợi thêm 5-10 phút
2. F5 refresh browser
3. Clear cache
4. Check URL: http:// (không https://)
```

</details>

<details>
<summary><b>5. Credential không đúng</b></summary>

**Nguyên nhân:**
- Sai username/password
- Case sensitivity

**Giải pháp:**
```
Windows:
Username: Admin (chữ A viết HOA)
Password: Window@123456 (chữ W HOA, có @)

Ubuntu:
Username: Admin (chữ A viết HOA)
Password: Ubuntu@123456 (chữ U HOA, có @)

Lưu ý: Password có ký tự @ và phân biệt hoa thường!
```

</details>

---

## ❓ **FAQ**

<details>
<summary><b>Q: Có mất phí không?</b></summary>

**A:** HOÀN TOÀN MIỄN PHÍ!
```
Free Account: 2,000 phút/tháng
Pro Account: 3,000 phút/tháng
Mỗi run: Tối đa 6 giờ (360 phút)
```

</details>

<details>
<summary><b>Q: Có thể chạy 24/7 không?</b></summary>

**A:** KHÔNG. Giới hạn 6 giờ/run.
```
Sau 6 giờ:
• Workflow tự động stop
• Mọi dữ liệu bị xóa
• Phải run lại manually
```

</details>

<details>
<summary><b>Q: Có GPU không?</b></summary>

**A:** KHÔNG có GPU.
```
❌ Không chạy được:
• Games
• Video editing (GPU-accelerated)
• AI/ML training
• 3D rendering

✅ Có thể chạy:
• Programming
• Web browsing
• Office work
```

</details>

<details>
<summary><b>Q: Có thể cài software không?</b></summary>

**A:** CÓ, full admin rights!
```
Windows: Download .exe/.msi và install
Ubuntu: sudo apt install <package>

⚠️ Lưu ý: Mọi cài đặt mất sau 6 giờ!
```

</details>

<details>
<summary><b>Q: Dữ liệu có được lưu không?</b></summary>

**A:** KHÔNG! Mọi dữ liệu bị XÓA sau 6h.
```
PHẢI backup trước khi kết thúc:
• Upload lên cloud
• Push code lên GitHub
• Download files quan trọng
```

</details>

---

## 📞 **HỖ TRỢ**

### 💬 **Kênh hỗ trợ chính thức**

```
╔════════════════════════════════════════════════════════════╗
║              📞 OFFICIAL SUPPORT CHANNELS                  ║
╠════════════════════════════════════════════════════════════╣
║                                                            ║
║  🐛 GitHub Issues (RECOMMENDED)                           ║
║     https://github.com/zun209384-lgtm/window/issues       ║
║                                                            ║
║  💬 GitHub Discussions                                     ║
║     https://github.com/zun209384-lgtm/window/discussions  ║
║                                                            ║
║  📧 Email                                                  ║
║     (Available in repository description)                  ║
║                                                            ║
╚════════════════════════════════════════════════════════════╝
```

### 📋 **Khi tạo Issue**

**Bao gồm:**
```markdown
1. OS version đã chọn
2. Workflow run URL
3. Full error logs
4. Screenshots
5. Steps to reproduce
6. Expected vs actual behavior
```

**Template:**
```markdown
**Describe the issue**
Mô tả chi tiết

**To Reproduce**
1. Go to '...'
2. Click on '...'
3. See error

**Expected behavior**
Hành vi mong đợi

**Screenshots**
Attach screenshots

**Environment:**
- OS: Windows Server 2025
- Runner: windows-latest

**Logs**
```
paste logs here
```
```

---

## 🙏 **CREDITS**

```
╔════════════════════════════════════════════════════════════╗
║                      👏 CREDITS                            ║
╠════════════════════════════════════════════════════════════╣
║                                                            ║
║  👤 ORIGINAL AUTHOR                                        ║
║     • Zun209384-lgtm                                       ║
║     • GitHub: https://github.com/zun209384-lgtm           ║
║     • Repository: https://github.com/zun209384-lgtm/window║
║                                                            ║
║  📅 VERSION                                                ║
║     • Version: 2.0                                         ║
║     • Release: January 2026                                ║
║     • Status: Production Ready                             ║
║                                                            ║
║  🛠️ TOOLS & SERVICES                                       ║
║     • GitHub Actions - CI/CD Platform                      ║
║     • Kami Tunnel - Public IP Tunneling                    ║
║     • Dockurr/Windows - Windows Docker Images              ║
║     • Microsoft - Windows & RDP Protocol                   ║
║     • Canonical - Ubuntu Linux                             ║
║                                                            ║
║  📜 COPYRIGHT                                              ║
║     • © 2024-2026 Zun209384-lgtm                          ║
║     • All Rights Reserved                                  ║
║     • Protected by DMCA                                    ║
║                                                            ║
╚════════════════════════════════════════════════════════════╝
```

### ⚖️ **Compliance Statement**

```
This project complies with:
✅ GitHub Terms of Service
✅ GitHub Actions Usage Limits
✅ DMCA Guidelines
✅ International Copyright Laws
✅ Open Source Best Practices

All trademarks, logos, and brand names are the property
of their respective owners.
```

---

## 📜 **LEGAL DISCLAIMER**

```
╔════════════════════════════════════════════════════════════════════════╗
║                         ⚖️ LEGAL DISCLAIMER                            ║
╠════════════════════════════════════════════════════════════════════════╣
║                                                                        ║
║  This software is provided "AS IS" without warranty of any kind,       ║
║  either expressed or implied, including but not limited to the         ║
║  implied warranties of merchantability and fitness for a particular    ║
║  purpose.                                                              ║
║                                                                        ║
║  The author(s) shall not be liable for any damages, including but      ║
║  not limited to direct, indirect, incidental, special, exemplary,      ║
║  or consequential damages arising out of the use or inability to       ║
║  use this software.                                                    ║
║                                                                        ║
║  Users are solely responsible for:                                     ║
║  • Compliance with GitHub Terms of Service                            ║
║  • Legal use of GitHub Actions resources                              ║
║  • Protection of their own data and credentials                       ║
║  • Ensuring their activities comply with local laws                   ║
║                                                                        ║
║  This software must not be used for:                                   ║
║  • Illegal activities of any kind                                     ║
║  • Mining cryptocurrencies                                            ║
║  • DDoS attacks or network abuse                                      ║
║  • Spam or phishing operations                                        ║
║  • Any activity violating GitHub ToS                                  ║
║                                                                        ║
║  By using this software, you agree to these terms and take            ║
║  full responsibility for your actions.                                 ║
║                                                                        ║
╚════════════════════════════════════════════════════════════════════════╝
```

---

<div align="center">

## ⭐ **STAR THIS REPOSITORY** ⭐

**Nếu project này hữu ích, hãy cho 1 Star! 🌟**

---

### 📊 **Repository Statistics**

![GitHub stars](https://img.shields.io/github/stars/zun209384-lgtm/window?style=social)
![GitHub forks](https://img.shields.io/github/forks/zun209384-lgtm/window?style=social)
![GitHub watchers](https://img.shields.io/github/watchers/zun209384-lgtm/window?style=social)

![GitHub issues](https://img.shields.io/github/issues/zun209384-lgtm/window)
![GitHub pull requests](https://img.shields.io/github/issues-pr/zun209384-lgtm/window)
![GitHub last commit](https://img.shields.io/github/last-commit/zun209384-lgtm/window)

---

### 📄 **License & Copyright**

```
MIT License

Copyright (c) 2024-2026 Zun209384-lgtm

All rights reserved. Unauthorized copying, modification,
distribution, or use of this software is strictly prohibited
without explicit written permission from the copyright holder.
```

---

Made with ❤️ by [Zun209384-lgtm](https://github.com/zun209384-lgtm)

**Version 2.0 - January 2026**

[⬆ Về đầu trang](#️-remote-desktop-services---github-actions-workflow)

---

</div>
