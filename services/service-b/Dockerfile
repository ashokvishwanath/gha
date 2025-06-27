FROM golang:1.19

# Set working directory
WORKDIR /app

# Copy source
COPY main.go .

# Build the Go binary
RUN go build -o service-b main.go

# Expose port and run
EXPOSE 5000
CMD ["./service-b"]
