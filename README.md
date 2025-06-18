# Gửi và nhận email thông qua giao thức bảo mật PGP
[📄 Lý thuyết về giao thức PGP](./PGP_Protocol.md)

## Kịch bản thử nghiệm
  Trong quá trình trao đổi email, Alice (bên gửi) muốn gửi một email đảm bảo tính bí mật, toàn vẹn đến Tai (bên nhận). Hai người sử dụng Thunderbird kết hợp với giao thức bảo mật PGP. Đầu tiên, mỗi người tạo một cặp khóa PGP gồm khóa riêng và khóa công khai, sau đó trao đổi khóa công khai cho nhau và nhập vào hệ thống (keyring). Tiếp theo:
- Alice cần thực hiện:
    1. Tạo email cần gửi
    2. Sừ dụng khóa bí mật của mình để ký số
    3. Sử dụng khóa công khai của Tai để mã hóa email
    4. Sau đó gửi email đi
- Tai sau khi nhận email:
    1. Sử dụng khóa bí mật của mình để giải mã email
    2. Sử dụng khóa công khai của Alice để xác nhận email có bị sửa đổi không.
