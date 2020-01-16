# Read-content-of-file
Program that reads content of file if file exists
def read_content_of_file(path):
    try:
        with open(path, "r") as file:
            for line in file:
                print(line)
    except FileNotFoundError:
        print("Nie ma takiego pliku")

nameOfFile = input("What file do you want to open?")

fileContent = read_content_of_file(nameOfFile)
