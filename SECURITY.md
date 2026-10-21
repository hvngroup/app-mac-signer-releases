# Bảo mật

## Báo lỗ hổng

Vui lòng **không mở issue công khai**. Gửi riêng tới **kythuat@hvn.vn** hoặc qua
[GitHub Security Advisories](https://github.com/hvngroup/app-mac-signer-releases/security/advisories/new),
kèm phiên bản bị ảnh hưởng và các bước tái hiện. HVN GROUP phản hồi trong vài ngày làm việc và ghi công người báo
trong release notes nếu anh/chị muốn.

Không gửi kèm PIN, mật khẩu, tệp `.p12`/`.pfx`, khoá bí mật, tài liệu thật, dữ liệu nội bộ hay dữ liệu khách hàng.

## Ứng dụng xử lý dữ liệu thế nào

- **Tài liệu không rời máy.** Ký và kiểm tra chữ ký PDF chạy hoàn toàn trên máy Mac.
- **Không lưu PIN, mật khẩu hay khoá bí mật.** PIN chỉ nằm trong bộ nhớ trong lúc ký; khoá bí mật không rời USB token
  hoặc tệp chứng thư. Ứng dụng không tự thử PIN.
- **Dữ liệu lưu trên máy** nằm trong `~/Library/Application Support/vn.hvn.macsigner/`: cài đặt, mẫu chữ ký và lịch sử.
  Lịch sử chỉ ghi thời điểm, thao tác và kết quả, không ghi nội dung tài liệu.
- **Dịch vụ ký cho trang web** (ESIGN cho cổng thuế, API tương thích CTSigningHub cho trang hóa đơn điện tử) mặc định
  tắt và chỉ nhận kết nối từ chính máy. Mỗi lần trang web yêu cầu ký, ứng dụng hiện hộp thoại để người dùng kiểm tra;
  không bấm **Ký** thì không có gì được ký.
- **Dấu thời gian** (mặc định tắt): khi bật, mỗi lần ký ứng dụng gửi mã băm SHA-256 của chữ ký (không gửi tài liệu) tới
  máy chủ dấu thời gian người dùng chọn, mặc định `http://timestamp.digicert.com`.
- **Kiểm tra cập nhật:** khi bật **Tự động cập nhật** (mặc định), vài giờ một lần ứng dụng
  đọc `latest.json` ở repo này và không gửi dữ liệu nào. Tắt công tắc này ở **Cài đặt → Giới thiệu** thì ứng dụng không
  tự kết nối. Không có máy chủ của HVN và không thu thập dữ liệu sử dụng.
- **Cập nhật** chỉ được cài khi gói mang chữ ký bằng khoá cập nhật của HVN GROUP, và chỉ khi người dùng khởi động lại
  hoặc thoát ứng dụng. Bản macOS được ký Developer ID của HVN GROUP và notarize bởi Apple.

## Phiên bản được hỗ trợ

Chỉ bản phát hành mới nhất được vá lỗi.

---

HVN GROUP · hvn.vn
