### Read Me

In case it is helpful, below is a `docker inspect` of my ui_container

```
[
    {
        "Id": "9b44e54540a2d1c7298efc747db0324a5058761f4dbad9a8b56311627bd847b1",
        "Created": "2021-01-13T23:09:41.7587709Z",
        "Path": "tail",
        "Args": [
            "-f",
            "/dev/null"
        ],
        "State": {
            "Status": "running",
            "Running": true,
            "Paused": false,
            "Restarting": false,
            "OOMKilled": false,
            "Dead": false,
            "Pid": 10553,
            "ExitCode": 0,
            "Error": "",
            "StartedAt": "2021-01-13T23:09:42.2899142Z",
            "FinishedAt": "0001-01-01T00:00:00Z"
        },
        "Image": "sha256:97c8116710411e2af17409c1cf7bd954b8b84b265207ba42fa9934183469738f",
        "ResolvConfPath": "/var/lib/docker/containers/9b44e54540a2d1c7298efc747db0324a5058761f4dbad9a8b56311627bd847b1/resolv.conf",
        "HostnamePath": "/var/lib/docker/containers/9b44e54540a2d1c7298efc747db0324a5058761f4dbad9a8b56311627bd847b1/hostname",
        "HostsPath": "/var/lib/docker/containers/9b44e54540a2d1c7298efc747db0324a5058761f4dbad9a8b56311627bd847b1/hosts",
        "LogPath": "/var/lib/docker/containers/9b44e54540a2d1c7298efc747db0324a5058761f4dbad9a8b56311627bd847b1/9b44e54540a2d1c7298efc747db0324a5058761f4dbad9a8b56311627bd847b1-json.log",
        "Name": "/ui_container",
        "RestartCount": 0,
        "Driver": "overlay2",
        "Platform": "linux",
        "MountLabel": "",
        "ProcessLabel": "",
        "AppArmorProfile": "",
        "ExecIDs": null,
        "HostConfig": {
            "Binds": [
                "C:\\Users\\jabbott\\vsdbg\\vs2017u5:/remote_debugger:rw",
                "C:\\Users\\jabbott\\AppData\\Roaming\\Microsoft\\UserSecrets:/root/.microsoft/usersecrets:ro",
                "C:\\Users\\jabbott\\AppData\\Roaming\\ASP.NET\\Https:/root/.aspnet/https:ro",
                "C:\\Users\\jabbott\\Documents\\Repositories\\Prototypes\\DockerEnvTest:/src:rw",
                "C:\\Users\\jabbott\\.nuget\\packages:/root/.nuget/packages:ro",
                "C:\\Users\\jabbott\\Documents\\Repositories\\Prototypes\\DockerEnvTest\\UI:/app:rw"
            ],
            "ContainerIDFile": "",
            "LogConfig": {
                "Type": "json-file",
                "Config": {}
            },
            "NetworkMode": "TestNetwork",
            "PortBindings": {
                "443/tcp": [
                    {
                        "HostIp": "",
                        "HostPort": ""
                    }
                ],
                "80/tcp": [
                    {
                        "HostIp": "",
                        "HostPort": "80"
                    },
                    {
                        "HostIp": "",
                        "HostPort": ""
                    }
                ]
            },
            "RestartPolicy": {
                "Name": "",
                "MaximumRetryCount": 0
            },
            "AutoRemove": false,
            "VolumeDriver": "",
            "VolumesFrom": [],
            "CapAdd": null,
            "CapDrop": null,
            "Capabilities": null,
            "Dns": null,
            "DnsOptions": null,
            "DnsSearch": null,
            "ExtraHosts": null,
            "GroupAdd": null,
            "IpcMode": "private",
            "Cgroup": "",
            "Links": null,
            "OomScoreAdj": 0,
            "PidMode": "",
            "Privileged": false,
            "PublishAllPorts": false,
            "ReadonlyRootfs": false,
            "SecurityOpt": null,
            "UTSMode": "",
            "UsernsMode": "",
            "ShmSize": 67108864,
            "Runtime": "runc",
            "ConsoleSize": [
                0,
                0
            ],
            "Isolation": "",
            "CpuShares": 0,
            "Memory": 0,
            "NanoCpus": 0,
            "CgroupParent": "",
            "BlkioWeight": 0,
            "BlkioWeightDevice": null,
            "BlkioDeviceReadBps": null,
            "BlkioDeviceWriteBps": null,
            "BlkioDeviceReadIOps": null,
            "BlkioDeviceWriteIOps": null,
            "CpuPeriod": 0,
            "CpuQuota": 0,
            "CpuRealtimePeriod": 0,
            "CpuRealtimeRuntime": 0,
            "CpusetCpus": "",
            "CpusetMems": "",
            "Devices": null,
            "DeviceCgroupRules": null,
            "DeviceRequests": null,
            "KernelMemory": 0,
            "KernelMemoryTCP": 0,
            "MemoryReservation": 0,
            "MemorySwap": 0,
            "MemorySwappiness": null,
            "OomKillDisable": false,
            "PidsLimit": null,
            "Ulimits": null,
            "CpuCount": 0,
            "CpuPercent": 0,
            "IOMaximumIOps": 0,
            "IOMaximumBandwidth": 0,
            "MaskedPaths": [
                "/proc/asound",
                "/proc/acpi",
                "/proc/kcore",
                "/proc/keys",
                "/proc/latency_stats",
                "/proc/timer_list",
                "/proc/timer_stats",
                "/proc/sched_debug",
                "/proc/scsi",
                "/sys/firmware"
            ],
            "ReadonlyPaths": [
                "/proc/bus",
                "/proc/fs",
                "/proc/irq",
                "/proc/sys",
                "/proc/sysrq-trigger"
            ]
        },
        "GraphDriver": {
            "Data": {
                "LowerDir": "/var/lib/docker/overlay2/5718720dade33e0b0d55e785e11d3f5c9e3f3378ba6e418f031c7ad23100037e-init/diff:/var/lib/docker/overlay2/40ce7487105c7f442cd7f2f6732028c85e8364f53d3f04a5eece078ef5a61915/diff:/var/lib/docker/overlay2/5729267b77f5c71d815f79f7016581d3b0e6514c0650df7c9e637fa3ad5f28bc/diff:/var/lib/docker/overlay2/1a45f91c3aff4bc2c3a54f5ce7717da7ccf38dd23dbbbd1395c701077847271a/diff:/var/lib/docker/overlay2/1915f8757d670fbb2c4d47910b0ecd77a6bd14878f538cf8ee73408a158d3178/diff:/var/lib/docker/overlay2/5835891efc35808b5e378c15b17981a31d7f52e3b04b4987795780952916d07c/diff:/var/lib/docker/overlay2/8c14e2296063705bf162ca33fbf661de37367cc44bf48751bdb3fb7bf3e8be3a/diff",
                "MergedDir": "/var/lib/docker/overlay2/5718720dade33e0b0d55e785e11d3f5c9e3f3378ba6e418f031c7ad23100037e/merged",
                "UpperDir": "/var/lib/docker/overlay2/5718720dade33e0b0d55e785e11d3f5c9e3f3378ba6e418f031c7ad23100037e/diff",
                "WorkDir": "/var/lib/docker/overlay2/5718720dade33e0b0d55e785e11d3f5c9e3f3378ba6e418f031c7ad23100037e/work"
            },
            "Name": "overlay2"
        },
        "Mounts": [
            {
                "Type": "bind",
                "Source": "C:\\Users\\jabbott\\AppData\\Roaming\\Microsoft\\UserSecrets",
                "Destination": "/root/.microsoft/usersecrets",
                "Mode": "ro",
                "RW": false,
                "Propagation": "rprivate"
            },
            {
                "Type": "bind",
                "Source": "C:\\Users\\jabbott\\AppData\\Roaming\\ASP.NET\\Https",
                "Destination": "/root/.aspnet/https",
                "Mode": "ro",
                "RW": false,
                "Propagation": "rprivate"
            },
            {
                "Type": "bind",
                "Source": "C:\\Users\\jabbott\\Documents\\Repositories\\Prototypes\\DockerEnvTest",
                "Destination": "/src",
                "Mode": "rw",
                "RW": true,
                "Propagation": "rprivate"
            },
            {
                "Type": "bind",
                "Source": "C:\\Users\\jabbott\\.nuget\\packages",
                "Destination": "/root/.nuget/packages",
                "Mode": "ro",
                "RW": false,
                "Propagation": "rprivate"
            },
            {
                "Type": "bind",
                "Source": "C:\\Users\\jabbott\\Documents\\Repositories\\Prototypes\\DockerEnvTest\\UI",
                "Destination": "/app",
                "Mode": "rw",
                "RW": true,
                "Propagation": "rprivate"
            },
            {
                "Type": "bind",
                "Source": "C:\\Users\\jabbott\\vsdbg\\vs2017u5",
                "Destination": "/remote_debugger",
                "Mode": "rw",
                "RW": true,
                "Propagation": "rprivate"
            }
        ],
        "Config": {
            "Hostname": "9b44e54540a2",
            "Domainname": "",
            "User": "",
            "AttachStdin": false,
            "AttachStdout": false,
            "AttachStderr": false,
            "ExposedPorts": {
                "443/tcp": {},
                "80/tcp": {}
            },
            "Tty": true,
            "OpenStdin": false,
            "StdinOnce": false,
            "Env": [
                "ASPNETCORE_ENVIRONMENT=Development",
                "ASPNETCORE_URLS=https://+:443;http://+:80",
                "DOTNET_USE_POLLING_FILE_WATCHER=1",
                "ASPNETCORE_LOGGING__CONSOLE__DISABLECOLORS=true",
                "NUGET_FALLBACK_PACKAGES=",
                "PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin",
                "DOTNET_RUNNING_IN_CONTAINER=true"
            ],
            "Cmd": null,
            "Image": "ui:dev",
            "Volumes": {
                "/app": {},
                "/remote_debugger": {},
                "/root/.aspnet/https": {},
                "/root/.microsoft/usersecrets": {},
                "/root/.nuget/packages": {},
                "/src": {}
            },
            "WorkingDir": "/app",
            "Entrypoint": [
                "tail",
                "-f",
                "/dev/null"
            ],
            "OnBuild": null,
            "Labels": {
                "com.docker.compose.config-hash": "ab7411f6e3a8a3630de0d29a7eaac657b9840c1a3417a32bb37872fc7115f229",
                "com.docker.compose.container-number": "1",
                "com.docker.compose.oneoff": "False",
                "com.docker.compose.project": "dockercompose769523303561097960",
                "com.docker.compose.project.config_files": "C:\\Users\\jabbott\\Documents\\Repositories\\Prototypes\\DockerEnvTest\\docker-compose.yml,C:\\Users\\jabbott\\Documents\\Repositories\\Prototypes\\DockerEnvTest\\docker-compose.override.yml,C:\\Users\\jabbott\\Documents\\Repositories\\Prototypes\\DockerEnvTest\\obj\\Docker\\docker-compose.vs.debug.g.yml",
                "com.docker.compose.project.working_dir": "C:\\Users\\jabbott\\Documents\\Repositories\\Prototypes\\DockerEnvTest",
                "com.docker.compose.service": "ui",
                "com.docker.compose.version": "1.27.4",
                "com.microsoft.created-by": "visual-studio",
                "com.microsoft.visual-studio.project-name": "UI",
                "com.microsoft.visualstudio.debuggee.arguments": " --additionalProbingPath /root/.nuget/packages  \"/app/bin/Debug/netcoreapp3.1/UI.dll\"",
                "com.microsoft.visualstudio.debuggee.killprogram": "/bin/sh -c \"if PID=$(pidof dotnet); then kill $PID; fi\"",
                "com.microsoft.visualstudio.debuggee.program": "dotnet",
                "com.microsoft.visualstudio.debuggee.workingdirectory": "/app"
            }
        },
        "NetworkSettings": {
            "Bridge": "",
            "SandboxID": "d3c68b7c52f062d7a186dd62a8491f7352e61a7d69c0acbdbb69d49000fddb6a",
            "HairpinMode": false,
            "LinkLocalIPv6Address": "",
            "LinkLocalIPv6PrefixLen": 0,
            "Ports": {
                "443/tcp": [
                    {
                        "HostIp": "0.0.0.0",
                        "HostPort": "49202"
                    }
                ],
                "80/tcp": [
                    {
                        "HostIp": "0.0.0.0",
                        "HostPort": "80"
                    },
                    {
                        "HostIp": "0.0.0.0",
                        "HostPort": "49201"
                    }
                ]
            },
            "SandboxKey": "/var/run/docker/netns/d3c68b7c52f0",
            "SecondaryIPAddresses": null,
            "SecondaryIPv6Addresses": null,
            "EndpointID": "",
            "Gateway": "",
            "GlobalIPv6Address": "",
            "GlobalIPv6PrefixLen": 0,
            "IPAddress": "",
            "IPPrefixLen": 0,
            "IPv6Gateway": "",
            "MacAddress": "",
            "Networks": {
                "TestNetwork": {
                    "IPAMConfig": null,
                    "Links": null,
                    "Aliases": [
                        "ui",
                        "9b44e54540a2"
                    ],
                    "NetworkID": "edeae335d736565b70746f4b86f221d6e1ea6e4e74021cce0ddfb6a3b93f28ad",
                    "EndpointID": "d24e664d3d1cc0ffc34e2a7467976851c63cbc4f66966894074fa84596b08d3d",
                    "Gateway": "172.20.0.1",
                    "IPAddress": "172.20.0.3",
                    "IPPrefixLen": 16,
                    "IPv6Gateway": "",
                    "GlobalIPv6Address": "",
                    "GlobalIPv6PrefixLen": 0,
                    "MacAddress": "02:42:ac:14:00:03",
                    "DriverOpts": null
                }
            }
        }
    }
]
```