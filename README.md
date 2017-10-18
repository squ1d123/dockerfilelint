This is a fork from replicatedhq/dockerfilelint

This creates a smaller docker image based on alpine

It has been reduced from 1GB to 30MB

It has also been modified to take standard input.

### Usage:
`docker run --rm -i squ1d12d/dockerfilelint < Dockerfile`

or 

```
docker run --rm -i squ1d12d/dockerfilelint << EOF
FROM .....
MAINTAINER ....
...
...
EOF
```

or 

`docker run --rm -i squ1d12d/dockerfilelint <<< FROM ...`
