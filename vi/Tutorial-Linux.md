# Cài đặt Nest.js và các phần mềm liên quan

Tài liệu dành cho Linux.

Hệ điều hành khác: [Windows](Tutorial-Windows.md) - [macOS](Tutorial-macOS.md)

## Mục lục

- [Cài đặt Nest.js và các phần mềm liên quan](#cài-đặt-nestjs-và-các-phần-mềm-liên-quan)
  - [Mục lục](#mục-lục)
  - [Cài đặt](#cài-đặt)
    - [Node.js](#nodejs)
    - [Nest.js](#nestjs)
    - [Postman](#postman)
    - [Database](#database)
  - [Bước kế tiếp](#bước-kế-tiếp)

## Cài đặt

### Node.js

[Node.js](https://nodejs.org/en) là một môi trường server để viết các ứng dụng bằng ngôn ngữ Javascript. Nest.js là framework chạy trên Node.js.

Để cài đặt Node.js:

- Tải Node.js binaries ở [https://nodejs.org/en/download](https://nodejs.org/en/download)
- Giải nén file đã tải
- Copy các thư mục trong thư mục đã giải nén vào `/usr`

Hoặc cài đặt từ các hệ thống quản lý gói phần mềm (package manager) theo hướng dẫn: [https://nodejs.org/en/download/package-manager](https://nodejs.org/en/download/package-manager)

Sau khi cài đặt, kiểm tra bằng lệnh sau, nếu hiển thị các phiên bản của `npm` và `node` thì việc cài đặt thành công.

```sh
node --version
npm --version
```

### Nest.js

Cài đặt [Nest.js](https://nestjs.com/) bằng lệnh

```sh
npm i -g @nestjs/cli
```

Sau khi cài đặt, kiểm tra bằng lệnh, nếu hiển thị phiên bản của `nest` thì cài đặt thành công.

```sh
nest --version
```

### Postman

[Postman](https://www.postman.com/) là công cụ để thao tác với API, nhằm mục đích kiểm thử và xây dựng API.

![Source: postman.com](../images/postman-product-screen.svg)

Để cài đặt công cụ:

- Tải installer ở [https://www.postman.com/downloads/](https://www.postman.com/downloads/)
- Giải nén file đã tải
- Tạo desktop icon và lưu ở `~/.local/share/applications/Postman.desktop` với nội dung file như sau (trong đó, thay thế `/path/to/Downloads` thành đường dẫn thư mục chứa thư mục được giải nén):

```txt
[Desktop Entry]
Encoding=UTF-8
Name=Postman
Exec=/path/to/Downloads/Postman/app/Postman %U
Icon=/path/to/Downloads/Postman/app/resources/app/assets/icon.png
Terminal=false
Type=Application
Categories=Development;
```

Hoặc sử dụng lệnh (yêu cầu [Snap store](https://snapcraft.io/)):

```sh
snap install postman
```

Lưu ý:

- Các phiên bản Linux hỗ trợ: Ubuntu 14.04 (và mới hơn), Fedora 24, Debian 8 (và mới hơn).
- Cần có quyền đọc và ghi ở thư mục `~/.config` để Postman lưu thông tin.
- Với Ubuntu 18, cần cài đặt package `libgconf-2-4` với lệnh `apt-get install libgconf-2-4`
- Chi tiết: [https://learning.postman.com/docs/getting-started/installation-and-updates/#installing-postman-on-linux](https://learning.postman.com/docs/getting-started/installation-and-updates/#installing-postman-on-linux)

### Database

Các ứng dụng Nest.js có thể cần làm việc với cơ sở dữ liệu. Để cài đặt một số cơ sở dữ liệu thông dụng, vui lòng tham khảo các liên kết sau:

- MySQL: [https://dev.mysql.com/doc/mysql-installation-excerpt/8.0/en/](https://dev.mysql.com/doc/mysql-installation-excerpt/8.0/en/)
- MongoDB: [https://www.mongodb.com/docs/manual/installation/#mongodb-installation-tutorials](https://www.mongodb.com/docs/manual/installation/#mongodb-installation-tutorials)
- PostgreSQL: [https://www.postgresql.org/docs/current/installation.html](https://www.postgresql.org/docs/current/installation.html)

## Bước kế tiếp

[Băt đầu sử dụng Nest.js](../Readme.md#bắt-đầu-sử-dụng-nestjs)
