FROM ruby:3.0.4

# Set working directory
WORKDIR /app

# Install dependencies
COPY Gemfile Gemfile.lock ./
RUN bundle install

# Copy application files
COPY server.rb .

# Expose the server port
EXPOSE 3333

# Set the entrypoint command
CMD ["ruby", "server.rb"]
