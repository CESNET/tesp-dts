# DTS

Example of data transfer server using HTTP, S3 and FTP.

Project uses Docker and deploy 4 containers:  
- s3
- ftp
- http
- clients

The `clients` container contains clients for the used protocols. So you doesn't need to install the clients on you local computer to test it.

## Deploy

`docker compose up -d`

## Examples of usage

### HTTP

Upload  
`curl -i -X POST -F "file=@up-file.txt;filename=file.txt" localhost:5000/upload`

Download  
`curl -X GET -o down-file.txt localhost:5000/download/file.txt`

### S3
Create bucket  
`s3cmd mb s3://test`

Upload  
`s3cmd put file.txt s3://file.txt`

Download  
`s3cmd get s3://text/file.txt file.txt`

List all object in all buckets  
`s3cmd la`

### FTP
TODO
