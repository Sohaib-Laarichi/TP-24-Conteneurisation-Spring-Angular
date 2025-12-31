# ==============================
# Stage 1: Build frontend
# ==============================
FROM node:18-alpine AS builder
WORKDIR /app

COPY package*.json ./
RUN npm install

COPY . .
RUN npm run build

# ==============================
# Stage 2: Nginx runtime
# ==============================
FROM nginx:alpine

COPY --from=builder /app/dist/smart-home /usr/share/nginx/html

EXPOSE 80
CMD ["nginx", "-g", "daemon off;"]