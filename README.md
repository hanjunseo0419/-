# - num1
import random

def guess_number():
    number_to_guess = random.randint(1, 100)
    attempts = 0

    print("1부터 100 사이의 숫자를 맞춰보세요!")

    while True:
        
        user_guess = int(input("숫자를 입력하세요: "))
        attempts += 1
        
        if user_guess < number_to_guess:
                print("너무 작아요!")
        elif user_guess > number_to_guess:
                print("너무 커요!")
        else:
            print(f"정답입니다! {attempts}번 만에 맞췄어요!")
            break
        

guess_number()
