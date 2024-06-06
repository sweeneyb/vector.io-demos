# Starting
## My start
Download from https://vector.dev/download/  The .gitinore is set up for this:

```
wget https://packages.timber.io/vector/0.38.0/vector-0.38.0-x86_64-unknown-linux-gnu.tar.gz
tar -xvzf vector-0.38.0-x86_64-unknown-linux-gnu.tar.gz
rm vector-0.38.0-x86_64-unknown-linux-gnu.tar.gz
```

```./vector-x86_64-unknown-linux-gnu/bin/vector -c vector.yaml``` will show some demo output.

## Quickstart
https://vector.dev/docs/setup/quickstart/

## Container
alias vector='docker run -i -v $(pwd)/:/etc/vector/ --rm timberio/vector:0.34.1-debian'

# More examples
./vector-x86_64-unknown-linux-gnu/bin/vector -c prom-tests.yaml 


curl -i -H "Content-Type: application/json" -H "dest_bucket: foo" --data '{"baz":"bonk"}' http://foo.localhost:8080 --connect-to foo.localhost:8080:127.0.0.1:8080

curl -i -H "Content-Type: application/json" -H "dest_bucket: foo" --data @short.json http://foo.localhost:8080 --connect-to foo.localhost:8080:127.0.0.1:8080
curl -i -H "Content-Type: application/json" -H "dest_bucket: foo" --data @long.json http://foo.localhost:8080 --connect-to foo.localhost:8080:127.0.0.1:8080


### metric length
curl -s localhost:8082/metrics|grep -v \#|wc -l
366