# Use the official Ubuntu base image
FROM ubuntu:latest

# Install necessary dependencies and .NET SDK
RUN apt-get update \
    && apt-get install -y wget software-properties-common \
    && wget https://packages.microsoft.com/config/ubuntu/22.04/packages-microsoft-prod.deb -O packages-microsoft-prod.deb \
    && dpkg -i packages-microsoft-prod.deb \
    && apt-get update \
    && apt-get install -y apt-transport-https dotnet-sdk-7.0 \
    && rm -rf /var/lib/apt/lists/*

# Set the working directory
WORKDIR /app

# Copy your .NET application files into the container
COPY . .

# Build and run the application
RUN dotnet publish -c Release -o /app/out

# Define the entry point
ENTRYPOINT ["dotnet", "out/HelloWorld.dll"]
