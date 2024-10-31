import java.util.Scanner;
import java.util.List;
import java.util.ArrayList;

//Create a Book class and declare its variables and methods
class Book {
    private String title;
    private String author;
    private String isbn;
    private boolean isAvailable;
    private User borrower;

    public Book(String title, String author, String isbn) {
        this.title = title;
        this.author = author;
        this.isbn = isbn;
        this.isAvailable = true;
    }

    public String getTitle() {
        return title;
    }

    public boolean isAvailable() {
        return isAvailable;
    }

    public void setAvailable(boolean available) {
        isAvailable = available;
    }

    public User getBorrower() {
        return borrower;
    }

    public void setBorrower(User borrower) {
        this.borrower = borrower;
    }

    @Override
    public String toString() {
        return String.format("%s by %s (ISBN: %s) - Available: %s", title, author, isbn, isAvailable);
    }
}

//Create a User class,declaring its variables and methods
class User {
    private String name;
    private List<Book> borrowedBooks;

    public User(String name) {
        this.name = name;
        this.borrowedBooks = new ArrayList<>();
    }

    public String getName() {
        return name;
    }

    public List<Book> getBorrowedBooks() {
        return borrowedBooks;
    }

    @Override
    public String toString() {
        return String.format("%s has borrowed these books: %s", name, borrowedBooks);
    }

    public void borrow(Book book) {
        borrowedBooks.add(book);
        book.setBorrower(this);
    }

    public void returnBook(Book book) {
        borrowedBooks.remove(book);
        book.setBorrower(null);
    }
}

//Create sub-classes inherited from Book class according to book category
class MysteryBook extends Book {
    public MysteryBook(String title, String author, String isbn) {
        super(title, author, isbn);
    }
}

class HorrorBook extends Book {
    public HorrorBook(String title, String author, String isbn) {
        super(title, author, isbn);
    }
}

class RomanceBook extends Book {
    public RomanceBook(String title, String author, String isbn) {
        super(title, author, isbn);
    }
}

//Create a main Library class and its main method
public class Library {
    private static Scanner scanner = new Scanner(System.in);

    public static void main(String[] args) {
        List<Book> availableBooks = new ArrayList<>();
        availableBooks.add(new MysteryBook("The Hound of the Baskervilles", "Sir Arthur Conan Doyle", "978-1503312753"));
        availableBooks.add(new HorrorBook("The Exorcist", "William Peter Blatty", "978-0061007224"));
        availableBooks.add(new RomanceBook("Pride and Prejudice", "Jane Austen", "978-0141439518"));

        List<User> users = new ArrayList<>();
        users.add(new User("Dilini"));
        users.add(new User("Rashmika"));
		users.add(new User("Abhi"));
		
        while (true) {
            System.out.println("\n------ LIBRARY MANAGEMENT SYSTEM ------");
            System.out.println("1. Borrow a book");			
            System.out.println("2. Return a book");
            System.out.println("3. Display user information");
            System.out.println("4. Display book information");
            System.out.println("5. Add a new book");
            System.out.println("0. Exit");
            System.out.print("Enter your choice: ");

            int choice;
            try {
                choice = Integer.parseInt(scanner.nextLine());
            } catch (NumberFormatException e) {
                System.out.println("Invalid input. Please enter a number.");		//Error handling
                continue;
            }

            switch (choice) {
                case 1:
                    borrowBook(scanner, availableBooks, users);
                    break;
                case 2:
                    returnBook(scanner, availableBooks, users);
                    break;
                case 3:
                    displayUserInformation(users);
                    break;
                case 4:
                    displayBookInformation(availableBooks);
                    break;
                case 5:
                    addNewBook(scanner, availableBooks);
                    break;
                case 0:
                    System.out.println("**__Exiting the Library__**");
                    scanner.close();
                    System.exit(0);
                    break;
                default:
                    System.out.println("Invalid choice. Please enter a valid option.");			//Error handling
            }
        }
    }
	
//Borrowing books using user name and book title
    private static void borrowBook(Scanner scanner, List<Book> availableBooks, List<User> users) {
        System.out.print("\nEnter user name: ");
        String userName = scanner.nextLine();

        System.out.print("Enter book title to borrow: ");
        String bookTitle = scanner.nextLine();

        User user = findUserByName(userName, users);
        Book book = findBookByTitle(bookTitle, availableBooks);

        if (user != null && book != null && book.isAvailable()) {
            user.borrow(book);
            book.setAvailable(false);
            System.out.println("----" + userName + " has successfully borrowed " + bookTitle + "----");		//Show the book was borrowed successfully
        } else {
            System.out.println("Invalid user, book, or book is not available for borrowing.");		//Error handling
        }
    }

//Returning books using user name and book title
    private static void returnBook(Scanner scanner, List<Book> availableBooks, List<User> users) {
        System.out.print("\nEnter user name: ");
        String userName = scanner.nextLine();

        System.out.print("Enter book title to return: ");
        String bookTitle = scanner.nextLine();

        User user = findUserByName(userName, users);
        Book book = findBookByTitle(bookTitle, user.getBorrowedBooks());

        if (user != null && book != null) {
            user.returnBook(book);
            book.setAvailable(true);
            System.out.println("----" + userName + " has successfully returned " + bookTitle + "----");		//Show the book was returned successfully
        } else {
            System.out.println("Invalid user / book, or the book was not borrowed by the user.");		//Error handling
        }
    }

//User information and book information
    private static User findUserByName(String name, List<User> users) {
        for (User user : users) {
            if (user.getName().equals(name)) {
                return user;
            }
        }
        return null;
    }

    private static Book findBookByTitle(String title, List<Book> books) {
        for (Book book : books) {
            if (book.getTitle().equals(title)) {
                return book;
            }
        }
        return null;
    }

//Displaying the information of users
    private static void displayUserInformation(List<User> users) {
        System.out.println("\n----- User Information -----");
        for (User user : users) {
            System.out.println(user);
        }
    }
//Displaying the list of available books
    private static void displayBookInformation(List<Book> books) {
        System.out.println("\n----- Book Information -----");
        for (Book book : books) {
            System.out.println(book);
        }
    }

//Adding a new book by entering book title,author,ISBN and book category
    private static void addNewBook(Scanner scanner, List<Book> availableBooks) {
        System.out.println("\n----- Add a New Book -----");
        System.out.print("Enter book title: ");
        String title = scanner.nextLine();

        System.out.print("Enter book author: ");
        String author = scanner.nextLine();

        System.out.print("Enter book ISBN: ");
        String isbn = scanner.nextLine();

        System.out.println("Select book category:");
        System.out.println("1. Mystery");
        System.out.println("2. Horror");
        System.out.println("3. Romance");
        System.out.print("Enter category choice: ");

        int categoryChoice;
        try {
            categoryChoice = Integer.parseInt(scanner.nextLine());
        } catch (NumberFormatException e) {
            System.out.println("Invalid input. Please enter a number.");		//Error handling
            return;
        }

        Book newBook;
        switch (categoryChoice) {
            case 1:
                newBook = new MysteryBook(title, author, isbn);
                break;
            case 2:
                newBook = new HorrorBook(title, author, isbn);
                break;
            case 3:
                newBook = new RomanceBook(title, author, isbn);
                break;
            default:
                System.out.println("Invalid category choice.");			//Error handling
                return;
        }

        availableBooks.add(newBook);
        System.out.println("New book added successfully: " + newBook);		//Show the book was added successfully
    }
}
