
# Golf Club Management System

This project is a Java-based application that manages information about members of a golf club. It includes features for storing member data, displaying it in a tabular format, and filtering records based on specific criteria such as join date, handicap score, and team/gender.

## Features

- **Member Registration**: Add multiple golf club members by providing their details.
- **Data Display**: View all member records in a tabular format.
- **Filters**:
  - Display members who joined before a specific date.
  - Display members with a handicap score less than a given value.
  - Display female members belonging to a specific team.

## Classes and Functionality

### `Date` Class
Handles date-related functionality:
- **Constructor**: Initializes a date with day, month, and year.
- **Methods**:
  - `dateDisplay()`: Formats and returns the date as a string.
  - `dateCompare()`: Compares two dates to check if one is earlier than the other.

### `golfClub` Class
Manages member data:
- **Attributes**:
  - Member ID, Name, Handicap, Gender, Team, Member Type, Coach, Phone Number, and Join Date.
- **Methods**:
  - `display()`: Outputs member details in a formatted table.
  - Main method for user input and processing.

## How to Run

1. **Compile**: Use the `javac` command to compile the program:
   ```bash
   javac Main.java
   ```
2. **Run**: Execute the program with:
   ```bash
   java GolfClubManagement.Main
   ```
3. **Input**: Follow the prompts to:
   - Enter the number of members.
   - Provide details for each member.

## Example Input and Output

### Input:
```
Enter number of members: 2
Enter details of member 1/2
Enter Member ID: 101
Enter First Name: John
Enter Last Name: Doe
Enter Handicap: 10
Enter Gender: M
Enter Team: TeamA
Enter Member Type: Regular
Enter Coach: 1
Enter Phone Number: 1234567890
Enter Join Date(DD/MM/YYYY): 15 January 2020
```

### Output:
```
+-----------+------------+------------+----------+--------+------------+--------------+--------+------------+------------------+
| Member ID | Last Name  | First Name | Handicap | Gender | Team       | Member Type  | Coach  | Phone      | Join Date        |
+-----------+------------+------------+----------+--------+------------+--------------+--------+------------+------------------+
| 101       | Doe        | John       | 10       | M      | TeamA      | Regular      | 1      | 1234567890 | 15-January-2020  |
+-----------+------------+------------+----------+--------+------------+--------------+--------+------------+------------------+

Records where member's Join Date is earlier than 7 April 2009:
No records found⛔

Records where member's Handicap score is less than 12:
Records found: 1

Records where member's are female and belong to team B:
No records found⛔
```

## Prerequisites

- Java Development Kit (JDK) 8 or above.

## Future Enhancements

- Add a GUI for easier interaction.
- Support data persistence using a database or file storage.

## License

This project is open-source and available under the [MIT License](LICENSE).
```

Let me know if you'd like further customization!
