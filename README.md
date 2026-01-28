prog2005-BIT250220-Tran Duy Long // BaiTapChuong1
```python


#Bai1
import math
from operator import truediv


def bai1():
    a = int(input('nhap so nguyen: '))
    b = float(input('nhap so thuc: '))
    c = str(input('nhap mot chuoi: '))
    print(a,b,c, end=' ')
#Bai2
def bai2():
    pi = 3.14
    r=5
    c = 2*pi*r
    print('chu vi hinh tron la:',c)
#Bai3
def bai3():
    a = float(input('nhap so a :'))
    b = float(input('nhap so b :'))
    c = a+b
    d = a - b
    e = a*b
    f = a/b
    print('tong, hieu, tich, thuong cua 2 so a va b lan luot la: ',c,d,e,f,end=' ')
#Bai4
def bai4():
    def sum_two_numbers(a,b):
        return a+b
    c = int(input('nhap so a :'))
    d = int(input('nhap so b :'))
    result = sum_two_numbers(c,d)
    print('Tong 2 so la:', result)
#Bai5
def bai5():
    name = 'Tran Duy Long'
    age = 18
    average_score = 9.5
    print('Name:', name, '| Kieu du lieu:', type(name))
    print('Age:', age, '| Kieu du lieu:', type(age))
    print('Average_score:', average_score, '| Kieu du lieu:', type(average_score))
    age_next_year = age + 1
    doubled_score = average_score * 2
    print('Age next year:', age_next_year, '| Kieu du lieu:', type(age_next_year))
    print('Doubled score:', doubled_score, '| Kieu du lieu:', type(doubled_score))
#Bai6
def bai6():
    def is_even(n):
        return n % 2 == 0
    n = int(input('nhap so a :'))
    print(is_even(n))
#Bai7
def bai7():
    a = float(input('nhap so a :'))
    b = float(input('nhap so b :'))
    c = float(input('nhap so b :'))
    if a >= b and a >= c:
        print('so lon nhat trong 3 so la:', a)
    elif b >= a and b >= c:
        print('so lon nhat trong 3 so la:', b)
    else:
        print('so lon nhat trong 3 so la:', c)
#Bai8
def bai8():
    def greet(name='Student'):
        print('Hello', name,'!')
    greet()
    greet(name='Long')
#Bai9
def bai9():
    a=int(input('nhap so tuoi cua ban :'))
    if a >= 1 and a <= 120:
        print('Do tuoi cua ban nam trong khoang tu 1 den 120')
    else:
        print('Do tuoi cua ban khong nam trong khoang tu 1 den 120')
#Bai10
def bai10():
    n = str(input("nhap day ki tu :"))
    x = str('a')
    dem = 0
    for i in n:
        if i == x:
            dem += 1
    print('so lan xuat hien', x, 'la:', dem)
#Bai11
def bai11():
    a=float(input('nhap do C :'))
    b= a*9/5+32
    print('Do F la :', b)
#Bai12
def bai12():
    a=float(input('nhap can nang (kg) :'))
    b=float(input('nhap chieu cao (m) :'))
    BMI = a/(b*b)
    print(f'BMI = {BMI:.2f}')
#Bai13
def bai13():
    try:
        a=int(input('nhap so a :'))
        b=int(input('nhap so b :'))
        c=a/b
        print('Ket qua la:' ,c)

    except ZeroDivisionError:
        print("Error: Khong the chia cho 0.")

    except ValueError:
        print("Error: Du lieu khong hop le.")
#Bai14
def bai14():
    a=float(input('nhap so a :'))
    if a <= 0 or a == 0 :
        print('Error')
    else:
        b= math.sqrt(a)
        print('Can bac hai cua ',a, 'la: ',b)
#Bai15
def bai15():
    n=3
    for i in range(1,n+1):
        print("TT SV: ")
        x = input(f"Ten SV{i}: ")
        Toan = float(input(f"Diem Toan cua sv{i}: "))
        Ly = float(input(f"Diem Ly cua sv{i}: "))
        Hoa = float(input(f"Diem Hoa cua sv{i}: "))
        print(x, "diem trung binh: ", (Toan+Ly+Hoa)/3)




while True:
    chon = input('chon bai:')
    if chon == '1':
        bai1()
        break
    if chon == '2':
        bai2()
        break
    if chon == '3':
        bai3()
        break
    if chon == '4':
        bai4()
        break
    if chon == '5':
        bai5()
        break
    if chon == '6':
        bai6()
        break
    if chon == '7':
        bai7()
        break
    if chon == '8':
        bai8()
        break
    if chon == '9':
        bai9()
        break
    if chon == '10':
        bai10()
        break
    if chon == '11':
        bai11()
        break
    if chon == '12':
        bai12()
        break
    if chon == '13':
        bai13()
        break
    if chon == '14':
        bai14()
        break
    if chon == '15':
        bai15()
        break
```

