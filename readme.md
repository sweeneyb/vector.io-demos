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
