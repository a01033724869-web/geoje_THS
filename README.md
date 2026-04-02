import random

def pick_numbers(start, end, count):
    # 범위 내에서 중복 없이 숫자 추출
    numbers = random.sample(range(start, end + 1), count)
    numbers.sort()  # 보기 좋게 정렬
    return numbers

# 예: 1부터 45까지의 숫자 중 6개 뽑기
result = pick_numbers(1, 45, 6)
print(f"추첨된 번호: {result}")
