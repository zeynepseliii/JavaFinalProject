# Temel imaj
FROM node:18

# Uygulama dizinine geç
WORKDIR /app

# Bağımlılıkları kopyala
COPY package*.json ./

# Bağımlılıkları yükle
RUN npm install

# Diğer tüm dosyaları kopyala
COPY . .

# Uygulamayı derle
RUN npm run build

# Production sunucusu olarak serve kullan
RUN npm install -g serve

# Portu belirt
EXPOSE 3000

# Başlatma komutu
CMD ["serve", "-s", "build"]