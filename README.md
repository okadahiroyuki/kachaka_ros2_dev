# Ubuntuデスクトップ＋ROS2にアクセスするためのHTML5 VNCインターフェースを提供するDockerfile
This Dockerfile is based on <br>
https://github.com/Tiryoh/docker-ros2-desktop-vnc<br>
https://github.com/AI-Robot-Book-Humble<br>
which is released under the Apache-2.0 license.







amd64
```
docker buildx build --platform=linux/amd64 --progress=plain -t tiryoh/ros2-desktop-vnc:jazzy-amd64 .
```
arm64
```
docker buildx build --platform=linux/arm64 --progress=plain -t okdhryk/ros2-desktop-vnc:jazzy-arm64 .
```

```
docker run -p 6080:80 --security-opt seccomp=unconfined --shm-size=512m okdhryk/ros2-desktop-vnc:jazzy-arm64
```
