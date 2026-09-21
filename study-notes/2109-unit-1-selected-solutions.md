# Paper 2109 Unit 1 — ရွေးထားသောပုဒ်စာများ ရှင်းပြချက်

သိမ်းသည့်ရက် — 2026-09-18

ဒီ note သည် [2109-all-selected-questions-v2.png](../study-pages/2109/2109-all-selected-questions-v2.png) တွင် စုစည်းထားသော Unit 1 ရွေးထားသည့် မေးခွန်းများ၏ solution notes ဖြစ်သည်။ Vector Algebra မေးခွန်း No. 1–6 နှင့် Vector Calculus မေးခွန်းများကို မေးခွန်းနံပါတ် မလွဲစေရန် source list အတိုင်း စီထားသည်။

## အခြေခံသင်္ကေတများ

- `i, j, k` သည် x၊ y၊ z directions ရှိ unit vectors များဖြစ်သည်။
- Dot product `a · b` သည် scalar ထွက်ပြီး `a · b = 0` ဖြစ်လျှင် non-zero vectors နှစ်ခု perpendicular ဖြစ်သည်။
- Cross product `a × b` သည် vector ထွက်သည်။
- Vector magnitude `|a| = sqRoot(a · a)` ဖြစ်သည်။
- Function `phi(x,y,z)` ၏ gradient သည် `grad phi = phi_x i + phi_y j + phi_z k` ဖြစ်သည်။

## No. 1 — Ex. 1.1: Vector magnitude identity

### မေးခွန်း

`a = a1 i + a2 j + a3 k` အတွက်

`|a| = sqrt(a · a) = sqrt(a1^2 + a2^2 + a3^2)`

ဖြစ်ကြောင်း ပြပါ။

### ရှင်းပြချက်

Unit vectors များ၏ dot-product rules များမှာ `i · i = j · j = k · k = 1` နှင့် `i · j = j · k = k · i = 0` ဖြစ်သည်။ ထို့ကြောင့်

`a · a = (a1 i + a2 j + a3 k) · (a1 i + a2 j + a3 k)`

`= a1^2(i·i) + a2^2(j·j) + a3^2(k·k)`

`+ 2a1a2(i·j) + 2a2a3(j·k) + 2a3a1(k·i)`

Cross terms များသည် zero ဖြစ်သောကြောင့် `a · a = a1^2 + a2^2 + a3^2` ဖြစ်သည်။ Vector magnitude definition အရ

`|a| = sqrt(a · a) = sqrt(a1^2 + a2^2 + a3^2)`။

### အဖြေ

လိုချင်သည့် identity ကို သက်သေပြပြီးဖြစ်သည်။

## No. 2 — Model Question No. 2: `angle ABC` သည် right angle

### ပေးထားချက်

`a = 5i + 3j + 2k`, `b = 2i - j + 3k`, `c = 7i - 3j + 10k`

ဒီနေရာတွင် `a, b, c` သည် A, B, C ၏ position vectors ဖြစ်သည်။ Angle ABC သည် B မှထွက်သော `BA` နှင့် `BC` vectors ကြား angle ဖြစ်သည်။

### တွက်ချက်ခြင်း

`BA = a - b = (5-2)i + (3-(-1))j + (2-3)k`

`= 3i + 4j - k`

`BC = c - b = (7-2)i + (-3-(-1))j + (10-3)k`

`= 5i - 2j + 7k`

`BA · BC = (3)(5) + (4)(-2) + (-1)(7) = 15 - 8 - 7 = 0`

Dot product zero ဖြစ်သောကြောင့် `BA` နှင့် `BC` သည် perpendicular ဖြစ်သည်။

### အဖြေ

`angle ABC = 90°` ဖြစ်သည်။

## No. 3 — S.A. 1.1 (1): Vectors နှစ်ခုကြား angle

### ပေးထားချက်

`a = 2i + 2j - k`, `b = 6i - 3j + 2k`

### Dot product နှင့် magnitude

`a · b = (2)(6) + (2)(-3) + (-1)(2) = 12 - 6 - 2 = 4`

`|a| = sqrt(2^2 + 2^2 + (-1)^2) = sqrt(9) = 3`

`|b| = sqrt(6^2 + (-3)^2 + 2^2) = sqrt(49) = 7`

Angle formula `a · b = |a||b| cos(theta)` ဖြစ်သောကြောင့်

`4 = (3)(7) cos(theta)`

`cos(theta) = 4/21`

`theta = cos^(-1)(4/21) approx 79°`

### အဖြေ

`theta = cos^(-1)(4/21) approx 79°`။

## No. 4 — S.A. 1.1 (2)(i): Scalar triple product

### ပေးထားချက်

`q = i + 2j - 3k = (1,2,-3)`

`b = 2i - j + k = (2,-1,1)`

`c = -i + 4j - k = (-1,4,-1)`

ရှာရန်မှာ `q · (b × c)` ဖြစ်သည်။

### `b × c`

`b × c = | i  j  k ; 2  -1  1 ; -1  4  -1 |`

`= ((-1)(-1)-1(4))i - (2(-1)-1(-1))j + (2(4)-(-1)(-1))k`

`= -3i + j + 7k`

### Dot product

`q · (b × c) = (1,2,-3) · (-3,1,7)`

`= -3 + 2 - 21 = -22`

### အဖြေ

`q · (b × c) = -22`။

## No. 5 — S.A. 1.1 (2)(ii): Vector triple product

ရှာရန်မှာ `(q × b) × c` ဖြစ်သည်။

### Direct cross products

`q × b = | i  j  k ; 1  2  -3 ; 2  -1  1 | = -i - 7j - 5k`

ထို့ကြောင့်

`(q × b) × c = (-1,-7,-5) × (-1,4,-1)`

`= (27,4,-11) = 27i + 4j - 11k`

### Vector triple-product identity ဖြင့် စစ်ခြင်း

`(q × b) × c = b(q · c) - q(b · c)`

`q · c = (1)(-1)+(2)(4)+(-3)(-1)=10`

`b · c = (2)(-1)+(-1)(4)+(1)(-1)=-7`

ထို့ကြောင့်

`(q × b) × c = 10b - (-7)q = 10b + 7q`

`= (20,-10,10)+(7,14,-21) = (27,4,-11)`။

### အဖြေ

`(q × b) × c = 27i + 4j - 11k`။

## No. 6 — Ex. 1.2: `(a × b) × c`

### ပေးထားချက်

`a = 3i - j + 2k = (3,-1,2)`

`b = 2i + j - k = (2,1,-1)`

`c = 2i - 2j + 2k = (2,-2,2)`

### `a × b`

`a × b = | i  j  k ; 3  -1  2 ; 2  1  -1 | = -i + 7j + 5k`

ထို့ကြောင့်

`(a × b) × c = (-1,7,5) × (2,-2,2)`

`= (24,12,-12) = 24i + 12j - 12k`

### အဖြေ

`(a × b) × c = 24i + 12j - 12k`။

## No. 7 — Question No. 3: Directional derivative

### ပေးထားချက်

`phi = x^2 y z + 4xz^2`

Point = `(1,-2,-1)`၊ direction vector `d = 2i - j - 2k = (2,-1,-2)`

Directional derivative အတွက် gradient ကိုရှာပြီး direction vector ကို unit vector ပြောင်းရမည်။

### Gradient

`phi_x = 2xyz + 4z^2`

`phi_y = x^2z`

`phi_z = x^2y + 8xz`

Point `(1,-2,-1)` တွင်

`phi_x = 2(1)(-2)(-1) + 4(-1)^2 = 8`

`phi_y = (1)^2(-1) = -1`

`phi_z = (1)^2(-2) + 8(1)(-1) = -10`

ထို့ကြောင့် `grad phi = 8i - j - 10k`။

### Unit direction vector

`|d| = sqrt(2^2 + (-1)^2 + (-2)^2) = sqrt(9) = 3`

`u = d/|d| = (2i - j - 2k)/3`

### Directional derivative

`D_u phi = grad phi · u`

`= (8,-1,-10) · (2,-1,-2)/3`

`= (16 + 1 + 20)/3 = 37/3`

### အဖြေ

**Directional derivative = `37/3`.** Learner confirmation ရရှိထားသည်။

## No. 8 — Question No. 1: `1/r` သည် harmonic ဖြစ်ကြောင်းပြခြင်း

### သတ်မှတ်ချက်

`r = [x,y,z]` ဟုယူပြီး `r = sqrt(x^2+y^2+z^2)` ဖြစ်သည်။ Harmonic function ဆိုသည်မှာ Laplacian သုညဖြစ်သော function ဖြစ်သည်။ သက်သေပြရန် `nabla^2(1/r) = 0` ကိုရှာရမည်။ `r = 0` တွင် `1/r` မသတ်မှတ်နိုင်သောကြောင့် result သည် `r != 0` အတွက် ဖြစ်သည်။

### First and second partial derivatives

`phi = 1/r = (x^2+y^2+z^2)^(-1/2)` ဟုယူလျှင်

`phi_x = -x/r^3`, `phi_y = -y/r^3`, `phi_z = -z/r^3`

`phi_xx = -1/r^3 + 3x^2/r^5`

`phi_yy = -1/r^3 + 3y^2/r^5`

`phi_zz = -1/r^3 + 3z^2/r^5`

ထို့ကြောင့်

`nabla^2 phi = phi_xx + phi_yy + phi_zz`

`= -3/r^3 + 3(x^2+y^2+z^2)/r^5`

`= -3/r^3 + 3r^2/r^5 = -3/r^3 + 3/r^3 = 0`

### အဖြေ

`nabla^2(1/r)=0` for `r != 0` ဖြစ်သောကြောင့် **`1/r` သည် harmonic function ဖြစ်သည်**။

**အခြေအနေ — explanation deferred / learner confirmation pending.**

## No. 9 — Question No. 2: Closed circuit

### မေးခွန်း

`C` သည် area `S` ကို ဝန်းရံထားသော closed circuit ဖြစ်လျှင် `integral_C phi grad(phi) · ds = 0` ဖြစ်ကြောင်း ပြပါ။

### Gradient identity

Scalar function `phi` အတွက် chain rule ဖြင့်

`grad(phi^2/2) = phi grad(phi)`

ဖြစ်သည်။ ထို့ကြောင့်

`integral_C phi grad(phi) · ds = integral_C grad(phi^2/2) · ds`

ဖြစ်သည်။

Gradient field တစ်ခု၏ line integral သည် endpoint potential difference ဖြစ်သည်။

`integral_A^B grad(phi^2/2) · ds = [phi^2/2]_A^B`

Closed circuit တွင် starting point နှင့် ending point တူသောကြောင့် `[phi^2/2]_A^A = 0` ဖြစ်သည်။ ထို့ကြောင့်

`integral_C phi grad(phi) · ds = 0`

ဖြစ်သည်။

### Green's theorem ဖြင့် စစ်နိုင်သောပုံစံ

2-D တွင် `grad(phi)·ds = phi_x dx + phi_y dy` ဖြစ်သောကြောင့် integrand သည်

`phi phi_x dx + phi phi_y dy`

ဖြစ်သည်။ Green's theorem ဖြင့် area integral သို့ပြောင်းလျှင်

`partial(phi phi_y)/partial x - partial(phi phi_x)/partial y`

`= (phi_x phi_y + phi phi_xy) - (phi_y phi_x + phi phi_yx) = 0`

ဖြစ်သည်။ Mixed partial derivatives တူသည်ဟု ယူသောအခါ result သည် zero ဖြစ်သည်။

**အခြေအနေ — explanation given; learner confirmation pending.**

## No. 10 — Question No. 3: Gradient နှင့် directional derivative

### ပေးထားချက်

`phi(x,y,z) = 2x^2 - 3xy + 9z - 2`

Point = `(1,0,0)`၊ direction = `[2,-2,1]`

### Gradient

`phi_x = 4x - 3y`, `phi_y = -3x`, `phi_z = 9`

ထို့ကြောင့် `grad phi = (4x-3y)i - 3xj + 9k` ဖြစ်ပြီး point `(1,0,0)` တွင်

`grad phi(1,0,0) = 4i - 3j + 9k`

### Unit direction vector

`d = 2i - 2j + k`

`|d| = sqrt(2^2+(-2)^2+1^2) = sqrt(9)=3`

`u = d/|d| = (2i-2j+k)/3`

### Directional derivative

`D_u phi = grad phi · u`

`= (4,-3,9) · (2,-2,1)/3`

`= (8+6+9)/3 = 23/3`

### အဖြေ

- Gradient at `(1,0,0)` = **`4i - 3j + 9k`**
- Directional derivative in `[2,-2,1]` direction = **`23/3`**

**အခြေအနေ — explanation pending / learner confirmation pending.**

## အမှားမဖြစ်ရန် မှတ်ချက်

- Angle ABC တွင် A နှင့် C ၏ position vectors ကို တိုက်ရိုက် dot မလုပ်ရ။ `BA = a-b` နှင့် `BC = c-b` ကို အရင်ဖွဲ့ရမည်။
- Directional derivative တွင် ပေးထားသော direction vector ကို unit vector မပြောင်းဘဲ gradient နှင့် dot လုပ်လျှင် အဖြေမှားနိုင်သည်။
- `(a × b) × c` နှင့် `a × (b × c)` မတူပါ။ Brackets ကို မဖျက်ရ။
- `1/r` ၏ harmonic proof တွင် `r=0` ကို မထည့်ရ။ Origin တွင် function မသတ်မှတ်နိုင်ပါ။
- Closed curve line integral သုညဖြစ်ရန် field သည် `grad(phi^2/2)` ကဲ့သို့ gradient/conservative field ဖြစ်ကြောင်း အရင်ပြရမည်။

## လက်ရှိအခြေအနေ အကျဉ်း

| မေးခွန်း                                                     | အခြေအနေ                                                           |
| -------------------------------------------------------------------- | ------------------------------------------------------------------------ |
| Ex. 1.1; Model Q No. 2; S.A. 1.1 (1); S.A. 1.1 (2)(i), (ii); Ex. 1.2 | ရှင်းပြပြီး learner confirmation ရရှိ — ပြီးဆုံး |
| Question No. 3 — Directional derivative                             | ရှင်းပြပြီး learner confirmation ရရှိ — ပြီးဆုံး |
| Question No. 1 — Harmonic function                                  | Reference solution သိမ်းထား — confirmation pending              |
| Question No. 2 — Closed circuit                                     | Explanation သိမ်းထား — confirmation pending                     |
| Question No. 3 — Gradient                                           | Reference solution သိမ်းထား — confirmation pending              |
