<p style="text-align: center;">uni-db-security</p>
<p style="text-align: center;">This repository will hold scripts and configurations for the DB Security course.</p>

### Quick install
```
curl -fsSL https://get.docker.com -o get-docker.sh
sh get-docker.sh
rm get-docker.sh
docker login container-registry.oracle.com
docker pull container-registry.oracle.com/database/enterprise:23.26.1.0
```

### Useful commands

```
sudo chown -R 54321:54321 ./oradata
```
```
docker exec -it oracle-db bash
```
```
sqlplus sys@//localhost:1521/ORCLCDB as sysdba
```
```
docker exec -it oracle-db sqlplus / as sysdba
```
```
sqlplus sys/<passwd>@//localhost:<port>/<sid> as sysdba
```
```
docker exec oracle-db ./setPassword.sh <new passwd>
```
