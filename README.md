# README

## Start Service
```
docker-compose up
```

or

```
docker-compose up -d
```

## Explore your container
After start service,
```
docker-compose exec django bash
```

## Stop Service
```
docker-compose down
```

## SetUp for MySQL User

### Login to MySQL Container
```
docker-compose exec db bash
```

### Change MySQL User setting
```
mysql -u root -p

mysql > ALTER USER 'django'@'%' IDENTIFIED WITH mysql_native_password BY 'django'; 
mysql > FLUSH PRIVILEGES;
```
