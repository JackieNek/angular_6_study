# I. Kiến trúc
## 1. Tổng quan
  * **Angular** dùng để xây dựng các ứng dụng client. 
  * **Angular** được viết bằng *TypeScript*. 
  * Các khối cơ bản của ứng dụng **Angular** được xây dựng là *NgModules*, là môi trường cho các *Component*. 
  * *NgModules* chứa các mã lệnh liên quan đến chức năng. Ứng dụng **Angular** được xây dựng bởi tập các *NgModules*. 
  * Một ứng dụng **Angular** luôn có ít nhất một *Module* gốc cho phép *bootstrapping* và có nhiều *Feature Module*. 
    * **Component** là các *views*, là tập hợp các thành phần giao diện mà **Angular** có thể sửa đổi logic và data.
    * **Component** sử dụng các **Service**, cung cấp chức năng cụ thể mà không thông qua trực tiếp với các *views*. Các **Service** có thể sử dụng các *dependencies*, giúp chia nhỏ mã nguồn cho dễ quản lý, đồng thời có thể *inject* các **Service** và các **Component** khác nhau, tái sử dụng mã nguồn
  * Các **Component** và **Service** đơn giản chỉ là các lớp cung cấp các hiệu ứng và *metadata* cho các *template*.
    * Các *metadata* của **Component** đi kèm với các mẫu template là các views được kết hợp bởi *HTML* với các *directive* và *binding markup* để thay đổi *HTML* trước khi được *render* và *display*
    * Các *metadata* của **Service** cung cấp cho thông tin mà **Angular** cần để cung cấp cho các **Component** các thông qua việc *dependency injection*