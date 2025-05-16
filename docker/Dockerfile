FROM ros:humble-ros-base

ENV DEBIAN_FRONTEND=noninteractive

# 必要な開発ツールのインストール
RUN apt-get update && apt-get install -y \
    python3-pip \
    clang \
    clang-format \
    curl \
    lsb-release \
    sudo \
    git \
    cmake \
    && rm -rf /var/lib/apt/lists/*

# rosdep の初期化
RUN rosdep init && rosdep update


