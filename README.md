# - num1
import random

def guess_number():
    num = random.randint(1, 100)
    attempts = 0

    print("1부터 100 사이의 숫자를 맞춰보세요")

    while True:
        
        me = int(input("숫자를 입력하세요: "))
        attempts += 1
        
        if me < num:
                print("더 커야 합니다")
        elif me > num:
                print("더 작아야합니다")
        else:
            print("정답! %d 번 만에 맞췄습니다." %attempts)
            break
        

guess_number()
