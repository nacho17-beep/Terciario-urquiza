```mermaid
classDiagram
    class Book {
        +String title
        +String author
        +String isbn
        +boolean isAvailable()
    }

    class 
Miembro {
        +String name
        +String memberId
        +borrowBook(Book book)
        +returnBook(Book book)
    }

    class libreria {
        +String name
        +String employeeId
        +addBook(Book book)
        +removeBook(Book book)
    }

    class libreria {
        +String name
        +List books
        +List members
        +List librarians
        +addMember(Member member)
    }

    Library "1" -- "contains" libros
    Library "1" -- "registers" 
Miembro
    Library "1" -- "manages" libreria
