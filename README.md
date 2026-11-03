print("===============================")
print("  WELCOME TO PYTHON TUTORIAL   ")
print("===============================")

print("Hello welcome to python tutorial system.")
print("how can i help you today")

print("what chapter do you want to study?")
print("[1] chapter 1 - Introduction to programming")
print("[2] chapter 2 - python basic syntax")
print("[3] chapter 3 - arithmetic operators and expressions")

chapter = input("enter chapter number:")

if chapter == "1":
    print("chapter 1: introduction to programming")
    print("[1] what is python programming?")
    print("[2] why learn python?")
    print("[3] what do you need to start python?")

    lesson = input("enter lesson number:")

    if lesson == "1":
        print("Lesson: what is python programming?")
        print("python is high-level interpreted and general purpose programming language it was created by Guido van rossum in 1991")

        print("example code:")
        print('print("hello, world")')

        print("output:")
        print("hello world!")

    elif lesson == "2":
        print("lesson: why learn python?")
        print("python is simple and easy to learn. it has readable syntax and is versatile. it also has a huge community.")

        print("output:")
        print('print("python is easy to learn!')

    elif lesson == "3":
        print("lesson: what do you need to start python?")
        print("You need Python and a code editor or IDE.Examples are PyCharm, VS Code,and Jupyter Notebook.")


