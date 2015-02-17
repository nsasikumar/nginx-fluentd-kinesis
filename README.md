# nginx-fluentd-kinesis
Add fluentd kinesis logging to nginx-php-fail2ban

To build:
docker build -t nsasikumar/nginx-fluentd .

To run:
docker run -d -e AWS_ACCESS_KEY_ID=<aws-access-key> -e AWS_SECRET_ACCESS_KEY=<aws-secret-access-key> -e KINESIS_STREAM=<kinesis-stream-name> -e KINESIS_REGION=<kinesis-region> nsasikumar/nginx-fluend
