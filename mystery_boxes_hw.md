code1
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
email = "john.doe@gmail.com"
len_email = len(email)
first_name = ""
last_name = ""
found_alt_mark = False
found_dot = False
result = first_name,last_name
def divide_email (email):
    for index in range(len_email):
        print(index, email[index])

        if email[index] == ".":
            found_dot = True
        else:
            if found_dot == False:
                first_name += email[index]
            else:
                 if email[index] == "@":
                    found_alt_mark = True

                 else:
                     if found_alt_mark == False:
                        last_name += email[index]



    return result


print(result)


```
