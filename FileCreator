try:
    with open("file.txt",'r') as file:
        print("File already exists")
except FileNotFoundError:
    print("This file doesn't exist ")
    create = input("Type 1 if you want to create a file:")
    if create == '1':
        open("file.txt", 'w').close()
        print("File now exists :)")
    else:
        print("Invalid input")

while True:
    choice = input("Type 1 if you want to write/overwrite this file, 2 if you want to append it, 3 if you want to exit:")
    if choice =='1':
        try:
           text = input("Type some text:\n")
           with open("file.txt", 'w') as file:
               file.write(text)
        except Exception as e:
           print("Error writing to file")
    elif choice == '2':
        text = input("Type some text:\n")
        with open("file.txt", 'a') as file:
            file.write(text)
    elif choice == '3':
        break
    else:
        print("Invalid input")
