# Vue + Pocketbase template

go (pocket base) as backend and vue as frontend

## Build and Run

Build

```bash
docker build -t template .
```


Run. You need to specify a pesistant volume to store the data (`./pb_data`)

```bash
docker run -p 8080:8080 -v ./pb_data:/pb_data template
```

## Run locally (dev mode)

### Go Backend

```bash
go run maio.go
# or
air
```

### Vue Frontend

```bash
VITE_POCKETBASE_URL=http://localhost:8090 npm run dev
```