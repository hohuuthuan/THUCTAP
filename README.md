# Chạy back end
B1: Cài đặt .NET 6.0.x
B2: Mở SQL Server, kết nối
B3: Mở file MobileShopAPI.sln bằng Microsoft Visual Studio (Tím)
B4: Làm theo video là đc
-- Nếu lỗi chạy SQL thì cứ sửa như video đã hướng dẫn là đc
-- Chạy API nếu bị "Không bảo mật" thì dán đường link ra Chrome là được


# Mô tả bảng:
Quản lý người dùng và quyền truy cập:
    dbo.AspNetUsers: Thông tin chi tiết về người dùng.
    dbo.AspNetRoles: Các vai trò mà người dùng có thể đảm nhận.
    dbo.AspNetUserRoles: Mối quan hệ giữa người dùng và vai trò.
    dbo.AspNetUserClaims, dbo.AspNetUserLogins, dbo.AspNetUserTokens: Các thông tin liên quan đến quyền truy cập và xác thực người dùng.

Quản lý sản phẩm:
    dbo.product: Thông tin chi tiết về các sản phẩm.
    dbo.category: Các loại sản phẩm.
    dbo.brand: Thương hiệu của sản phẩm.
    dbo.color, dbo.size: Các thuộc tính của sản phẩm như màu sắc, kích cỡ.
    dbo.image: Hình ảnh của sản phẩm.
    dbo.marked_product: Có thể là danh sách sản phẩm được đánh dấu hoặc yêu thích.

Quản lý đơn hàng:
    dbo.order: Thông tin về các đơn hàng.
    dbo.product_order: Mối quan hệ giữa sản phẩm và đơn hàng, thường chứa thông tin về số lượng sản phẩm trong mỗi đơn hàng.
    dbo.shipping_address: Địa chỉ giao hàng cho mỗi đơn hàng.

Quản lý giao dịch và gói dịch vụ:
    dbo.internal_transaction, dbo.transaction: Các giao dịch nội bộ hoặc giao dịch chung.
    dbo.subscription_package: Các gói dịch vụ mà người dùng có thể đăng ký.
    dbo.active_subscription: Các gói dịch vụ mà người dùng đang đăng ký.

Quản lý đánh giá và báo cáo:
    dbo.user_rating: Đánh giá của người dùng về sản phẩm hoặc dịch vụ.
    dbo.report, dbo.report_category: Các báo cáo và loại báo cáo liên quan.

Quản lý tiền ảo:
    dbo.coin_action: Các hành động liên quan đến tiền ảo.
    dbo.coin_package: Các gói tiền ảo mà người dùng có thể mua.