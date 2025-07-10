

**System Architecture Diagram**
+------------------------+                   +----------------------+
|   Client Browser       |                   |   Firebase Services  |
|------------------------|                   |----------------------|
| HTML, CSS, Bootstrap   |<-- Firestore API->| Firestore Database   |
| Vanilla JS             |                   | /products            |
|                        |                   | /carts/{userId}/items|
| Firebase Auth          |<-- Auth API ----->| /orders              |
|                        |                   | /users               |
+------------------------+                   +----------------------+


**User Dashboard**
+-----------------------------------+
| Navbar: Home | Cart | Orders | Profile | Logout |
+-----------------------------------+

[Products Grid]
+--------------------+  +--------------------+
| Product Card       |  | Product Card       |
| Name, Image, Price |  | Name, Image, Price |
| [Add to Cart]      |  | [Add to Cart]      |
+--------------------+  +--------------------+

[Cart View]
[Order Summary]
[Place Order Button]


**Admin Panel**
+--------------------+
| Manage Products    |
| Manage Orders      |
| Logout             |
+--------------------+

[Manage Products Section]
[Product Cards with Edit/Delete]

[Add Product Form]

[Manage Orders Section]
[Order Cards with Status Update]
