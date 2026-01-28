# BaiTapChuong1
```python
prog2005-BIT250220-Tran Duy Long // BaiTapChuong1
Chuong 1

import math
from math import factorial

#BT1
def bai1():
    n = int(input('Nhap so cua ban:'))
    if n > 0:
        print(n, 'la so duong')
    elif n<0:
        print(n, 'la so am')
    else:
        print(n, 'la so khong duong cung khong am')

#BT2
def bai2():
    for i in range(1, 11):
        print(i)

#BT3
def bai3():
    n = int(input("nhap so cua ban:"))
    tong = 0
    if n<0:
        print('vui long nhap lai')
    else:
        for i in range(0, n+1):
            tong=tong+i
    print(tong)
#BT4
def bai4():
    n = int(input("nhap so cua ban:"))
    if n <= 0:
        print('vui long nhap lai')
    else:
        if n%2==0:
            print(n,'la so chan')
        else:
            print(n, 'la so le')
#BT5
def bai5():
    for i in range(2, 21):
        if i%2:
            continue
        print(i)
#BT6
def bai6():
    n = int(input("nhap so cua ban:"))
    if n <= 0:
        print('vui long nhap lai')
    else:
        so_chu_so = len(str(n))
        print("SCS cua",n,'la',so_chu_so)
#BT7
def bai7():
    n = int(input("nhap so cua ban:"))
    if n <= 0:
        print('vui long nhap lai')
    else:
        ket_qua = factorial(n)
        print(ket_qua)
#BT8
def bai8():
    n = int(input("nhap so cua ban:"))
    if 1 < n < 9:
        for i in range(1, n+1):
            print('bang cuu chuong :')
            for x in range(1, 11):
                print(i,'*',x,'=',i*x)
    else:
        print('nhap lai')

#BT9
def bai9():
    for i in range(1, 101):
        if i%3:
            continue
        print(i)
#BT10
def bai10():
    i = 100
    while True:
        if i % 7 == 0:
            print("Số nguyên đầu tiên lớn hơn 100 và chia hết cho 7 là:", i)
            break
        i = i + 1
#BT11
def bai11():
    n = int(input("nhap so cua ban:"))
    if n <= 1:
        print(n,'khong la SNT')
        return
    SNT=True
    for i in range(2, int(math.sqrt(n)+1)):
            if n % i == 0:
                SNT = False
                break
    if SNT:
        print(n,'la SNT')

    else:
        print(n,' khong la SNT')
#BT12
def bai12():
    n = int(input("nhap so cua ban:"))
    a = 0
    b=1
    for i in range(n):
        print(a, end=' ')
        a, b = b, a + b #so tiep theo luon bang tong 2 so truoc
#BT13
def bai13():
    n = int(input("nhap so cua ban:"))
    tong = 0
    for i in str(n):
        tong += int(i)
    print('ket qua la', tong)
#BT14
def bai14():
    n = str(input("nhap day ki tu :"))
    x = str(input("nhap 1 ki tu:"))
    dem = 0
    for i in n:
        if i == x:
            dem += 1
    print('so lan xuat hien',x,'la:',dem)
#BT15
def giai_thua(n):
    if n == 0 or n == 1:
        return 1
    return n * giai_thua(n - 1)

def bai15():
    n = int(input("nhap so cua ban: "))
    if n < 0:
        print("nhap lai")
    else:
        print("giai thua", n, "la:", giai_thua(n))
#BT16
def bai16():
    a=int(input("nhap so thu nhat: "))
    b=int(input("nhap so thu hai: "))

    if a <= 0 or b <= 0 :
        print("nhap lai")
        return

    gcd = 1
    for i in range(1, min(a, b) + 1):
        if a % i == 0 and b % i == 0:
            gcd = i
    print('UCLN cua 2 so la',gcd)
#BT17
def bai17():
    for i in range(1, 1001):
        tong = 0
        for x in range(1, i):
            if i % x == 0:
                tong += x
        if tong == i:
            print('so hoan hao la', i)
#BT18
def bai18():
    a = input("nhap so cua ban: ")

    dao = ""
    for i in a:
        dao = i + dao    # ghép ký tự vào đầu chuỗi

    print("so dao nguoc la:", dao)
#BT19
def bai19():
    a = input("nhap so cua ban: ")
    so_lon_nhat = '0'
    for i in a:
        if i > so_lon_nhat:
            so_lon_nhat = i
    print("so_lon_nhat:", so_lon_nhat)
#BT20
def tong_so_nguyen(n):
    if n == 1:
        return 1
    return n + tong_so_nguyen(n-1)
def bai20():
    n=int(input("nhap so cua ban:"))
    if n <= 0:
        print('vui long nhap lai')
        return
    print('tong so nguyen la: ', tong_so_nguyen(n))



















while (True):
    chon = input('chon bai :')
    if chon == '1':
        bai1()
        break
    elif chon == '2':
        bai2()
        break
    elif chon == '3':
        bai3()
        break
    elif chon == '4':
        bai4()
        break
    elif chon == '5':
        bai5()
        break
    elif chon == '6':
        bai6()
        break
    elif chon == '7':
        bai7()
        break
    elif chon == '8':
        bai8()
        break
    elif chon == '9':
        bai9()
        break
    elif chon == '10':
        bai10()
        break
    elif chon == '11':
        bai11()
        break
    elif chon == '12':
        bai12()
        break
    elif chon == '13':
        bai13()
        break
    elif chon == '14':
        bai14()
        break
    elif chon == '15':
        bai15()
        break
    elif chon == '16':
        bai16()
        break
    elif chon == '17':
        bai17()
        break
    elif chon == '18':
        bai18()
        break
    elif chon == '19':
        bai19()
        break
    elif chon == '20':
        bai20()
        break
    else:
        print('chon lai')











