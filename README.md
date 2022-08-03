# XrayR-script
A Xray backend framework that can easily support many panels.

# R.I.P XrayR

Một khung công tác back-end dựa trên Xray, hỗ trợ các giao thức V2ay, Trojan, Shadowsocks, cực kỳ dễ mở rộng và hỗ trợ kết nối nhiều bảng điều khiển

# Hướng dẫn chi tiết

[hướng dẫn](https://crackair.gitbook.io/xrayr-project/)

# Cài đặt chính

```
bash <(curl -Ls https://raw.githubusercontent.com/CatPort/XrayR-script/master/install.sh)
```

# Cài đặt Docker
```
docker pull mikumiku1/xrayr:latest && docker run --restart=always --name xrayr -d -v ${PATH_TO_CONFIG}/config.yml:/etc/XrayR/config.yml --network=host mikumiku1/xrayr:latest
```
# Cài đặt Docker compose (khuyến nghị)
0. Cài đặt docker-compose: 
```
curl -fsSL https://get.docker.com | bash -s docker
curl -L "https://github.com/docker/compose/releases/download/1.26.1/docker-compose-$(uname -s)-$(uname -m)" -o /usr/local/bin/docker-compose
chmod +x /usr/local/bin/docker-compose
```

1. `git clone https://github.com/CatPort/XrayR-script`
2. `cd XrayR-script`
3. Chỉnh sửa cấu hình。
Định dạng cơ bản của tệp cấu hình như sau. Có thể thêm nhiều bảng và nhiều thông tin cấu hình nút trong Nodes cùng một lúc. Chỉ cần thêm các mục Nodes ở cùng một định dạng.。
4. Khởi động docker：`docker-compose up -d`
5. Để xem nhật ký, vui lòng sử dụng：`docker-compose logs`

## Nâng cấp Docker compose
Thực thi trong thư mục docker-compo.yml：
```
docker-compose pull
docker-compose up -d
```

# Một lần nữa, tôi xin chân thành cảm ơn Crackair, tác giả gốc của XrayR.
