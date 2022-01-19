# highload-homework-20

**Horizontal Sharding**

- Create 3 docker containers: postgresql-b, postgresql-b1, postgresql-b2
- Setup horizontal sharding as it’s described in this lesson
- Insert 1 000 000 rows into books
- Measure performance
- Do the same without sharding
- Compare performance

## Installation 

```
git clone https://github.com/god-of-north/highload-homework-20.git
cd highload-homework-20
docker-compose up
cat shard-magic.sql | docker exec -i highload-homework-20_postgres-b_1 psql postgresql://postgres:postgres@postgres-b:5432/postgres
```

https://www.kaggle.com/brosen255/goodreads-books

