import math

a = 15
b = 20

c = math.sqrt(a * a + b * b)

print(c)
a = float(input("a = "))
b = float(input("b = "))
c = float(input("c = "))

if (a + b > c) and (a + c > b) and (b + c > a):
    print("Gurvaljny tal bolno")
else:
    print("Gurvaljny tal bolohgui")
    a = int(input("a = "))
b = int(input("b = "))

s = 0

if a > b:
    t = a
    a = b
    b = t

for i in range(a, b + 1):
    s += i

print(s)
a = int(input("a = "))

p = 1

for i in range(1, a + 1, 2):
    p = p * i

print(p)

Даалгавар

p = int(input("Дүн оруул: "))

if 90 <= p <= 100:
    print("A")
elif 80 <= p <= 89:
    print("B")
elif 70 <= p <= 79:
    print("C")
elif 60 <= p <= 69:
    print("D")
elif 0 <= p <= 59:
    print("F")
else:
    print("Буруу дүн")

   b1 = float(input("b1 = "))
q = float(input("q = "))
n = int(input("n = "))

if q == 1:
    s = b1 * n
else:
    s = b1 * (q**n - 1) / (q - 1)

print("Нийлбэр =", s)

a1 = float(input("a1 = "))
d = float(input("d = "))
n = int(input("n = "))

s = n * (2 * a1 + (n - 1) * d) / 2

print("Нийлбэр =", s)

n = int(input("n = "))

if n < 2:
    print("Анхны тоо биш")
else:
    prime = True

    for i in range(2, int(n**0.5) + 1):
        if n % i == 0:
            prime = False
            break

    if prime:
        print("Анхны тоо")
    else:
        print("Анхны тоо биш")

        n = int(input("n = "))

for i in range(n, -1, -1):
    if str(i) == str(i)[::-1]:
        print("Палиндром =", i)
        break
        Өөрийгөө сориорой
        Sub t
q=0
While n<>0
 q=q+1
 n=n/10
 n=Math.Round(n)
EndWhile
EndSub
Sub t
q=0
While n<>0
 q=q*10+Math.Remainder(n,10)
 n=n/10
 n=Math.Floor(n)
EndWhile
EndSub
m=n
t()

If q=m Then
  TextWindow.Write("Tiim")
Else
  TextWindow.Write("Ugui")
EndIf

Sub Prime
  p = "True"

  If n < 2 Then
    p = "False"
  Else
    For i = 2 To Math.Floor(Math.SquareRoot(n))
      If Math.Remainder(n, i) = 0 Then
        p = "False"
      EndIf
    EndFor
  EndIf
EndSub
For n = 1 To 1000
  Prime()
  If p = "True" Then
    TextWindow.WriteLine(n)
  EndIf
EndFor
s = 0

For k = 1 To 100
  n = Math.GetRandomNumber(1000)

  Prime()

  If p = "True" Then
    s = s + n
  EndIf
EndFor

TextWindow.WriteLine(s)

Sub Palindrome
  m = n
  q = 0

  While n <> 0
    q = q * 10 + Math.Remainder(n,10)
    n = Math.Floor(n/10)
  EndWhile

  If m = q Then
    p = "True"
  Else
    p = "False"
  EndIf
EndSub
For n = 1 To 10000
  Palindrome()

  If p = "True" Then
    TextWindow.WriteLine(n)
  EndIf
EndFor
s = 0

For i = 1 To 1000
  n = Math.GetRandomNumber(10000)

  Palindrome()

  If p = "True" Then
    s = s + n
  EndIf
EndFor

TextWindow.WriteLine(s)
Sub Digit
  t = n

  For i = 1 To k-1
    t = Math.Floor(t/10)
  EndFor

  p = Math.Remainder(t,10)
EndSubDigit()

If p = t Then
  TextWindow.WriteLine("Tiim")
Else
  TextWindow.WriteLine("Ugui")
EndIfDigit()

TextWindow.WriteLine("k-r cifr = " + p)Digit()

If Math.Remainder(p,2)=0 Then
  TextWindow.WriteLine("Tegsh")
Else
  TextWindow.WriteLine("Sondgoi")
EndIfDigit()

If p = m Then
  TextWindow.WriteLine("Tiim")
Else
  TextWindow.WriteLine("Ugui")
EndIf
a[1] = 4
a[2] = 5
a[3] = 8
a[4] = 7
a[5] = 6
a[6] = 9
a[7] = 2
a[8] = 4
a[9] = 6
a[10] = 3

' а
q = a[1] + a[3] - a[5]
If (a[4] = a[2] + a[7]) Then
  TextWindow.Write("Doloo")
EndIf
TextWindow.WriteLine("")

' б
s = 0
For i = 1 To 10
  u = Math.Remainder(a[i], 2)
  If u = 1 Then
    s = s + a[i]
  EndIf
EndFor
TextWindow.WriteLine(s)

' г
For i = 1 To 10
  u = Math.Remainder(a[i], 3)
  If u = 0 Then
    TextWindow.Write(a[i] + " ")
  EndIf
EndFor
TextWindow.WriteLine("")

' д
For i = 1 To 10 Step 2
  TextWindow.Write(a[i] + " ")
EndFor
TextWindow.WriteLine("")

' е
p = 1
For i = 2 To 10 Step 2
  p = p * a[i]
EndFor
TextWindow.WriteLine(a[i])

' ё
m = a[1]
For i = 2 To 10
  If m > a[i] Then
    m = a[i]
  EndIf
EndFor
TextWindow.WriteLine(m)

' ж
For i = 1 To 10
  u = Math.Remainder(a[i], 2)
  If u = 1 Then
    TextWindow.Write(i + " ")
  EndIf
EndFor
TextWindow.WriteLine("")

' з
d = 0
For i = 1 To 10
  d = d + a[i]
EndFor
d = d / 10
TextWindow.WriteLine(d)

' и
For i = 1 To 10
  q = Math.SquareRoot(a[i])
  q = Math.Floor(q)
  If (q * q = a[i]) Then
    TextWindow.Write(a[i] + " ")
  EndIf
EndFor
TextWindow.WriteLine("")a[1] = 4
a[2] = 5
a[3] = 8
a[4] = 7
a[5] = 6
a[6] = 9
n = 6

For i = 1 To n - 1
  For j = 1 To n - i
    If a[j] > a[j+1] Then
      temp = a[j]
      a[j] = a[j+1]
      a[j+1] = temp
    EndIf
  EndFor
EndFor

For i = 1 To n
  TextWindow.Write(a[i] + " ")
EndFor
TextWindow.WriteLine("")
' Массив үүсгэх жишээ
a[1] = 12
a[2] = 5
a[3] = 23
a[4] = 8
a[5] = 17

max = a[1]
min = a[1]
max_idx = 1
min_idx = 1

For i = 2 To 5
  If a[i] > max Then
    max = a[i]
    max_idx = i
  EndIf
  If a[i] < min Then
    min = a[i]
    min_idx = i
  EndIf
EndFor

' 1.а. Утгыг хэвлэх
TextWindow.WriteLine("Max: " + max)
TextWindow.WriteLine("Min: " + min)

' 1.б. Дугаартай хамт хэвлэх
TextWindow.WriteLine("Max element: a[" + max_idx + "] = " + max)
TextWindow.WriteLine("Min element: a[" + min_idx + "] = " + min)' 3х4 хэмжээтэй массив үүсгэх жишээ
matrix[1][1] = 5
matrix[1][2] = 8
matrix[1][3] = 2
matrix[1][4] = 9

matrix[2][1] = 4
matrix[2][2] = 1
matrix[2][3] = 7
matrix[2][4] = 3

matrix[3][1] = 6
matrix[3][2] = 12
matrix[3][3] = 10
matrix[3][4] = 11

' а. Мөр бүрийн хамгийн их элементээр массив үүсгэх
For i = 1 To 3
  row_max = matrix[i][1]
  For j = 2 To 4
    If matrix[i][j] > row_max Then
      row_max = matrix[i][j]
    EndIf
  EndFor
  row_max_array[i] = row_max
EndFor

' б. Багана бүрийн хамгийн бага элементээр массив үүсгэх
For j = 1 To 4
  col_min = matrix[1][j]
  For i = 2 To 3
    If matrix[i][j] < col_min Then
      col_min = matrix[i][j]
    EndIf
  EndFor
  col_min_array[j] = col_min
EndFor

' в. Мөр бүрийн хамгийн их элементийн дугаарыг (баганыг) хэвлэх
For i = 1 To 3
  row_max = matrix[i][1]
  max_col_idx = 1
  For j = 2 To 4
    If matrix[i][j] > row_max Then
      row_max = matrix[i][j]
      max_col_idx = j
    EndIf
  EndFor
  TextWindow.WriteLine("Mor " + i + "-iin max elementiin bagana: " + max_col_idx)
EndFor

' г. Багана бүрийн хамгийн бага элементийн дугаарыг (мөрийг) хэвлэх
For j = 1 To 4
  col_min = matrix[1][j]
  min_row_idx = 1
  For i = 2 To 3
    If matrix[i][j] < col_min Then
      col_min = matrix[i][j]
      min_row_idx = i
    EndIf
  EndFor
  TextWindow.WriteLine("Bagana " + j + "-iin min elementiin mor: " + min_row_idx)
EndForFor i = 1 To 10
  For j = 1 To 10
    b[i][j] = i * j
    TextWindow.Write(b[i][j] + "	")
  EndFor
  TextWindow.WriteLine("")
EndForn = 3
m = 4
sum_a = 0
sum_b = 0
sum_v = 0

' 4.а. хэлбэр
TextWindow.WriteLine("Хэлбэр А:")
For i = 1 To n
  For j = 1 To m
    A[i][j] = i
    sum_a = sum_a + A[i][j]
    TextWindow.Write(A[i][j] + " ")
  EndFor
  TextWindow.WriteLine("")
EndFor

' 4.б. хэлбэр
TextWindow.WriteLine("Хэлбэр Б:")
For i = 1 To n
  For j = 1 To m
    B[i][j] = j
    sum_b = sum_b + B[i][j]
    TextWindow.Write(B[i][j] + " ")
  EndFor
  TextWindow.WriteLine("")
EndFor

' 4.в. хэлбэр
TextWindow.WriteLine("Хэлбэр В:")
count = 1
For i = 1 To n
  For j = 1 To m
    V[i][j] = count
    count = count + 1
    sum_v = sum_v + V[i][j]
    TextWindow.Write(V[i][j] + "	")
  EndFor
  TextWindow.WriteLine("")
EndFor

' 5. Нийлбэрүүдийг хэвлэх
TextWindow.WriteLine("A massiviin niilber: " + sum_a)
TextWindow.WriteLine("B massiviin niilber: " + sum_b)
TextWindow.WriteLine("V massiviin niilber: " + sum_v)n = 3
m = 4
sum_a = 0
sum_b = 0
sum_v = 0

' 4.а. хэлбэр
TextWindow.WriteLine("Хэлбэр А:")
For i = 1 To n
  For j = 1 To m
    A[i][j] = i
    sum_a = sum_a + A[i][j]
    TextWindow.Write(A[i][j] + " ")
  EndFor
  TextWindow.WriteLine("")
EndFor

' 4.б. хэлбэр
TextWindow.WriteLine("Хэлбэр Б:")
For i = 1 To n
  For j = 1 To m
    B[i][j] = j
    sum_b = sum_b + B[i][j]
    TextWindow.Write(B[i][j] + " ")
  EndFor
  TextWindow.WriteLine("")
EndFor

' 4.в. хэлбэр
TextWindow.WriteLine("Хэлбэр В:")
count = 1
For i = 1 To n
  For j = 1 To m
    V[i][j] = count
    count = count + 1
    sum_v = sum_v + V[i][j]
    TextWindow.Write(V[i][j] + "	")
  EndFor
  TextWindow.WriteLine("")
EndFor

' 5. Нийлбэрүүдийг хэвлэх
TextWindow.WriteLine("A massiviin niilber: " + sum_a)
TextWindow.WriteLine("B massiviin niilber: " + sum_b)
TextWindow.WriteLine("V massiviin niilber: " + sum_v)n = 3
m = 4
sum_a = 0
sum_b = 0
sum_v = 0

' 4.а. хэлбэр
TextWindow.WriteLine("Хэлбэр А:")
For i = 1 To n
  For j = 1 To m
    A[i][j] = i
    sum_a = sum_a + A[i][j]
    TextWindow.Write(A[i][j] + " ")
  EndFor
  TextWindow.WriteLine("")
EndFor

' 4.б. хэлбэр
TextWindow.WriteLine("Хэлбэр Б:")
For i = 1 To n
  For j = 1 To m
    B[i][j] = j
    sum_b = sum_b + B[i][j]
    TextWindow.Write(B[i][j] + " ")
  EndFor
  TextWindow.WriteLine("")
EndFor

' 4.в. хэлбэр
TextWindow.WriteLine("Хэлбэр В:")
count = 1
For i = 1 To n
  For j = 1 To m
    V[i][j] = count
    count = count + 1
    sum_v = sum_v + V[i][j]
    TextWindow.Write(V[i][j] + "	")
  EndFor
  TextWindow.WriteLine("")
EndFor

' 5. Нийлбэрүүдийг хэвлэх
TextWindow.WriteLine("A massiviin niilber: " + sum_a)
TextWindow.WriteLine("B massiviin niilber: " + sum_b)
TextWindow.WriteLine("V massiviin niilber: " + sum_v)n = 3
m = 4
sum_a = 0
sum_b = 0
sum_v = 0

' 4.а. хэлбэр
TextWindow.WriteLine("Хэлбэр А:")
For i = 1 To n
  For j = 1 To m
    A[i][j] = i
    sum_a = sum_a + A[i][j]
    TextWindow.Write(A[i][j] + " ")
  EndFor
  TextWindow.WriteLine("")
EndFor

' 4.б. хэлбэр
TextWindow.WriteLine("Хэлбэр Б:")
For i = 1 To n
  For j = 1 To m
    B[i][j] = j
    sum_b = sum_b + B[i][j]
    TextWindow.Write(B[i][j] + " ")
  EndFor
  TextWindow.WriteLine("")
EndFor

' 4.в. хэлбэр
TextWindow.WriteLine("Хэлбэр В:")
count = 1
For i = 1 To n
  For j = 1 To m
    V[i][j] = count
    count = count + 1
    sum_v = sum_v + V[i][j]
    TextWindow.Write(V[i][j] + "	")
  EndFor
  TextWindow.WriteLine("")
EndFor

' 5. Нийлбэрүүдийг хэвлэх
TextWindow.WriteLine("A massiviin niilber: " + sum_a)
TextWindow.WriteLine("B massiviin niilber: " + sum_b)
TextWindow.WriteLine("V massiviin niilber: " + sum_v)n = 3
a[1] = 4
a[2] = 5
a[3] = 8
a[4] = 7
a[5] = 6
a[6] = 9
n = 6

For i = 1 To n - 1
  For j = 1 To n - i
    If a[j] < a[j+1] Then
      temp = a[j]
      a[j] = a[j+1]
      a[j+1] = temp
    EndIf
  EndFor
EndFor

For i = 1 To n
  TextWindow.Write(a[i] + " ")
EndFor
TextWindow.WriteLine("")a[1] = 4
a[2] = 5
a[3] = 8
a[4] = 7
a[5] = 6
a[6] = 9
n = 6

For i = n To 2 Step -1
  max_idx = 1
  For j = 2 To i
    If a[j] > a[max_idx] Then
      max_idx = j
    EndIf
  EndFor
  
  temp = a[max_idx]
  a[max_idx] = a[i]
  a[i] = temp
EndFor

For i = 1 To n
  TextWindow.Write(a[i] + " ")
EndFor
TextWindow.WriteLine("")
