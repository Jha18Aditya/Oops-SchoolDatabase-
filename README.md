

School Alumni Management System
This project is a C++ application for managing school alumni, teachers, and students using Object-Oriented Programming (OOP) principles. It demonstrates key OOP concepts such as Abstraction, Encapsulation, Inheritance, and Polymorphism.

Features
Add Members: Add new alumni, teachers, and students to the database. Remove Members: Remove members from the database by name. Update Details: Update details of existing members, including graduation year, subject, and grade. Search Members: Search for members by name. Display Members: Display details of all members in the database. Display Member Count: Display the count of alumni, teachers, and students. Sort Members: Sort members by name. Dynamic Memory Management: Manage dynamic memory for member objects.
Code Explanation
Classes
SchoolMember (Abstract Base Class)
Attributes: name, age Methods:
displayDetails(): Pure virtual method to display member details. Getters and setters for name and age.
Alumni (Inherits from SchoolMember)
Attributes: graduationYear Methods:
displayDetails(): Overrides base class method to display alumni details. Getters and setters for graduationYear.
Teacher (Inherits from SchoolMember)
Attributes: subject Methods:
displayDetails(): Overrides base class method to display teacher details. Getters and setters for subject.
Student (Inherits from SchoolMember)
Attributes: grade Methods:
displayDetails(): Overrides base class method to display student details. Getters and setters for grade.
SchoolDatabase
Attributes: members (array of pointers to SchoolMember), count (number of members) Methods:
addMember(SchoolMember* member): Adds a new member to the database. removeMember(const string& name): Removes a member by name. updateMember(const string& name): Updates member details based on type. displayAllMembers(): Displays details of all members. searchMember(const string& name): Searches for a member by name. displayMemberCount(): Displays the count of alumni, teachers, and students. sortMembersByName(): Sorts members by name.
Main Function
The main() function provides a menu-driven interface for interacting with the SchoolDatabase:

Display All Members: Shows details of all members. Search Member by Name: Allows searching for a member by name. Update Member Details: Prompts for and updates details of a specified member. Remove Member: Removes a member by name. Display Member Count: Shows counts of different member types. Sort Members by Name: Sorts and displays members by name. Exit: Cleans up allocated memory and exits the program.
Compilation and Executions 
