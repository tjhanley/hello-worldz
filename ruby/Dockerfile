# Use the official Ruby image from the Docker Hub
FROM ruby:2.7

# Set the working directory inside the container
WORKDIR /usr/src/app

# Copy the Gemfile and Gemfile.lock into the working directory
COPY Gemfile Gemfile.lock ./

# Install dependencies
RUN bundle install

# Copy the rest of the application code
COPY . .

# Expose port 3000 to the host
EXPOSE 3000

# Set the default command to run the Sinatra application
CMD ["ruby", "app.rb"]
