# Thông báo bên thứ ba

HVN Mac Signer chứa mã và tài nguyên của bên thứ ba. Mỗi phần giữ giấy phép riêng của nó.

## MacSigner — Nextwaves (Apache-2.0)

HVN Mac Signer được phát triển từ [MacSigner](https://github.com/DeanOpen/MacSigner), bản 0.2.2 (commit `6cb0590`,
20/10/2026), Copyright 2026 Nextwaves, phát hành theo [Apache License 2.0](LICENSE). Bản sao giấy phép nằm trong tệp
`LICENSE` của repo này.

Theo điều 4(b) của giấy phép, HVN GROUP ghi nhận các thay đổi chính so với bản gốc:

- Đổi tên sản phẩm thành HVN Mac Signer, định danh `vn.hvn.macsigner`, kênh cập nhật và khoá cập nhật của HVN GROUP.
- Chỉ hỗ trợ macOS: bỏ kho chứng thư Windows, bộ nạp DLL Windows, worker PKCS#11 x86 và các script PowerShell.
- Tách lõi ký thành crate `macsigner-core` và vỏ app Tauri thành crate `macsigner-app` trong một workspace Cargo.
- Dựng lại vỏ ứng dụng theo nhận diện HVN GROUP: biểu tượng, màu, menu macOS, cửa sổ Giới thiệu và Trợ giúp, giao diện
  tiếng Việt và English; bỏ phần nhà tài trợ.
- Quy trình kiểm thử, đóng gói và phát hành mới theo HVN App Builder Suite.

Danh sách đầy đủ theo từng phiên bản nằm trong mô tả của từng Release.

## Phông chữ

Chữ ký hiển thị trên PDF dùng phông có sẵn của macOS (Times New Roman, Arial); app không đóng gói phông này.

- **Inter**, **JetBrains Mono** (qua `@fontsource-variable`) — dùng trong giao diện. SIL Open Font License 1.1.

## Thư viện

- **PDF.js** (`pdfjs-dist`) — hiển thị PDF trong app. Apache License 2.0, Mozilla Foundation.
- Các crate Rust và gói npm khác giữ giấy phép ghi trong `Cargo.lock`/`pnpm-lock.yaml` và trong chính gói đó.

## Thương hiệu

Logo và tên của 26 tổ chức cung cấp dịch vụ chứng thực chữ ký số công cộng (VNPT-CA, Viettel-CA, FPT-CA, MISA-CA,…)
thuộc về chủ sở hữu tương ứng. Chúng chỉ dùng để giúp người dùng nhận ra nhà phát hành chứng thư của mình, không hàm ý
liên kết hay bảo trợ. Xem thêm `DISCLAIMER.md`.
