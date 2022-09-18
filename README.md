docker build -t hadoop .

docker run -dp 3000:3000 hadoop

# start interactive shell in running container
docker exec -it hadoop

# once shell has started run hadoop "pi" example job
hadoop jar $HADOOP_HOME/share/hadoop/mapreduce/hadoop-mapreduce-examples-2.8.1.jar pi 10 100