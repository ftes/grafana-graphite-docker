1. `docker-compose up`
2. login to [grafana](http://localhost:3000) (admin:admin)
3. setup data source: `http://<graphite-container-ip>:80`, basic auth (guest:guest)
  - have to use container IP, as the hostname won't work
  - find IP with `docker inspect grafanagraphite_graphite_1 | grep IPAddress`
4. (optional) login to [graphite](http://localhost:8080) (guest:guest)
