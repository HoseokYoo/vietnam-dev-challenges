# Description | Question 03

도서관 시스템을 설계하고, 주어진 책(Book) 데이터를 기반으로 특정 작가(author)의 책 목록과 총 페이지 수를 계산하여 출력하는 프로그램을 작성하세요.

Design a library system and write a program to calculate and print the list of books and the total number of pages for a specific author based on given book data.

Thiết kế một hệ thống thư viện và viết một chương trình để tính toán và in ra danh sách các cuốn sách cùng tổng số trang cho một tác giả cụ thể dựa trên dữ liệu sách đã cho.

```typescript
// Define the Book interface
interface Book {
  title: string;
  author: string;
  pages: number;
}

// Create a class Library to manage the books
class Library {
  private books: Book[];

  constructor(books: Book[]) {
    this.books = books;
  }

  // Method to get books by a specific author
  // Write your code here
  public getBooks(author: string){
    this.books.forEach(book => {
      if(author == book.author){
        console.log(book);
      }
    })
  }

  // Method to calculate the total number of pages for a specific author
  // Write your code here
  public getTotal_page(author: string){
    let total_pages=0;
    this.books.forEach(book => {
      if(author == book.author){
        total_pages+=book.pages;
      }
    })
    console.log("Total page of "+author+": ", total_pages);
  }
}

// Initialize the book data
const books: Book[] = [
  { title: "Book 1", author: "Author A", pages: 300 },
  { title: "Book 2", author: "Author B", pages: 200 },
  { title: "Book 3", author: "Author A", pages: 150 },
  { title: "Book 4", author: "Author C", pages: 400 },
  { title: "Book 5", author: "Author A", pages: 250 }
];

// Create an instance of the Library class and process the data
// Write your code here
console.log("Those are books of author A: ");
books.getBooks("Author A");
books.getTotal_page("Author A");
```
