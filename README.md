import math

a = float(input("nhập hệ số a: "))
b = float(input("nhập hệ số b: "))
c = float(input("nhập hệ số c: "))
if a == 0:
  print("phương trình trở thành phương trình bậc nhất(ax+b=0)hoặc không hợp lệ")
else:
  delta = b**2 - 4*a*c
  if delta > 0:
    x1 = (-b + math.sqrt(delta)) / (2*a)
    x2 = (-b - math.sqrt(delta)) / (2*a)
    print(f"phương trình có hai nghiệm phân biệt: x1 = {x1} và x2 = {x2}")
  elif delta == 0:
    x = -b / (2*a)
    print(f" phương trình có nghiệm kép: x = {x}")
  else:
    print("phương trình vô nghiệm")
