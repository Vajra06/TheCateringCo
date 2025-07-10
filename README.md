# 🥗 The Catering Co. - Reservation and Ordering System
How it works: https://thecateringco.netlify.app/

This project is a **web-based catering reservation and ordering system** that allows customers to:
- Browse available catering services and products
- Add items to a shopping cart
- Place orders and track their status
- Manage their profile

An **admin panel** enables administrators to:
- Manage products (add, edit, delete)
- Manage orders (approve, cancel, delete)

Built with:
- **HTML5, CSS3, Bootstrap 5**
- **Vanilla JavaScript (ES Modules)**
- **Firebase Auth + Firestore**

---

## 🚀 Features

### 👥 User Module
✅ User registration and login  
✅ View products and services  
✅ Search products by name  
✅ Add products to cart  
✅ Update quantities and remove items  
✅ Place orders  
✅ Track order status  
✅ View profile information  
✅ Logout securely  

---

### 🛠️ Admin Module
✅ Secure admin login  
✅ View all products  
✅ Add new products  
✅ Edit and delete products  
✅ View all orders  
✅ Update order statuses (Booked / Cancelled)  
✅ Delete orders  

---

## 📂 Project Structure

/project-root
├── index.html # Landing page
├── login.html # User/Admin login page
├── register.html # User registration page
├── dashboard.html # User dashboard
└── admin.html # Admin panel


---

## 🔧 Setup Instructions

### 1️⃣ Firebase Configuration
1. Create a Firebase project in the [Firebase Console](https://console.firebase.google.com/).
2. Enable **Email/Password Authentication** under **Authentication > Sign-in method**.
3. Create **Firestore Database** in **test mode**.
4. Create these Firestore collections:
   - `products`
   - `orders`
   - `users`
   - `carts/{userId}/items`
5. Update the `firebaseConfig` in your JavaScript with your project credentials.

Example:
```javascript
const firebaseConfig = {
  apiKey: "YOUR_API_KEY",
  authDomain: "YOUR_PROJECT_ID.firebaseapp.com",
  projectId: "YOUR_PROJECT_ID",
  storageBucket: "YOUR_PROJECT_ID.appspot.com",
  messagingSenderId: "SENDER_ID",
  appId: "APP_ID"
};

**Test Cases**

| #  | Test Description                   | Expected Result                  |
| -- | ---------------------------------- | -------------------------------- |
| 1  | Register a new user                | User account created             |
| 2  | Login as user                      | Dashboard loads                  |
| 3  | Search for a product               | Filtered products displayed      |
| 4  | Add product to cart                | Cart count increases             |
| 5  | Increase/decrease quantity in cart | Quantity updates in Firestore    |
| 6  | Remove product from cart           | Item removed                     |
| 7  | Place an order                     | Cart clears and order saved      |
| 8  | View order history                 | Orders with correct status shown |
| 9  | Login as admin                     | Admin panel loads                |
| 10 | Add a new product                  | Product visible to users         |
| 11 | Edit existing product              | Product updated                  |
| 12 | Delete a product                   | Product removed from Firestore   |
| 13 | Mark order as booked or cancelled  | User sees updated status         |
| 14 | Logout                             | Redirected to login page         |
| 15 | Unauthorized access to admin.html  | Redirected to login page         |


## License
This project is for educational purposes. Feel free to adapt and extend.

##Acknowledgements
Firebase

Bootstrap

FontAwesome
