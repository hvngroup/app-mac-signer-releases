# Disclaimer

> **Languages:** English first. [Tiếng Việt](#tuyen-bo-mien-tru) is below.

## No affiliation

HVN Mac Signer is an independent, interoperable implementation. It is not
affiliated with, sponsored by, endorsed by, or certified by any certificate
authority, any government agency, or the vendor of any other signing product.

HVN Mac Signer is built by HVN GROUP on the open-source MacSigner by Nextwaves
(Apache-2.0). Nextwaves does not sponsor, endorse or support this build.

All product names, brand names, trademarks and service marks that appear in
this project, in its documentation, or in its data tables are the property of
their respective owners. They are used only to identify the systems and
protocols that HVN Mac Signer is designed to interoperate with. Their appearance
does not imply any endorsement or partnership.

## No warranty

The software is provided "AS IS", without warranty of any kind, express or
implied, as stated in the [LICENSE](LICENSE). The authors and contributors are
not liable for any claim, damages or other liability arising from the use of
the software.

## Legal validity of signatures

HVN Mac Signer is a technical tool for producing and verifying digital signatures.
It does not, and cannot, guarantee that a signature it produces is legally
valid, admissible, or accepted by any portal, authority or counterparty. The
legal effect of an electronic signature depends on the certificate, the issuing
authority, applicable law, and the policies of the party that receives the
document. You are solely responsible for confirming that your certificate,
device and workflow meet those requirements.

RFC 3161 timestamping is optional and off by default; when turned on, the
time stamp comes from the time-stamp authority the user chooses, and the app
checks the token's signature but not the authority's certificate chain. The
following are not performed in the current release: full certificate chain
validation and revocation checking (OCSP / CRL). A certificate that is still within its validity dates is not,
by that fact alone, trustworthy or free of revocation.

## Devices, tokens and middleware

Device support is experimental. Detecting a reader, listing a token, or
reading a certificate does not mean that signing with a PIN, renewal, or
re-issuance will succeed on real hardware. Each combination of certificate
authority, device model, firmware, operating system and CPU architecture must
be verified independently.

HVN Mac Signer never stores PINs, passwords or private keys, never tries a PIN or a
default PIN on its own, and never writes to or erases data on a device. Entering
a wrong PIN too many times can lock a token; that risk is inherent to the
device, not to this software.

Vendor middleware (PKCS#11 libraries, USB or CCID drivers)
remains subject to the license of its vendor. Redistributing it in a portable
layout is your responsibility and may require the vendor's permission.

## Your responsibility

You are responsible for using HVN Mac Signer lawfully, for holding valid rights to
the certificates and devices you use, for complying with the terms of the
systems you connect to, and for verifying every signed document before you rely
on it.

---

<a id="tuyen-bo-mien-tru"></a>

# Tuyên bố miễn trừ

## Không liên kết

HVN Mac Signer là một bản triển khai độc lập, có khả năng tương tác. Phần mềm không
liên kết, không được tài trợ, không được bảo trợ và không được chứng nhận bởi
bất kỳ tổ chức chứng thực nào, bất kỳ cơ quan nhà nước nào, hay nhà cung cấp của
bất kỳ sản phẩm ký số nào khác.

HVN Mac Signer do HVN GROUP phát triển trên mã nguồn mở MacSigner của Nextwaves
(Apache-2.0). Nextwaves không bảo trợ, không xác nhận và không hỗ trợ bản này.

Mọi tên sản phẩm, tên thương hiệu, nhãn hiệu và nhãn hiệu dịch vụ xuất hiện
trong dự án này, trong tài liệu hoặc trong các bảng dữ liệu đều thuộc về chủ sở
hữu tương ứng. Chúng chỉ được dùng để nhận diện các hệ thống và giao thức mà
HVN Mac Signer được thiết kế để tương tác. Sự xuất hiện của chúng không hàm ý bất kỳ
sự bảo trợ hay hợp tác nào.

## Không bảo hành

Phần mềm được cung cấp "NGUYÊN TRẠNG", không kèm bảo hành dưới bất kỳ hình thức
nào, dù minh thị hay ngụ ý, như nêu trong [LICENSE](LICENSE). Tác giả và những
người đóng góp không chịu trách nhiệm cho bất kỳ khiếu nại, thiệt hại hay nghĩa
vụ nào phát sinh từ việc sử dụng phần mềm.

## Hiệu lực pháp lý của chữ ký

HVN Mac Signer là công cụ kỹ thuật để tạo và kiểm tra chữ ký số. Phần mềm không và
không thể bảo đảm rằng chữ ký tạo ra là hợp lệ về mặt pháp lý, được chấp nhận
làm chứng cứ, hay được bất kỳ cổng dịch vụ, cơ quan hoặc đối tác nào chấp nhận.
Hiệu lực pháp lý của chữ ký điện tử phụ thuộc vào chứng thư, tổ chức cấp, pháp
luật hiện hành và chính sách của bên nhận tài liệu. Người dùng tự chịu trách
nhiệm xác nhận rằng chứng thư, thiết bị và quy trình của mình đáp ứng các yêu
cầu đó.

Dấu thời gian RFC 3161 là tuỳ chọn và mặc định tắt; khi bật, dấu thời gian do máy
chủ dấu thời gian người dùng chọn cấp, và ứng dụng kiểm chữ ký của token nhưng
không kiểm chuỗi chứng thư của máy chủ đó. Những phần sau chưa được thực hiện
trong phiên bản hiện tại: kiểm tra đầy đủ chuỗi chứng thư và kiểm tra thu hồi
(OCSP / CRL).
Một chứng thư còn trong thời hạn hiệu lực, chỉ riêng điều đó, không đồng nghĩa
đáng tin cậy hay chưa bị thu hồi.

## Thiết bị, token và middleware

Hỗ trợ thiết bị đang ở mức thử nghiệm. Nhận được đầu đọc, liệt kê được token,
hay đọc được chứng thư không đồng nghĩa việc ký bằng PIN, gia hạn hay cấp lại sẽ
thành công trên thiết bị thật. Mỗi tổ hợp tổ chức chứng thực, mẫu thiết bị,
firmware, hệ điều hành và kiến trúc CPU đều phải được kiểm chứng riêng.

HVN Mac Signer không bao giờ lưu PIN, mật khẩu hay khóa riêng, không tự thử PIN hay
PIN mặc định, và không ghi hay xóa dữ liệu trên thiết bị. Nhập sai PIN quá nhiều
lần có thể khóa token; rủi ro đó thuộc về bản thân thiết bị, không phải phần mềm
này.

Middleware của nhà cung cấp (thư viện PKCS#11, driver USB
hoặc CCID) vẫn chịu sự điều chỉnh theo giấy phép của nhà cung cấp đó. Việc phân
phối lại chúng trong bản portable thuộc trách nhiệm của bạn và có thể cần sự cho
phép của nhà cung cấp.

## Trách nhiệm của người dùng

Bạn chịu trách nhiệm sử dụng HVN Mac Signer một cách hợp pháp, nắm giữ quyền hợp lệ
đối với chứng thư và thiết bị mình dùng, tuân thủ điều khoản của các hệ thống
mình kết nối, và kiểm tra mọi tài liệu đã ký trước khi tin dùng.
