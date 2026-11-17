# zalo Bot — Thanh Hải

Trợ lý AI trên Zalo, hỗ trợ quản lý công việc, báo cáo, lịch hẹn và kho tri thức. Đa tài khoản, tự triển khai, tên hiển thị có thể tùy chỉnh.

Gói do **Bùi Thanh Hải** cấu hình và phát hành.

## Tải bộ mã nguồn và cài đặt

**[Tải zalo-agent-thanhhai.zip](./zalo-agent-thanhhai.zip?raw=true)**

Gói ZIP chứa đầy đủ 1.025 tệp mã nguồn, bộ cài Windows/Docker, tài liệu và giao diện web đã dựng. Giải nén ZIP trước khi chạy; các thư mục mã nguồn nằm trong gói tải về.

### Windows

1. Tải và giải nén ZIP.
2. Mở PowerShell trong thư mục `zalo-agent-thanhhai` có `package.json`.
3. Chạy:

```powershell
powershell -ExecutionPolicy Bypass -File cai-dat\cai-dat.ps1
```

4. Mở `http://127.0.0.1:3910` và làm theo thông tin do bộ cài hiển thị.
5. Cấu hình nhà cung cấp AI rồi quét QR đăng nhập Zalo bằng tài khoản muốn sử dụng.

Yêu cầu Node.js >=22.13. Xem `HUONG-DAN-CHO-TRO-LY-AI.md` và `BAN-THANHHAI.md` bên trong ZIP để biết chi tiết.

### Docker / VPS

Giải nén ZIP, vào thư mục có `package.json`, rồi chạy:

```bash
bash cai-dat/cai-dat-docker.sh
```

Hướng dẫn VPS đầy đủ nằm trong `docs/deploy-vps-guide.md` của gói.

## Cấu hình mặc định

- Tên hiển thị: **zalo Bot**, đổi trong trang Thương hiệu.
- Cổng dashboard: **3910**.
- Tác vụ Windows: `ZaloAgentThanhhai`.
- Danh tính trợ lý hỗ trợ Bùi Thanh Hải — Giám đốc Ban Quản lý Tòa nhà Eurowindow Office Building (EOB); có thể sửa trong trang Agent.

Không có khóa API, mật khẩu thật hoặc phiên đăng nhập Zalo trong gói phát hành. Tạo cấu hình riêng sau khi cài và sao lưu `.env` cùng thư mục dữ liệu.

## Giấy phép

MIT. Xem [LICENSE](./LICENSE). Các thông báo bản quyền trong giấy phép được giữ nguyên.
