# Image de base ROS2 Humble
FROM ros:humble

# Mise à jour et installation des dépendances Python
RUN apt-get update && apt-get install -y \
    python3-pip \
    python3-colcon-common-extensions \
    && rm -rf /var/lib/apt/lists/*

# Création du workspace ROS2
WORKDIR /ros2_ws

# Installation des dépendances ROS2 Python
RUN apt-get update && apt-get install -y \
    ros-humble-rclpy \
    && rm -rf /var/lib/apt/lists/*

# Configuration de l'environnement ROS2
RUN echo "source /opt/ros/humble/setup.bash" >> ~/.bashrc

# Point d'entrée par défaut
CMD ["/bin/bash"]
