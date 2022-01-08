print("....................CONTACT BOOK....................")
contact_book={}
while True:
    choice=input("What do you want do in contact book \n To save contact press 'N' \n To search contact press 'S' \n To view all contact 'A' \n To edit contact press 'E' \n To exit press 'X'\n").upper()
    if choice == "N":
        Name=input('Name of the person: ')
        Mobile_number=input('Mobile number: ')
        contact_book[Name]=Mobile_number
    elif choice == "S":
        search_name=input("Enter the name of the person: ")
        print("The number of the",search_name,"is",contact_book[search_name])
    elif choice == "A":
        print(contact_book)
    elif choice == "E":
        name=input('Enter the name of the contact,Which you want to edit: ')
        new_mobile_number=input('Enter the number: ')
        contact_book[name]=new_mobile_number
    elif choice == "X":
        break
