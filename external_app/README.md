# Ứng dụng bên ngoài kết nối Odoo

Ứng dụng này nằm ngoài Odoo và kết nối vào Odoo bằng XML-RPC External API.

## Cách chạy

1. Mở Odoo tại `http://localhost:8069`.
2. Chạy app ngoài:

```bash
cd /home/quang/odoo-fitdnu
python3 external_app/odoo_external_app.py
```

3. Mở trình duyệt: `http://localhost:8070`
4. Nhập thông tin:
   - Odoo URL: `http://localhost:8069`
   - Database: `admin`
   - User: `admin@example1.com`
   - Mật khẩu: mật khẩu đăng nhập Odoo
5. Bấm `Kết nối`.

## Chức năng demo

- Xem danh sách khách hàng từ Odoo.
- Xem danh sách văn bản đến/đi từ Odoo, gồm cả cột AI đề xuất.
- Tạo khách hàng mới từ ứng dụng bên ngoài.
- Quay lại Odoo để thấy khách hàng vừa tạo xuất hiện trong `QLKH / Hồ sơ khách hàng`.

## Ý nghĩa với yêu cầu nâng cao

Tính năng này đáp ứng yêu cầu: kết nối Odoo với ứng dụng bên ngoài theo tài liệu External API của Odoo 15.

Nguồn tham khảo: https://www.odoo.com/documentation/15.0/developer/reference/external_api.html
