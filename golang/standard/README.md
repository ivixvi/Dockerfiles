# golang開発環境（仮）
## use
1. `docker-compose up {--build}`
    - コンテナの起動と永続化，必要に応じてリビルドする．
    - volumeは`./src:/go/src/work`にしてある．
1. `docker exec -it {continer_id} bash`
    - `docker ps`でコンテナIDを把握して，コンテナのシェルに入る．
    - `golang:latest`をベースとした環境になっており`go`コマンドが使用できる．
1. `go run main.go`
    - `Hello, World!`