completed_lessons = 0
total_score = 0

while True:
    print("\n================================")
    print("          PYTHON TUTORIAL")
    print("        YOUR PYTHON JOURNEY")
    print("==================================")

    print("\n[1] Lesson 1: Introduction to Programming")

    if completed_lessons >= 1:
        print("[2] Lesson 2: Basic Syntax")
    else:
        print("[2] Lesson 2: LOCKED")

    if completed_lessons >= 2:
        print("[3] Lesson 3: Arithmetic Operations")
    else:
        print("[3] Lesson 3: LOCKED")

    print("[4] Exit")

    choice = input("\nEnter your choice: ")

    if choice == "1":

        if completed_lessons >= 1:
            print("\nYou already completed Lesson 1!")

        else:
            print("\n================================")
            print("LESSON 1: INTRODUCTION TO PROGRAMMING")
            print("================================")

            print("\n1. WHAT IS PROGRAMMING?")
            print("Programming is writing instructions")
            print("that tell a computer what to do.")
            print("A computer is very fast, but it cannot think for itself.")
            print("It only follows the exact steps you give it.")
            print("A set of these instructions is called a program.")

            print("\nExample: a recipe for toast")
            print("Step 1: Get the bread")
            print("Step 2: Put the bread in the toaster")
            print("Step 3: Wait")
            print("Step 4: Take out the toast")
            print("A program works the same way, one step after another.")

            input("\nPress ENTER to continue...")

            print("\n2. PROGRAMMING LANGUAGES")
            print("Computers only understand 1s and 0s (machine code).")
            print("A programming language lets humans write instructions")
            print("in a form that is easier to read and write.")
            print("Examples: Python, Java, C++, JavaScript")

            print("\nThe same idea in two languages:")
            print('Python:     print("Hello")')
            print('JavaScript: console.log("Hello")')
            print("Both display: Hello")

            input("\nPress ENTER to continue...")

            print("\n3. WHAT IS PYTHON?")
            print("Python is a beginner-friendly programming language.")
            print("It was created by Guido van Rossum.")
            print("Python was first released in 1991.")
            print("Its code looks close to English, so it is easy to read.")
            print("The name comes from the comedy show Monty Python,")
            print("not from the snake!")

            print("\nCompanies that use Python:")
            print("Google, Netflix, Instagram, and Spotify")

            input("\nPress ENTER to continue...")

            print("\n4. WHERE IS PYTHON USED?")
            print("1. Web Development - building websites and web servers")
            print("2. Artificial Intelligence - teaching computers to learn")
            print("3. Data Science - studying and charting large amounts of data")
            print("4. Automation - making the computer do boring tasks for you")
            print("5. Game Development - making simple games")
            print("6. Cybersecurity - testing and protecting systems")

            input("\nPress ENTER to continue...")

            print("\n5. HOW A PROGRAM WORKS")
            print("Most programs follow three steps:")
            print("INPUT   - the data given to the program")
            print("PROCESS - what the program does with the data")
            print("OUTPUT  - the result shown to the user")

            print("\nExample: a calculator")
            print("Input:   the user types 5 and 3")
            print("Process: the program adds 5 + 3")
            print("Output:  the screen shows 8")

            input("\nPress ENTER to continue...")

            print("\n6. ERRORS AND BUGS")
            print("A bug is a mistake that makes a program stop")
            print("or give the wrong result.")
            print("Finding and fixing bugs is called debugging.")
            print("Every programmer, even an expert, makes bugs.")

            print("\nCommon types of errors:")
            print("1. Syntax error  - you broke the rules of Python")
            print("2. Runtime error - the program crashes while running")
            print("3. Logic error   - the program runs but gives the wrong answer")

            print("\nTip: read the error message.")
            print("It tells you the line and the problem.")

            input("\nPress ENTER to continue...")

            print("\n7. YOUR FIRST PYTHON PROGRAM")
            print('print("Hello, World!")')
            print("Output: Hello, World!")
            print("\nCommon mistake: forgetting the quotation marks")
            print("around the text inside print().")

            name = input("\nEnter your name: ")
            print("Hello", name + "!")
            print("Welcome to Python programming!")

            input("\nPress ENTER to continue...")

            print("\n========== LESSON 1 QUIZ ==========")

            score = 0

            questions = [
                ["What is programming?",
                 "A. Playing games",
                 "B. Giving instructions to a computer",
                 "C. Watching videos",
                 "D. Browsing websites",
                 "B"],

                ["Who created Python?",
                 "A. Bill Gates",
                 "B. Steve Jobs",
                 "C. Guido van Rossum",
                 "D. Mark Zuckerberg",
                 "C"],

                ["When was Python first released?",
                 "A. 1985",
                 "B. 1991",
                 "C. 2000",
                 "D. 2010",
                 "B"],

                ["Which function displays output?",
                 "A. input()",
                 "B. type()",
                 "C. print()",
                 "D. int()",
                 "C"],

                ["Which is a use of Python?",
                 "A. Data analysis",
                 "B. Washing clothes",
                 "C. Cooking food",
                 "D. Driving cars",
                 "A"]
            ]

            for question in questions:
                while True:
                    print("\n" + question[0])
                    print(question[1])
                    print(question[2])
                    print(question[3])
                    print(question[4])

                    answer = input("Your answer: ").upper()

                    if answer == question[5]:
                        print("Correct! Excellent work!")
                        score = score + 1
                        total_score = total_score + 10
                        break

                    elif answer in ["A", "B", "C", "D"]:
                        print("Incorrect! Try again.")

                    else:
                        print("Please enter A, B, C, or D.")

            print("\nQUIZ COMPLETED!")
            print("Score:", score, "/ 5")
            print("Points Earned:", score * 10)

            completed_lessons = 1

            print("\nCONGRATULATIONS!")
            print("LESSON 1 COMPLETED!")
            print("LESSON 2 IS NOW UNLOCKED!")

    elif choice == "2":

        if completed_lessons < 1:
            print("\nACCESS DENIED!")
            print("Complete Lesson 1 first.")

        elif completed_lessons >= 2:
            print("\nYou already completed Lesson 2!")

        else:
            print("\n================================")
            print("LESSON 2: BASIC SYNTAX")
            print("================================")

            print("\nSyntax means the rules of writing code.")
            print("Just like English has grammar rules,")
            print("Python has syntax rules.")

            input("\nPress ENTER to continue...")

            print("\n1. PRINT FUNCTION")
            print("The print() function displays information.")
            print("Text must be inside quotation marks.")
            print("Numbers do not need quotation marks.")
            print("You can print several things by separating them with commas.")

            print('\nExample: print("Hello")')
            print("Output: Hello")
            print('Example: print("Age:", 18)')
            print("Output: Age: 18")

            print("\nCommon mistake: print(Hello) without quotes causes an error.")

            message = input("\nEnter your own message: ")
            print("Your message is:", message)

            input("\nPress ENTER to continue...")

            print("\n2. INPUT FUNCTION")
            print("The input() function allows users to enter data.")
            print("The program pauses and waits for the user to type")
            print("something and press ENTER.")
            print("The typed data is usually saved in a variable.")
            print("IMPORTANT: input() always gives you text (a string),")
            print("even if the user types a number.")

            print('\nExample: name = input("Enter your name: ")')

            student_name = input("Enter your name: ")
            print("Hello", student_name)

            input("\nPress ENTER to continue...")

            print("\n3. VARIABLES")
            print("Variables store information.")
            print("Think of a variable as a labeled box.")
            print("The label is the variable name.")
            print("The item inside the box is the value.")
            print("The = sign puts a value into the box.")
            print("It does not mean 'equals' like in math.")

            name = "Alex"
            age = 18

            print("\nname =", name)
            print("age =", age)

            print("\nA variable can change:")
            age = 19
            print("age is now", age)

            print("\nCommon mistake: using a variable before creating it")
            print("causes a NameError.")

            input("\nPress ENTER to continue...")

            print("\n4. DATA TYPES")
            print("A data type tells Python what kind of value it is.")

            print("\nSTRING (str)")
            print("Text inside quotes")
            print('name = "Maria"')

            print("\nINTEGER (int)")
            print("Whole numbers")
            print("age = 20")

            print("\nFLOAT (float)")
            print("Decimal numbers")
            print("price = 99.50")

            print("\nBOOLEAN (bool)")
            print("Only True or False")
            print("is_student = True")

            print("\nYou can check a type using type():")
            print('print(type("Maria"))  ->', type("Maria"))
            print("print(type(20))       ->", type(20))
            print("print(type(99.50))    ->", type(99.50))
            print("print(type(True))     ->", type(True))

            print('\nCommon mistake: "20" with quotes is a string, not a number!')

            input("\nPress ENTER to continue...")

            print("\n5. COMMENTS")
            print("Comments are notes inside a program.")
            print("Python ignores comments when running code.")
            print("Comments start with the # symbol.")
            print('Example: # This is a comment')
            print('Example: print("Hi")  # this also works')
            print("Programmers use comments to explain their code")
            print("so others (and themselves) can understand it later.")

            print("\n6. VARIABLE NAMING RULES")
            print("1. Must start with a letter or underscore (_)")
            print("2. Can contain letters, numbers, and underscores")
            print("3. No spaces and no symbols like - or $")
            print("4. Names are case-sensitive: Age and age are different")
            print("5. Use meaningful names: student_name is better than x")

            print("\nValid: student_name")
            print("Valid: age1")
            print("Valid: _score")
            print("Invalid: 2student")
            print("Invalid: student name")
            print("Invalid: my-age")

            input("\nPress ENTER to continue...")

            print("\n7. TYPE CONVERSION")
            print("Type conversion changes a value to another data type.")
            print("Since input() always gives text, you must convert it")
            print("before doing math.")
            print("int() converts to an integer.")
            print("float() converts to a decimal.")
            print("str() converts to a string.")

            print('\nExample: "5" + "3" gives "53" (text joined together)')
            print('Example: int("5") + int("3") gives 8')

            print("\nCommon mistake: typing words like 'abc' into int()")
            print("causes a ValueError.")

            age = int(input("\nEnter your age: "))
            print("Your age next year is:", age + 1)

            input("\nPress ENTER to continue...")

            print("\n8. INDENTATION")
            print("Indentation is the space at the start of a line.")
            print("Many languages use { } to group code.")
            print("Python uses indentation instead.")
            print("The standard is 4 spaces.")

            print("\nExample:")
            print("age = 18")
            print("if age >= 18:")
            print('    print("Adult")')
            print("Output: Adult")

            print("\nCommon mistake: forgetting to indent causes an")
            print("IndentationError.")

            input("\nPress ENTER to continue...")

            print("\n========== LESSON 2 QUIZ ==========")

            score = 0

            questions = [
                ["What is syntax?",
                 "A. Rules of writing code",
                 "B. Computer hardware",
                 "C. Internet connection",
                 "D. Computer games",
                 "A"],

                ["Which function receives user input?",
                 "A. print()",
                 "B. input()",
                 "C. type()",
                 "D. len()",
                 "B"],

                ["Which data type stores decimal numbers?",
                 "A. String",
                 "B. Integer",
                 "C. Float",
                 "D. Boolean",
                 "C"],

                ["Which symbol is used for comments?",
                 "A. @",
                 "B. &",
                 "C. #",
                 "D. $",
                 "C"],

                ["Which is a valid variable name?",
                 "A. 2name",
                 "B. student name",
                 "C. student_name",
                 "D. student-name",
                 "C"]
            ]

            for question in questions:
                while True:
                    print("\n" + question[0])
                    print(question[1])
                    print(question[2])
                    print(question[3])
                    print(question[4])

                    answer = input("Your answer: ").upper()

                    if answer == question[5]:
                        print("Correct! Excellent work!")
                        score = score + 1
                        total_score = total_score + 10
                        break

                    elif answer in ["A", "B", "C", "D"]:
                        print("Incorrect! Try again.")

                    else:
                        print("Please enter A, B, C, or D.")

            print("\nQUIZ COMPLETED!")
            print("Score:", score, "/ 5")
            print("Points Earned:", score * 10)

            completed_lessons = 2

            print("\nCONGRATULATIONS!")
            print("LESSON 2 COMPLETED!")
            print("LESSON 3 IS NOW UNLOCKED!")

    elif choice == "3":

        if completed_lessons < 2:
            print("\nACCESS DENIED!")
            print("Complete Lesson 2 first.")

        elif completed_lessons >= 3:
            print("\nYou already completed Lesson 3!")

        else:
            print("\n================================")
            print("LESSON 3: ARITHMETIC OPERATIONS")
            print("================================")

            print("\nArithmetic operations are used")
            print("to perform mathematical calculations.")

            input("\nPress ENTER to continue...")

            print("\n1. ADDITION (+)")
            print("Adds numbers together.")
            print("print(10 + 5)")
            print("Output: 15")
            print("The + sign can also join text together:")
            print('print("Py" + "thon")')
            print("Output: Python")
            print('Common mistake: "Age: " + 18 causes a TypeError.')
            print('Use "Age: " + str(18) or print("Age:", 18).')

            print("\n2. SUBTRACTION (-)")
            print("Takes one number away from another.")
            print("print(10 - 5)")
            print("Output: 5")

            input("\nPress ENTER to continue...")

            print("\n3. MULTIPLICATION (*)")
            print("Multiplies numbers. Use * and not x.")
            print("print(10 * 5)")
            print("Output: 50")
            print("Example use: total cost = price * quantity")

            print("\n4. DIVISION (/)")
            print("Divides numbers.")
            print("Division always gives a decimal (float) result.")
            print("print(10 / 4)")
            print("Output: 2.5")
            print("print(20 / 4)")
            print("Output: 5.0")
            print("Common mistake: dividing by zero causes a")
            print("ZeroDivisionError.")

            input("\nPress ENTER to continue...")

            print("\n5. FLOOR DIVISION (//)")
            print("Divides and then drops the decimal part.")
            print("It tells you how many times a number fits completely.")
            print("print(10 // 3)")
            print("Output: 3")
            print("Example: 17 candies shared by 5 kids.")
            print("print(17 // 5)")
            print("Output: 3 (each kid gets 3 candies)")

            print("\n6. MODULUS (%)")
            print("Gives the REMAINDER after division.")
            print("print(10 % 3)")
            print("Output: 1")
            print("3 fits into 10 three times (9), and 1 is left over.")
            print("In Python, % means remainder, not percent.")

            input("\nPress ENTER to continue...")

            print("\nTry it! EVEN OR ODD CHECKER")
            print("If a number % 2 is 0, the number is even.")

            number = int(input("Enter a whole number: "))

            if number % 2 == 0:
                print(number, "is EVEN because", number, "% 2 is 0")
            else:
                print(number, "is ODD because", number, "% 2 is 1")

            input("\nPress ENTER to continue...")

            print("\n7. EXPONENTIATION (**)")
            print("Raises a number to a power.")
            print("print(2 ** 3)")
            print("Output: 8")
            print("2 ** 3 means 2 x 2 x 2.")
            print("print(5 ** 2)")
            print("Output: 25")
            print("Common mistake: using ^ for powers.")
            print("In Python, ^ does something different.")

            input("\nPress ENTER to continue...")

            print("\n8. ORDER OF OPERATIONS")
            print("Python solves math in this order:")
            print("1. Parentheses ( )")
            print("2. Exponents **")
            print("3. Multiplication, Division, Floor Division, Modulus")
            print("   (left to right)")
            print("4. Addition and Subtraction (left to right)")

            print("\nprint(2 + 3 * 4)")
            print("Output: 14   (multiplication goes first)")
            print("print((2 + 3) * 4)")
            print("Output: 20   (parentheses go first)")

            input("\nPress ENTER to continue...")

            print("\n9. ASSIGNMENT OPERATORS")
            print("A shorter way to update a variable.")
            print("score += 10 is the same as score = score + 10")
            print("Others: -=, *=, /=, //=, %=, **=")

            print("\nscore = 0")
            print("score += 10")
            print("score += 10")
            print("score -= 5")
            print("print(score)")
            print("Output: 15")

            print("\n10. HELPFUL NUMBER FUNCTIONS")
            print("round(3.14159, 2) -> 3.14  (rounds a number)")
            print("abs(-7)           -> 7     (makes a number positive)")
            print("max(4, 9, 2)      -> 9     (largest number)")
            print("min(4, 9, 2)      -> 2     (smallest number)")

            input("\nPress ENTER to continue...")

            print("\n========== PYTHON CALCULATOR ==========")

            num1 = float(input("Enter first number: "))
            num2 = float(input("Enter second number: "))

            print("\n[1] Addition")
            print("[2] Subtraction")
            print("[3] Multiplication")
            print("[4] Division")
            print("[5] Floor Division")
            print("[6] Modulus")
            print("[7] Exponentiation")

            operation = input("\nChoose an operation: ")

            if operation == "1":
                print("Result:", num1 + num2)

            elif operation == "2":
                print("Result:", num1 - num2)

            elif operation == "3":
                print("Result:", num1 * num2)

            elif operation == "4":
                if num2 != 0:
                    print("Result:", num1 / num2)
                else:
                    print("Cannot divide by zero!")

            elif operation == "5":
                if num2 != 0:
                    print("Result:", num1 // num2)
                else:
                    print("Cannot divide by zero!")

            elif operation == "6":
                if num2 != 0:
                    print("Result:", num1 % num2)
                else:
                    print("Cannot divide by zero!")

            elif operation == "7":
                print("Result:", num1 ** num2)

            else:
                print("Invalid operation!")

            input("\nPress ENTER to continue...")

            print("\n========== LESSON 3 QUIZ ==========")

            score = 0

            questions = [
                ["What is 15 + 10?",
                 "A. 20",
                 "B. 25",
                 "C. 30",
                 "D. 35",
                 "B"],

                ["What is 20 - 7?",
                 "A. 13",
                 "B. 17",
                 "C. 15",
                 "D. 12",
                 "A"],

                ["What is 6 * 5?",
                 "A. 11",
                 "B. 25",
                 "C. 30",
                 "D. 35",
                 "C"],

                ["What is 20 / 4?",
                 "A. 4",
                 "B. 5",
                 "C. 6",
                 "D. 8",
                 "B"],

                ["What is 10 % 3?",
                 "A. 0",
                 "B. 1",
                 "C. 2",
                 "D. 3",
                 "B"]
            ]

            for question in questions:
                while True:
                    print("\n" + question[0])
                    print(question[1])
                    print(question[2])
                    print(question[3])
                    print(question[4])

                    answer = input("Your answer: ").upper()

                    if answer == question[5]:
                        print("Correct! Excellent work!")
                        score = score + 1
                        total_score = total_score + 10
                        break

                    elif answer in ["A", "B", "C", "D"]:
                        print("Incorrect! Try again.")

                    else:
                        print("Please enter A, B, C, or D.")

            print("\nQUIZ COMPLETED!")
            print("Score:", score, "/ 5")
            print("Points Earned:", score * 10)

            completed_lessons = 3

            print("\n================================")
            print("CONGRATULATIONS, PYTHON LEARNER!")
            print("YOU COMPLETED ALL THREE LESSONS!")
            print("================================")

    elif choice == "4":
        print("Keep learning and keep coding!")
        break

    else:
        print("\nInvalid choice! Please enter 1 to 4.")
