Node.js application with Nginx proxy and Redis database
.
├── README.md
├── compose.yaml
├── nginx
│   ├── Dockerfile
│   └── nginx.conf
└── web
    ├── Dockerfile
    ├── package.json
    └── server.js

The compose file defines an application with four services redis, nginx, web1 and web2. When deploying the application, docker compose maps port 80 of the nginx service container to port 80 of the host as specified in the file.    