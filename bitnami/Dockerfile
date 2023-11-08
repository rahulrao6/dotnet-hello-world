# Use the Bitnami .NET image as the base image
FROM bitnami/dotnet:latest

# Set the working directory
WORKDIR /app

# Copy your .NET application files into the container
COPY HelloWorld.dll .

# Specify the entry point
CMD ["dotnet", "HelloWorld.dll"]
