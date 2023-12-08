# Ubuntu docker-in-dockerのテスト

## Usage

```bash
sudo docker compose up -d
sudo docker attach ...
docker run hello-world
```

## Synopsis

Ubuntuのイメージでdind(docker-in-docker)を行うための雛形です.

## 留意事項

- dockerの起動にsystemctlは使用不可
