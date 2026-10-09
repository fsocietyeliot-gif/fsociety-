# fsociety script

Скрипт на Python по мотивам сериала «Mr. Robot».

```python
import os
import sys
import time

def fsociety():
    os.system("cls" if os.name == "nt" else "clear")
    print("\nHello, friend.")
    time.sleep(1.4)
    print("Hello, friend?")
    time.sleep(1.2)
    print("That's lame.")
    time.sleep(1.1)
    print("Maybe I should give you a name...")
    time.sleep(1.5)
    print("But how good is a name?")
    time.sleep(1.3)
    print("If it's a mask?")
    time.sleep(1.6)
    print("\nWelcome to fsociety.")
    time.sleep(1.2)
    print("We are finally free.")
    sys.exit(0)

def leave():
    os.system("cls" if os.name == "nt" else "clear")
    print("\nYou chose the system.")
    time.sleep(1.3)
    print("Control is an illusion.")
    time.sleep(1.4)
    print("But you already knew that...")
    time.sleep(1.5)
    print("\nGoodbye, friend.")
    sys.exit(0)

def main():
    os.system("cls" if os.name == "nt" else "clear")
    print("====================================")
    print("          f s o c i e t y           ")
    print("====================================")
    print("\n Are you ready to wake up?")
    print("1 - Join us")
    print("0 - Stay asleep")

    choice = input("\nWhat do you choose? ")
    if choice == "1":
        fsociety()
    elif choice == "0":
        leave()
    else:
        print("\n There is no middle ground.")
        time.sleep(1.4)
        main()

if __name__ == "__main__":
    main()
