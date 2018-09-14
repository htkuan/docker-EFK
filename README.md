# launch

```bash
docker-compose up -d
```

# access kibana
[localhost:5601](http://localhost:5601)

index pattern need change to ```fluentd-*```

# send request to create logs

```bash
repeat 10 curl http://localhost:80/
```