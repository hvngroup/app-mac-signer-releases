# HVN Mac Signer — bản phát hành

HVN Mac Signer giúp ký số tệp PDF, ký kê khai thuế và hóa đơn điện tử ngay trên máy Mac, bằng USB token hoặc chứng thư
dạng tệp `.p12`/`.pfx`, không cần mượn máy Windows. Ứng dụng có giao diện tiếng Việt (mặc định) và English, chạy trên
Mac chip Apple và Intel, macOS 12 trở lên.

Repo này chỉ chứa bản phát hành và kênh cập nhật của ứng dụng. Mã nguồn được quản lý riêng tại HVN GROUP.

## Tải về

Tải bản mới nhất ở trang [Releases](https://github.com/hvngroup/app-mac-signer-releases/releases/latest):

| Máy | Tệp |
|---|---|
| Mac chip Apple (M1 trở lên) hoặc Intel, macOS 12 trở lên | `HVNMacSigner-<phiên bản>-universal.dmg` |
| Như trên, nếu không dùng được tệp `.dmg` | `HVNMacSigner-<phiên bản>-universal.zip` |

Mỗi tệp có một tệp `.sha256` đi kèm để đối chiếu; `SHA256SUMS.txt` gom mã của mọi tệp. Tệp `.app.tar.gz`, `.sig` và
`latest.json` dành cho trình cập nhật của ứng dụng, không cần tải về.

## Cài đặt

Mở tệp `.dmg`, kéo **HVN Mac Signer** vào **Applications** rồi mở. Bản phát hành được ký bằng Developer ID của HVN
GROUP và đã qua notarize của Apple, nên macOS mở bình thường.

Nếu dùng USB token, cài phần mềm USB token cho Mac của nhà cung cấp chứng thư số (nếu hãng có); ứng dụng tự tìm phần
mềm đó. Dùng chứng thư dạng tệp thì vào **Chứng thư số → Nhập P12/PFX**.

## Cập nhật

Bản cài trong **Applications** tự tìm và cài bản mới từ repo này. Ứng dụng chỉ cài gói được ký bằng khoá cập nhật của
HVN GROUP và không khởi động lại khi anh/chị đang ký. Có thể kiểm tra ngay ở **HVN Mac Signer → Kiểm tra cập nhật…**.
Cài đặt, mẫu chữ ký và chứng thư đã nhập được giữ nguyên.

## Báo lỗi và hỗ trợ

- Báo lỗi hoặc góp ý: mở [issue](https://github.com/hvngroup/app-mac-signer-releases/issues/new/choose). Ghi kèm
  phiên bản (trong cửa sổ **Giới thiệu**), loại máy Mac và phiên bản macOS. Không đính kèm PIN, mật khẩu, tệp chứng
  thư hay tài liệu thật; che mã số thuế trong ảnh chụp.
- Lỗ hổng bảo mật: gửi qua
  [security advisory riêng](https://github.com/hvngroup/app-mac-signer-releases/security/advisories/new), đừng mở
  issue công khai. Cách ứng dụng xử lý dữ liệu: [SECURITY.md](SECURITY.md).
- Hỗ trợ kỹ thuật: kythuat@hvn.vn · Hotline 024.9999.7777

## Giấy phép

Phát hành theo [Apache 2.0](LICENSE): được dùng, sửa và phân phối lại, miễn là giữ thông báo bản quyền và giấy phép.
Ứng dụng phát triển từ mã nguồn mở MacSigner ([THIRD_PARTY_NOTICES.md](THIRD_PARTY_NOTICES.md)). Vui lòng đọc
[tuyên bố miễn trừ](DISCLAIMER.md) trước khi sử dụng.

---

HVN GROUP · [hvn.vn](https://hvn.vn)
