# Steps to deploy votingapp

1.  **Create votingapp namespace**

- ``` k create ns votingapp ```

2. **Create db deployment manifest**
- ``` k create deployment db -n votingapp --image=postgres:16-alpine ```
- ``` k set env deployment/db -n votingapp POSTGRES_USER=postgres POSTGRES_PASSWORD=postgres --dry-run=client -o yaml > db/db-deployment.yaml ```
- ``` k apply -f db/db-deployment.yaml ```