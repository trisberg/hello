# hello

## build

```
pack build gcr.io/cf-sandbox-trisberg/hello-handler --path . --builder us.gcr.io/daisy-284300/kn-fn/builder:0.0.6 --publish
```

## deploy

```
kn service create hello --image gcr.io/cf-sandbox-trisberg/hello-handler
```

## invoke

```
curl -H 'Content-Type: application/json' http://hello.default.apps.34.67.89.126.nip.io/hello -d Tanzu
```
