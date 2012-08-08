Amazon S3 produces a lot of small log files per day. The log compactor downloads the logs, merges them together into one file per day, applies bzip2 compression, reuploads the compressed file and deletes the old log files.
It is originally written by Krzysztof Kowalczyk (http://blog.kowalczyk.info/article/Compacting-s3-aws-logs.html) and slightly modified by me.
