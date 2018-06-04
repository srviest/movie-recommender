# movie-recommender
Practice of building personalized movie recommenadation service using Flask and Spark
Referrence: [A scalable on-line movie recommender using Spark and Flask](https://github.com/jadianes/spark-movie-lens)


# Usage
## Submit Spark job
```
spark-submit --master 'local[*]'  --total-executor-cores 14 --executor-memory 6g  server.py
```

## Get top ratings given user_id
```
http://0.0.0.0:<int:port>/<int:user_id>/ratings/top/<int:count>
```

## Get ratings for moive_id given user_id
```
http://0.0.0.0:<int:port>/<int:user_id>/ratings/<int:movie_id>
```
