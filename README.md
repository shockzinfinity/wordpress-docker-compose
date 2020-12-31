# wordpress-docker-compose
docker-compose 를 통한 wordpress site 생성

## prerequisite

```bash
$ mkdir dataredis dbdata wordpress
$ chmod 777 wordpress
$ docker-compose up -d
```
```bash
# .env 파일은 적절하게 수정 후
$ mv ./.env.sample ./.env
```

- nginx reverse proxy + letsencrypt 구성 참고: [nginx reverse proxy containerizing](https://shockzinfinity.github.io/dev-log/nginx.html#nginx-reverse-proxy-containerizing)
- `docker-compose.yml` 상의 networks 부분은 reverse proxy 가 설정된 네트워크에 포함되어야 동작됨
