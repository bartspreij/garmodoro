
# Use the existing ConnectIQ builder image as the base
FROM adamjakab/connectiq-builder-sdk-v7.2.1:latest

# Install any additional tools you might need
RUN apt-get update && \
    apt-get install -y vim curl git make openjdk-17-jdk &&\
    apt clean

# Set up working directories inside the container
WORKDIR /app

# Copy all local files to the container
COPY . /app

# Set an entry point to open a shell for interactive development
CMD ["/bin/bash"]
