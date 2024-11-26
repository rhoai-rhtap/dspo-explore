FROM docker.io/python:3.13

# Set working directory
WORKDIR /app

# Copy the script into the container
COPY package_upload.sh /app/package_upload.sh

# Make sure the script is executable
RUN chmod +x /app/package_upload.sh

# Store the files in a folder
VOLUME /app/packages

ENTRYPOINT ["/app/package_upload.sh"]
