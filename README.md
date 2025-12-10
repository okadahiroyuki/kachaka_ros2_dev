# kachaka_ros2_dev


docker buildx build --platform=linux/arm64 --progress=plain -t okdhryk/ros2-desktop-vnc:jazzy-arm64 .

docker run -p 6080:80 --security-opt seccomp=unconfined --shm-size=512m okdhryk/ros2-desktop-vnc:jazzy-arm64
