# Use the universal image as the base
FROM mcr.microsoft.com/devcontainers/universal:2

# Install Java
RUN apt-get update && apt-get install -y openjdk-17-jdk

# Install Kotlin
RUN curl -s https://get.sdkman.io | bash && \
    source "$HOME/.sdkman/bin/sdkman-init.sh" && \
    sdk install kotlin

# Install Python
RUN apt-get install -y python3 python3-pip

# Clean up
RUN apt-get clean