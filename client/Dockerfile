# Use a lightweight base image
FROM ruby:3.0.4-alpine

# Set the working directory inside the container
WORKDIR /app

# Install system dependencies
RUN apk add --no-cache build-base

# Copy the client code to the container
COPY client.rb .

# Install the necessary gem
RUN gem install httparty

# Run the client script
CMD ["ruby", "client.rb"]
