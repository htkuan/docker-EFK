# launch

```bash
docker-compose build
docker-compose up -d
```

# access kibana
[localhost:5601](http://localhost:5601)

index pattern need change to ```fluentd-*```

# send request to create logs

1. Collect web logs
```bash
repeat 10 curl http://localhost:80/
```
2. Push directly
```bash
curl -X POST -d 'json={"json":"message"}' http://localhost:9880/sample.test
```