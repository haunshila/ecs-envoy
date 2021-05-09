## Build the image
Now that we have a Dockerfile, let’s verify it builds correctly:

```docker build -t service:latest .```
After the build completes, we can run the container:

```docker run -d -p 8080:8080 service```