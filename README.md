# Manajemen Toko Buku

Program sederhana untuk manajemen toko buku. Program ini menggunakan konsep Aggregation dengan dua kelas utama yaitu `Book` (Buku) dan `Bookstore` (Toko Buku). Setiap objek `Bookstore` akan memiliki beberapa objek `Book` yang merupakan daftar buku yang tersedia di toko tersebut.

## Deskripsi

Program ini terdiri dari dua kelas:

1. `Book` (Buku): Kelas ini merepresentasikan informasi tentang sebuah buku. Setiap objek `Book` memiliki atribut judul, penulis, dan harga.

2. `Bookstore` (Toko Buku): Kelas ini merepresentasikan toko buku. Setiap objek `Bookstore` memiliki atribut nama dan daftar objek `Book` yang tersedia di toko. Kelas ini juga memiliki metode untuk menambahkan buku baru ke dalam daftar dan menampilkan daftar buku yang tersedia di toko.

## Penggunaan

Berikut adalah contoh penggunaan program:

```python
# Membuat objek Bookstore
bookstore = Bookstore("Toko Buku ABC")

# Membuat beberapa objek Book dan menambahkannya ke Bookstore
book1 = Book("Harry Potter and the Philosopher's Stone", "J.K. Rowling", 150000)
book2 = Book("To Kill a Mockingbird", "Harper Lee", 120000)
book3 = Book("1984", "George Orwell", 90000)

bookstore.add_book(book1)
bookstore.add_book(book2)
bookstore.add_book(book3)

# Menampilkan daftar buku yang tersedia di toko
bookstore.display_books()
