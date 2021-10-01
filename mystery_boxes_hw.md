```py
def my_title(name):
    print("The input is",name)
    if 97 <= ord(name[0]) and 122>= ord(name[0]):
        old_first_letter = ord(name[0]) -32
    else:
        old_first_letter = ord(name[0])
    new_letter = chr(old_first_letter)

    result=  new_letter + name[1: ]
    return result

def my_lowercase(name):
    print("The input is",name)
    if 65 <= ord(name[0]) and 90>= ord(name[0]):
        old_first_letter = ord(name[0]) +32
    else:
        old_first_letter = ord(name[0])
    new_letter = chr(old_first_letter)

    result = new_letter + name[1: ]
    return result


test = my_lowercase(my_title(name="Anju"))
print("ok",test)

test = my_lowercase(name="aup")
print("ok",test)

test = my_lowercase(name="Dr.Ruben")
print("ok",test)

def box1(word, option):
    if option == True:
        test = my_lowercase(word)
        print(test)
    else:
        test = (word)
        print(test)

box1("Hello", True)
box1("Hello", False)


#changed
```


MB2 incomplete
```py
def my_email(email):
    print("The input is",email)
    i = 0
    while email[i] != ".":
        first_name = email[i]
        print(first_name, end= "")
        i += 1

    while email[i] == ".":
        i += 1

    while email[i] != "@":
            last_name = email[i]
            print(last_name, end="")
            i += 1

    while email[i] == "@":
            i += 1
#some code that makes letters after @ show
#.title() the first name and last name but it is always updated and we can't really do that
test = my_email(email = "anju.yasu@uwcisak.jp")

email = "john.doe@gmail.com"
len_email = len(email)
name = ""
domain= ""
found_alt_mark = False
for index in range(len_email):
    print(index, email[index])
    if email[index] == "@":
        found_alt_mark = True
    else:
        if found_alt_mark == False:
            name += email[index]
        else:
            domain += email[index]

```
