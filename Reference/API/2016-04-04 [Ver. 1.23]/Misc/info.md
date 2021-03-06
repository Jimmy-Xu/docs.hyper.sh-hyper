# Display Hyper.sh system-wide information

`GET /info`

Display Hyper.sh system-wide information

**Example request**:

    GET /info HTTP/1.1

**Example response**:

    HTTP/1.1 200 OK
    Content-Type: application/json

    {
        "Architecture": "x86_64",
        "Containers": 11,
        "ContainersRunning": 7,
        "ContainersStopped": 3,
        "ContainersPaused": 1,
        "CpuCfsPeriod": true,
        "CpuCfsQuota": true,
        "Debug": false,
        "DiscoveryBackend": "",
        "DockerRootDir": "",
        "Driver": "",
        "DriverStatus": [[""]],
        "Plugins": {
            "Volume": [
                ""
            ],
            "Network": [
                "null",
                "host",
                "bridge"
            ]
        },
        "ExecutionDriver": "hyper",
        "ExperimentalBuild": false,
        "HttpProxy": "",
        "HttpsProxy": "",
        "ID": "",
        "IPv4Forwarding": true,
        "Images": 16,
        "IndexServerAddress": "https://index.docker.io/v1/",
        "InitPath": "",
        "InitSha1": "",
        "KernelVersion": "3.12.0-1-amd64",
        "Labels": [
            "storage=ssd"
        ],
        "MemTotal": 2099236864,
        "MemoryLimit": true,
        "NCPU": 1,
        "NEventsListener": 0,
        "NFd": 11,
        "NGoroutines": 21,
        "Name": "prod-server-42",
        "NoProxy": "9.81.1.160",
        "OomKillDisable": true,
        "OSType": "linux",
        "OomScoreAdj": 500,
        "OperatingSystem": "HyperStart",
        "RegistryConfig": {
            "IndexConfigs": {
                "docker.io": {
                    "Mirrors": null,
                    "Name": "docker.io",
                    "Official": true,
                    "Secure": true
                }
            },
            "InsecureRegistryCIDRs": [ ]
        },
        "SwapLimit": false,
        "SystemTime": "2015-03-10T11:11:23.730591467-07:00"
        "ServerVersion": "1.9.0"
    }

Status Codes:

-   **200** – no error
-   **500** – server error
