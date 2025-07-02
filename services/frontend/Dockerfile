FROM nginx:alpine

# Set working directory
WORKDIR /usr/share/nginx/html

# Remove default nginx static assets
RUN rm -rf ./*

# Copy static HTML
COPY index.html .
COPY build_timestamp.txt .

# Add version info for debugging
RUN echo "Build date: $(date)" > version.txt

EXPOSE 80

CMD ["nginx", "-g", "daemon off;"]
