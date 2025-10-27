import os

def create_file (filename):
    try:
        with open (filename , 'x') as f:
            print (f'file {filename} created successfully')
    except FileExistsError:
        print ('File alredy exist')

    except Exception as E:
        print ('Error observed on creating file')

def view_all_files ():
    
    files = os.listdir()
    if not files:
        print ("No file found")

    else:
        print ('Below file found')
        for file in files:
            print(file)


def delete_file(filename):
    try:
        os.remove(filename)
        print (f'{filename} removed successfully')
    except FileNotFoundError:
        print ("File not found so can't delete")

    except Exception as E:
        print ('Error in removing file')

def read_file (filename):
    try:
        with open (filename, 'r') as f:
            content = f.read()
            print (content)
    except FileNotFoundError:
        print ('File not found')

    except Exception as e:
        print ("Error in reading file")


def edit_file (file_name):
    try:
        with open (file_name ,'a') as f:
            content = input("write Here - ")
            f.write(content + '\n')
            print (f"File {file_name} has been edited sucessfully ")
    except FileNotFoundError:
        print ('File Not found')
    except Exception as e:
        print ("Error observed in editing the file")

def sam():
    print ("1 for create file")
    print ("2 for view all file")
    print ("3 for delete file")
    print ("4 for read file")
    print ("5 for edit file")
    print ("6 for close the app")

    
    while True:
        print ("This will be used for file management")
        print ("Please type 1,2,3,4,5,6 ")
        try:
        
            choice = int(input("Enter the value - "))

        except ValueError:
            print ("Please type a valid value")
            continue

        except Exception as E:
            print ("Please type 1-6 only Lets Try again")
            continue

        if choice == 1:
            filename = input ("Please type file name - ")
            create_file(filename)

        elif choice ==2:
            view_all_files()

        elif choice ==3:
            filename = input("Enter the name of file which you want to delete - ")
            delete_file(filename)

        elif choice == 4:
            filename = input("Enter the filename which you want to read - ")
            read_file(filename)
        elif choice == 5:
            filename = input ("Enter the file name which you want to edit - ")
            edit_file(filename)

        elif choice == 6:
            print ('App has been closed thank you for using')
            break
        else:
            print ("Please type 1-6 only")

if __name__ == "__main__":
    sam()

            



