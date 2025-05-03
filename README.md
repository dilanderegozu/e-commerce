# 🛍️ E-Commerce Backend

## 🇹🇷 Türkçe

Bu proje, bir e-ticaret platformunun **backend** tarafını Node.js ve Express.js kullanarak geliştirmeyi amaçlamaktadır. Kullanıcı yönetimi, ürün yönetimi, sipariş işlemleri ve kimlik doğrulama gibi temel işlevleri kapsar.

### 🚀 Özellikler

- Kullanıcı kayıt ve giriş işlemleri (JWT tabanlı)
- Ürün CRUD işlemleri
- Sipariş oluşturma ve yönetimi
- Rol bazlı erişim kontrolü (admin/kullanıcı)
- MongoDB veritabanı ile kalıcı veri saklama

### 🛠️ Teknolojiler

- **Node.js** – JavaScript çalışma zamanı
- **Express.js** – Web uygulama çatısı
- **MongoDB & Mongoose** – Veritabanı ve ODM
- **JWT (JSON Web Token)** – Kimlik doğrulama
- **dotenv** – Ortam değişkenleri yönetimi
- **bcrypt** – Şifreleme

### ⚙️ Kurulum

```bash
git clone https://github.com/dilanderegozu/e-commerce.git
cd e-commerce
npm install
cp .env.example .env
# .env dosyasına gerekli bilgileri girin: MONGO_URI, JWT_SECRET, PORT
npm run dev
```

### 📁 Proje Yapısı

```
e-commerce/
├── config/
├── controllers/
├── models/
├── routes/
├── middleware/
├── utils/
├── validations/
├── app.js
└── server.js
```

### ✅ API Uç Noktaları

| Yöntem | URL                  | Açıklama                 | Koruma |
|--------|----------------------|--------------------------|--------|
| POST   | `/api/auth/register`| Yeni kullanıcı kaydı     | ❌     |
| POST   | `/api/auth/login`   | Kullanıcı girişi         | ❌     |
| GET    | `/api/products`     | Ürünleri listele         | ❌     |
| POST   | `/api/products`     | Ürün oluştur             | ✅ Admin |
| GET    | `/api/orders`       | Siparişleri getir        | ✅     |

### 📄 Lisans

Bu proje MIT lisansı ile lisanslanmıştır.

### 📬 İletişim

GitHub üzerinden [@dilanderegozu](https://github.com/dilanderegozu) ile iletişime geçebilirsiniz.

---

## 🇬🇧 English

This project aims to build the **backend** of an e-commerce platform using Node.js and Express.js. It includes core functionalities such as user management, product operations, order handling, and authentication.

### 🚀 Features

- User registration and login (JWT-based)
- Product CRUD operations
- Order creation and management
- Role-based access control (admin/user)
- Persistent storage with MongoDB

### 🛠️ Technologies Used

- **Node.js** – JavaScript runtime
- **Express.js** – Web framework
- **MongoDB & Mongoose** – Database and ODM
- **JWT (JSON Web Token)** – Authentication
- **dotenv** – Environment variable management
- **bcrypt** – Password hashing

### ⚙️ Installation

```bash
git clone https://github.com/dilanderegozu/e-commerce.git
cd e-commerce
npm install
cp .env.example .env
# Fill in .env with: MONGO_URI, JWT_SECRET, PORT
npm run dev
```

### 📁 Project Structure

```
e-commerce/
├── config/
├── controllers/
├── models/
├── routes/
├── middleware/
├── utils/
├── validations/
├── app.js
└── server.js
```

### ✅ API Endpoints

| Method | URL                  | Description             | Protected |
|--------|----------------------|-------------------------|-----------|
| POST   | `/api/auth/register`| Register a new user     | ❌        |
| POST   | `/api/auth/login`   | User login              | ❌        |
| GET    | `/api/products`     | Get list of products    | ❌        |
| POST   | `/api/products`     | Create a product        | ✅ Admin  |
| GET    | `/api/orders`       | Get user orders         | ✅        |



### 📬 Contact

Feel free to reach out via GitHub: [@dilanderegozu](https://github.com/dilanderegozu)
