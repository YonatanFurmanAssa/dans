# Install OS + Framework
FROM node:18-alpine3.16

# Create directory inside the image: 
WORKDIR /app

# Copy only package.json to image /app:
COPY package.json /app

# Run command line "npm i" insde the image:
RUN npm i

# Copy all files into image /app:
COPY . /app

# Environment Variables: 
# ENV PORT=3001 CLOUD_SERVICE_PROVIDER=AWS CLOUD_SUPPORT_EMAIL=support@aws.com
ENV PORT=3001 \
    CLOUD_SERVICE_PROVIDER=AWS \
    CLOUD_SUPPORT_EMAIL=support@aws.com

# Run "npm start" when container starts: 
CMD ["npm", "start"]
