# Paper 2102 — Last-Minute Review Sheet

ဒီဖိုင်ကို စာမေးပွဲမဝင်မီ တစ်ဖိုင်တည်းဖွင့်ပြီး မြန်မြန်ပြန်ကြည့်ရန် အသုံးပြုပါ။
မေးခွန်းကို အရင်ဆုံး **ဘယ်နည်းလမ်းအုပ်စုလဲ** ခွဲပြီးမှ အဆင့်များအတိုင်းတွက်ပါ။

---

## 1. Symbol များ၏ အဓိပ္ပါယ်

- y′ = dy/dx — first derivative
- y″ = d²y/dx² — second derivative
- y‴ = d³y/dx³ — third derivative
- C_1, C_2, C_3 — arbitrary constants
- c_0, c_1, c_2, … — power-series coefficients
- Σ — summation (ပေါင်းစုပြခြင်း)
- y_c — complementary/homogeneous solution
- y_p — particular solution
- W — Wronskian
- R — radius of convergence

Power-series notation ကို အောက်ပါအတိုင်း တစ်ပုံစံတည်းသုံးပါ။

~~~text
y = sum_{n=0}^{infinity} c_n x^n
y′ = sum_{n=0}^{infinity} (n+1)c_{n+1}x^n
y″ = sum_{n=0}^{infinity} (n+2)(n+1)c_{n+2}x^n
~~~

---

## 2. မေးခွန်းကိုမြင်တာနဲ့ နည်းလမ်းခွဲခြားရန်

| မေးခွန်းတွင် တွေ့ရသော clue | သုံးရမည့်နည်းလမ်း |
|---|---|
| ay″ + by′ + cy = 0 | Characteristic equation |
| RHS တွင် x, eˣ, sin x, cos x ပါ | y = y_c + y_p |
| “appropriate form for a particular solution” | y_p form ကိုသာရေး |
| “variation of parameters” | W, u_1′, u_2′ formula |
| “power-series method” | y = sum c_n x^n ဟုစပြီး coefficient များညှိ |
| y(0), y′(0), y″(0) ပေးထား | General solution ထဲ substitute လုပ် |
| y_1, y_2, y_3 are linearly independent | y = C_1y_1 + C_2y_2 + C_3y_3 |

---

## 3. Characteristic-equation method

~~~text
ay″ + by′ + cy = 0
y = eʳˣ ဟုယူ
ar² + br + c = 0       ← characteristic equation
~~~

Root အမျိုးအစားအလိုက်—

~~~text
Distinct real roots r_1, r_2:
y = C_1eʳ¹ˣ + C_2eʳ²ˣ

Repeated root r:
y = (C_1 + C_2x)eʳˣ

Complex roots r = α ± βi:
y = eᵅˣ(C_1 cos βx + C_2 sin βx)
~~~

Initial conditions ထည့်ရန်—

1. General solution ရေးပါ။
2. လိုအပ်သော y′, y″ ကို differentiate လုပ်ပါ။
3. x = 0 ထည့်ပြီး equations ဖွဲ့ပါ။
4. C_1, C_2, C_3 ကိုဖြေပြီး solution ထဲပြန်ထည့်ပါ။

---

## 4. Unit I No. 4 — Given three independent solutions

မေးခွန်းပုံစံ — y_1 = eˣ, y_2 = e²ˣ, y_3 = e³ˣ နှင့် initial conditions ပေးထားသည်။

~~~text
1. y = C_1eˣ + C_2e²ˣ + C_3e³ˣ
2. y′ = C_1eˣ + 2C_2e²ˣ + 3C_3e³ˣ
3. y″ = C_1eˣ + 4C_2e²ˣ + 9C_3e³ˣ
4. x = 0 ထည့်ပြီး equations သုံးခုဖွဲ့
5. C_1, C_2, C_3 ဖြေ
~~~

Final answer —

~~~text
y = (3/2)eˣ − 3e²ˣ + (3/2)e³ˣ
~~~

---

## 5. Assignment 1 No. 1 — Verify + repeated root

### (i) Solution verify လုပ်ခြင်း

y_1 = eˣ cos x, y_2 = eˣ sin x ကို တစ်ခုချင်းစီအတွက်—

~~~text
1. y′ ရှာ
2. y″ ရှာ
3. y″ − 2y′ + 2y ထဲ substitute လုပ်
4. ရလဒ် 0 ဖြစ်ကြောင်းရေး
~~~

### (ii) Repeated root

~~~text
9y″ − 12y′ + 4y = 0
9r² − 12r + 4 = 0
(3r − 2)² = 0
r = 2/3  (repeated root)
~~~

Final answer —

~~~text
y = (C_1 + C_2x)e²ˣ⁄³
~~~

**သတိ:** repeated root ဖြစ်လျှင် ဒုတိယ term တွင် x မဖြစ်မနေပါရမည်။

---

## 6. Assignment 1 No. 4 — Third-order IVP

~~~text
y‴ + 3y″ − 10y′ = 0

r³ + 3r² − 10r = 0
r(r + 5)(r − 2) = 0
r = 0, −5, 2
~~~

ထို့ကြောင့်—

~~~text
y = C_1 + C_2e⁻⁵ˣ + C_3e²ˣ
~~~

Initial conditions ထည့်ပြီး—

~~~text
C_1 + C_2 + C_3 = 7
−5C_2 + 2C_3 = 0
25C_2 + 4C_3 = 70
~~~

C_1 = 0, C_2 = 2, C_3 = 5။

~~~text
Final answer: y = 2e⁻⁵ˣ + 5e²ˣ
~~~

---

## 7. Unit I No. 8 — Non-homogeneous IVP

~~~text
y″ − 2y′ + 2y = x + 1
~~~

### အဆင့်များ

~~~text
1. r² − 2r + 2 = 0
   r = 1 ± i
   y_c = eˣ(C_1 cos x + C_2 sin x)

2. RHS = x + 1 ဖြစ်သောကြောင့်
   y_p = Ax + B ဟုယူ

3. y_p′ = A, y_p″ = 0 ကို equation ထဲထည့်
   A = 1/2, B = 1

4. y = y_c + y_p
5. y(0) = 3, y′(0) = 0 ထည့်
~~~

Final answer —

~~~text
y = eˣ(2 cos x − (5/2) sin x) + (1/2)x + 1
~~~

---

## 8. Unit I No. 6 — Appropriate particular-solution form

~~~text
y″ + 6y′ + 13y = e⁻³ˣ cos 2x
~~~

~~~text
1. r² + 6r + 13 = 0
   r = −3 ± 2i

2. y_c = e⁻³ˣ(C_1 cos 2x + C_2 sin 2x)

3. RHS ပုံစံအရ မူလခန့်မှန်းချက်:
   e⁻³ˣ(A cos 2x + B sin 2x)

4. အဲဒီပုံစံသည် y_c နှင့် ထပ်နေသည်။
   ထို့ကြောင့် x တစ်ခါမြှောက်ရမည်။
~~~

Required form —

~~~text
y_p = xe⁻³ˣ(A cos 2x + B sin 2x)
~~~

**သတိ:** “appropriate form” ဟုသာမေးလျှင် A, B ကို မရှာရသေးပါ။

---

## 9. Unit I No. 9 — Variation of parameters

~~~text
y″ + 3y′ + 2y = 4eˣ
~~~

~~~text
1. r² + 3r + 2 = 0
   r = −1, −2

2. y_1 = e⁻ˣ,  y_2 = e⁻²ˣ

3. W = y_1y_2′ − y_1′y_2 = −e⁻³ˣ

4. g(x) = 4eˣ

5. u_1′ = −y_2g/W
   u_2′ =  y_1g/W

6. Integrate:
   u_1 = 2e²ˣ
   u_2 = −(4/3)e³ˣ

7. y_p = u_1y_1 + u_2y_2
~~~

Final particular solution —

~~~text
y_p = (2/3)eˣ
~~~

**သတိ:** W = y_1y_2′ − y_1′y_2 ၏ အစီအစဉ်မပြောင်းပါနှင့်။

---

## 10. Power-series method — အမြဲသုံးရမည့် အဆင့်များ

### Standard setup

~~~text
1. y = sum_{n=0}^{infinity} c_n x^n ဟုယူ
2. y′ နှင့် y″ ကိုရေး
3. equation ထဲ substitute လုပ်
4. xⁿ တူညီသော terms များကို စု
5. coefficient တစ်ခုချင်းစီ 0 နှင့်ညီစေ
6. recurrence relation ရှာ
7. c_0, c_1 ကို initial conditions မှရှာ
8. series ကိုရေးပြီး လိုအပ်လျှင် closed form ပြောင်း
9. Ratio test / known series ဖြင့် R ရှာ
~~~

Initial conditions ပြောင်းနည်း—

~~~text
c_0 = y(0)
c_1 = y′(0)
~~~

---

## 11. Unit II No. 5 — (x − 3)y′ + 2y = 0

~~~text
y = sum c_n x^n
y′ = Σ (n+1)c_{n+1}x^n

(x − 3)y′ + 2y = 0 ထဲ substitute
~~~

Coefficient comparison မှ—

~~~text
(n + 2)c_n − 3(n + 1)c_{n+1} = 0
c_{n+1} = (n + 2)c_n / [3(n + 1)]
c_n = (n + 1)c_0 / 3ⁿ
~~~

Series နှင့် radius—

~~~text
y = c_0[1 + 2(x/3) + 3(x/3)² + 4(x/3)³ + ⋯]
R = 3
~~~

---

## 12. Unit II No. 6 — (x − 1)y′ + 2y = 0

Unit II No. 5 နှင့် အဆင့်တူပြီး 3 နေရာတွင် 1 ပြောင်းပါ။

~~~text
(n + 2)c_n − (n + 1)c_{n+1} = 0
c_{n+1} = (n + 2)c_n/(n + 1)
c_n = (n + 1)c_0
~~~

~~~text
y = c_0[1 + 2x + 3x² + 4x³ + ⋯]
R = 1
~~~

**General shortcut:** (x − a)y′ + 2y = 0 ဆိုလျှင်—

~~~text
c_{n+1} = (n + 2)c_n/[a(n + 1)]
c_n = (n + 1)c_0/aⁿ
R = |a|
~~~

---

## 13. Unit II No. 2 / Assignment 2 No. 4 — y″ + y = 0

~~~text
y = sum c_n x^n
y″ = Σ (n+2)(n+1)c_{n+2}x^n

(n + 2)(n + 1)c_{n+2} + c_n = 0
c_{n+2} = −c_n/[(n+2)(n+1)]
~~~

Even powers နှင့် odd powers ခွဲလျှင်—

~~~text
y = c_0(1 − x²/2! + x⁴/4! − ⋯)
  + c_1(x − x³/3! + x⁵/5! − ⋯)

y = c_0 cos x + c_1 sin x
~~~

---

## 14. Unit II No. 7 — Power-series IVP

~~~text
(x² + 1)y″ + 2xy′ − 2y = 0
y(0) = 0,  y′(0) = 1
~~~

Coefficient comparison မှ—

~~~text
c_{n+2} = (1 − n)c_n/(n + 1)
~~~

Initial conditions—

~~~text
c_0 = y(0) = 0
c_1 = y′(0) = 1
~~~

ထို့နောက် recurrence ကိုအသုံးပြုလျှင် c_2, c_3, c_4, … အားလုံး 0 ဖြစ်သည်။

~~~text
Final answer: y = x
~~~

**စာရွက်ထဲတွင် y′(0)=1 ⇒ c_1=0 ဟုပါလာလျှင် typo ဖြစ်သည်။ မှန်သည်မှာ c_1 = 1 ဖြစ်သည်။**

---

## 15. Final-answer map

| မေးခွန်း | အဓိကနည်း | မှတ်ရန် final result |
|---|---|---|
| Unit I No. 4 | 3rd-order general solution + IVP | y = (3/2)eˣ − 3e²ˣ + (3/2)e³ˣ |
| Unit I No. 6 | Resonance / appropriate y_p | y_p = xe⁻³ˣ(A cos 2x + B sin 2x) |
| Unit I No. 8 | y_c + y_p + IVP | eˣ(2 cos x − (5/2)sin x) + (1/2)x + 1 |
| Unit I No. 9 | Variation of parameters | y_p = (2/3)eˣ |
| Unit II No. 5 | Power series | c_n = (n+1)c_0/3ⁿ, R = 3 |
| Unit II No. 6 | Power series | c_n = (n+1)c_0, R = 1 |
| Unit II No. 7 | Power-series IVP | y = x |
| Assignment 1 No. 1(i) | Verify solution | Substitute → 0 |
| Assignment 1 No. 1(ii) | Repeated root | y = (C_1+C_2x)e²ˣ⁄³ |
| Assignment 1 No. 4 | 3rd-order IVP | y = 2e⁻⁵ˣ + 5e²ˣ |
| Assignment 2 No. 4 | Power series | y = c_0 cos x + c_1 sin x |

---

## 16. စာမေးပွဲခန်းထဲတွင် မမေ့ရန်

1. y′ နှင့် y″ ကို မရောပါနှင့်။
2. Repeated root တွင် x မထည့်မိခြင်းသည် အမှားအများဆုံးဖြစ်သည်။
3. Power series တွင် c_0 = y(0), c_1 = y′(0) ဖြစ်သည်။
4. W = y_1y_2′ − y_1′y_2 ၏ sign ကို စစ်ပါ။
5. RHS နှင့် y_c ထပ်နေလျှင် y_p ကို x မြှောက်ပါ။
6. Radius of convergence R သည် positive distance ဖြစ်သည်။
7. အဖြေမပြီးလျှင်တောင် method, formula, substitution, recurrence ကိုရေးထားပါ—partial marks ရနိုင်သည်။

### အချိန်အလွန်နည်းလျှင် ပြန်ကြည့်ရမည့်အစီအစဉ်

~~~text
1. Section 2 — method ခွဲခြားခြင်း
2. Section 3 — characteristic roots
3. Section 10 — power-series steps
4. Section 11–14 — power-series မေးခွန်း ၄ မျိုး
5. Section 15 — final-answer map
~~~
