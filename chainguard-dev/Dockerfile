# Use the Chainguard .NET SDK image as the base image
FROM cgr.dev/chainguard/dotnet-sdk:latest-dev	

# Set the working directory
WORKDIR /app

# Copy your .NET application files into the container
COPY . .

# Specify the entry point
CMD ["dotnet", "HelloWorld.dll"]
