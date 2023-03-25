# Hướng dẫn cài đặt và sử dụng Nest.js

Nest.js là một trong những Node.js framework, nhằm giúp việc xây dựng các hệ thống backend nhanh chóng, hiệu quả và dễ dàng mở rộng trong tương lai.

Với người mới bắt đầu, việc cài đặt để chạy được và sử dụng Nestjs có thể tốn nhiều thời gian, do đó, tài liệu này sẽ hướng dẫn ngắn gọn cách cài đặt Node.js và Nest.js, cùng với một số công cụ để hỗ trợ việc xây dựng hệ  thống backend, chẳng hạn như Postman để kiểm thử API. Cuối tài liệu bao gồm cách khởi tạo và làm việc với dự án Nest.js.

## Mục lục

- [Hướng dẫn cài đặt và sử dụng Nest.js](#hướng-dẫn-cài-đặt-và-sử-dụng-nestjs)
  - [Mục lục](#mục-lục)
  - [Cài đặt Nest.js và các phần mềm liên quan](#cài-đặt-nestjs-và-các-phần-mềm-liên-quan)
  - [Bắt đầu sử dụng Nest.js](#bắt-đầu-sử-dụng-nestjs)
    - [Khởi tạo dự án](#khởi-tạo-dự-án)
    - [Tạo một module](#tạo-một-module)
    - [Tạo một controller](#tạo-một-controller)
    - [Tạo một service](#tạo-một-service)
    - [Tạo một CRUD resource](#tạo-một-crud-resource)
  - [Liên kết tham khảo](#liên-kết-tham-khảo)


## Cài đặt Nest.js và các phần mềm liên quan

Chọn hệ điều hành bạn đang sử dụng: [Windows](os/Tutorial-Windows.md) - [Linux](os/Tutorial-Linux.md) - [macOS](os/Tutorial-macOS.md)

## Bắt đầu sử dụng Nest.js

Phần này bao gồm các câu lệnh thường dùng để khởi tạo và làm việc với dự án Nest.js

### Khởi tạo dự án

Các câu lệnh sau sẽ khởi tạo dự án mới, sau đó build và chạy dự án đã tạo.

```sh
nest new my-nest-project
cd my-nest-project
npm run start:dev
```

Truy cập http://localhost:3000 trên trình duyệt để xem ứng dụng đã được chạy.

### Tạo một module

Một dự án được tổ chức thành nhiều module. Mỗi module đóng gói những thành phần liên quan với nhau.

Để tạo module, sử dụng câu lệnh

```sh
nest generate module my-module
```

hoặc

```sh
nest g mo my-module
```

### Tạo một controller

Controller là thành phần xử lý các request và trả về các response cho client.

Để tạo controller, sử dụng câu lệnh

```sh
nest generate controller my-controller
```

hoặc

```sh
nest g co my-controller
```

### Tạo một service

Nest.js gồm một khái niệm quan trọng là provider, là một đối tượng có thể được injected thành dependency của đối tượng khác, tạo nên mối quan hệ giữa các đối tượng trong dự án. Trong đó, service là một loại provider thường dùng để xử lý logic, tương tác với các thực thể trong dự án Nest.js.

Để tạo service, sử dụng câu lệnh

```sh
nest generate service my-service
```

hoặc

```sh
nest g s my-service
```

### Tạo một CRUD resource

CRUD resource chỉ các tài nguyên, với các API để tạo (create), đọc (read), cập nhật (update) và xoá (delete) tài nguyên đó trong hệ thống.

Để tạo CRUD resource, sử dụng câu lệnh:

```sh
nest generate resource my-resource
```

hoặc

```sh
nest g res my-resource
```

## Liên kết tham khảo

- Trang documentation của Nest.js: https://docs.nestjs.com/
- Video hướng dẫn Nest.js: https://youtu.be/F_oOtaxb0L8
- Chi tiết về Nest CLI: https://docs.nestjs.com/cli/usages
- Hướng dẫn triển khai dự án Nest.js: 