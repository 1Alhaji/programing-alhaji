git clone [repository-url]
cd library-management-system
python --version
# Should display Python 3.8 or higher
python main.py
library-management-system/
│
├── main.py                 # Main application entry point
├── library.py             # Core Library class implementation
├── book.py               # Book class definition
├── member.py             # Member class definition
├── config.py             # System configuration and constants
├── utils.py              # Utility functions and helpers
├── Design Rationale.pdf  # Detailed design documentation
├── README.md             # This file
└── tests/                # Unit tests
    ├── test_library.py
    ├── test_book.py
    └── test_member.py
Select Option: 1 (Book Operations)
Select: 1 (Add Book)
Enter ISBN: 978-0134853987
Enter Title: Clean Code
Enter Author: Robert C. Martin
Select Genre: 1 (Programming)
Enter Total Copies: 5
Select Option: 3 (Borrowing Operations)
Select: 1 (Check Out Book)
Enter Member ID: M1001
Enter ISBN: 978-0134853987
Book successfully checked out!
from library import Library

# Create library instance
my_library = Library()

# System is ready to use
my_library.show_main_menu()
book_data = {
    "isbn": "978-0134853987",
    "title": "Clean Code",
    "author": "Robert C. Martin",
    "genre": "Programming",
    "total_copies": 5
}
my_library.add_book(book_data)
python -m pytest tests/
