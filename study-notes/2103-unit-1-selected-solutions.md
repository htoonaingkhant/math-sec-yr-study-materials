# Paper 2103 Unit 1 — ရွေးထားသောပုဒ်စာများ ရှင်းပြချက်

သိမ်းသည့်ရက် — 2026-09-18

ဒီ note သည် Paper 2103 Unit 1 မှ အတည်ပြုပြီးသား ရွေးထားသော No. 5, 6, 7, 10, 11 မေးခွန်းများ၏ ရှင်းပြချက်နှင့် full working ကို ပြန်လည်အသုံးပြုရန် သိမ်းထားခြင်းဖြစ်သည်။ Source reference pages များမှာ [page-02.png](../study-pages/2103/unit-1/page-02.png), [page-03.png](../study-pages/2103/unit-1/page-03.png), [page-05.png](../study-pages/2103/unit-1/page-05.png), [page-06.png](../study-pages/2103/unit-1/page-06.png) ဖြစ်သည်။

## အသုံးပြုသည့် အခြေခံနည်းများ

- String equilibrium တွင် force သုံးခု ဆုံသည့် point ကို ကြည့်ပြီး Lami's theorem ကို သုံးသည်။
- Lami's theorem — equilibrium ဖြစ်သော force သုံးခုအတွက် `P / sin(alpha) = Q / sin(beta) = R / sin(gamma)` ဖြစ်ပြီး angle တစ်ခုစီသည် ထို angle ၏ ဆန့်ကျင်ဘက် force နှစ်ခုကြား angle ဖြစ်သည်။
- Force များကို x၊ y components ခွဲလျှင် `X = sum(F cos theta)`, `Y = sum(F sin theta)` ဖြစ်သည်။
- Resultant magnitude နှင့် direction ကို `R = sqrt(X^2 + Y^2)`, `tan(theta) = Y / X` ဖြင့် ရှာသည်။ Quadrant ကို စစ်ပြီးမှ direction angle ကို သတ်မှတ်ရမည်။

## No. 5 — 50 lb mass, 3 ft နှင့် 4 ft strings

### ပေးထားချက်နှင့် geometry

- Mass ၏ weight = `50 lb wt`
- Strings အရှည်များ = `3 ft`, `4 ft`
- အပေါ်ဘက် attachment points ကြား အကွာ = `5 ft`
- ထို့ကြောင့် `3-4-5` right triangle ဖြစ်ပြီး C point ရှိ string နှစ်ချောင်းကြား angle သည် `90°` ဖြစ်သည်။
- `T1` သည် 3 ft string ၏ tension၊ `T2` သည် 4 ft string ၏ tension ဟု သတ်မှတ်သည်။

C point တွင် `T1`, `T2`, `50` သည် equilibrium ဖြစ်သော force သုံးခုဖြစ်သောကြောင့် Lami's theorem ကို သုံးနိုင်သည်။

### တွက်ချက်ခြင်း

`T1 / cos(beta) = T2 / cos(alpha) = 50 / sin(90°)`

ထို့ကြောင့်

`T1 = 50 cos(beta) = 50(4/5) = 40 lb wt`

`T2 = 50 cos(alpha) = 50(3/5) = 30 lb wt`

### အဖြေ

- 3 ft string ၏ tension = **40 lb wt**
- 4 ft string ၏ tension = **30 lb wt**

## No. 6 — 90 lb mass, 9 ft နှင့် 12 ft strings

### ပေးထားချက်နှင့် geometry

- Weight = `90 lb wt`
- Strings အရှည်များ = `9 ft`, `12 ft`
- Attachment points ကြား အကွာ = `15 ft`
- `9-12-15` right triangle ဖြစ်သည်။

`T1` ကို 9 ft string ၏ tension၊ `T2` ကို 12 ft string ၏ tension ဟု သတ်မှတ်သည်။

### တွက်ချက်ခြင်း

Lami's theorem နှင့် `sin(90°) = 1` ကို သုံးလျှင်

`T1 / cos(beta) = T2 / cos(alpha) = 90 / sin(90°) = 90`

ထို့ကြောင့်

`T1 = 90 cos(beta) = 90(12/15) = 72 lb wt`

`T2 = 90 cos(alpha) = 90(9/15) = 54 lb wt`

### အဖြေ

- 9 ft string ၏ tension = **72 lb wt**
- 12 ft string ၏ tension = **54 lb wt**

## No. 7 — Horizontal string BC နှင့် weights 10 lb၊ omega

### ပေးထားချက်

- AB သည် horizontal နှင့် `45°` ပြုသည်။
- CD သည် horizontal နှင့် `60°` ပြုသည်။
- B တွင် weight `10 lb wt`၊ C တွင် weight `omega` ရှိသည်။
- BC သည် horizontal ဖြစ်သည်။

### B point တွင် tension BC

B point တွင် force သုံးခုမှာ AB string tension၊ BC string tension `T2` နှင့် downward weight `10` ဖြစ်သည်။ Lami's theorem ဖြင့်

`T1 / sin(90°) = T2 / sin(135°) = 10 / sin(135°)`

Source diagram ၏ angle relationship အရ `T2 / sin(135°) = 10 / sin(135°)` ဖြစ်သောကြောင့်

`T2 = 10 lb wt`

### C point တွင် omega

C point တွင် ဘယ်ဘက်သို့ `T2 = 10`၊ ညာဘက်အပေါ်သို့ CD tension နှင့် အောက်သို့ `omega` ရှိသည်။ ထို force သုံးခုအတွက် Lami's theorem သည်

`10 / sin(150°) = omega / sin(120°) = T3 / sin(90°)`

ဖြစ်သည်။ ထို့ကြောင့်

`omega / sin(120°) = 10 / sin(150°)`

`omega = 10 sin(120°) / sin(150°)`

`= 10(√3/2)/(1/2) = 10√3 lb wt`

### အဖြေ

- String BC ၏ tension = **10 lb wt**
- `omega = 10√3 lb wt` (ခန့်မှန်း `17.32 lb wt`)

## No. 10 — Forces 1, 2, 3, 4 lb နှင့် resultant

### Direction များကို သတ်မှတ်ခြင်း

ပုံအရ x-axis ကို ညာဘက်အပြုသဘော၊ y-axis ကို အပေါ်ဘက်အပြုသဘော ယူလျှင်

- Force 1 သည် `0°`
- Force 2 သည် `60°`
- Force 3 သည် `90°`
- Force 4 သည် `150°` ဖြစ်သည် (`-x` axis အပေါ် `30°`)

### x-component

`X = 1 cos(0°) + 2 cos(60°) + 3 cos(90°) + 4 cos(150°)`

`= 1 + 2(1/2) + 3(0) + 4(-√3/2)`

`= 2 - 2√3 ≈ -1.464`

### y-component

`Y = 1 sin(0°) + 2 sin(60°) + 3 sin(90°) + 4 sin(150°)`

`= 0 + 2(√3/2) + 3 + 4(1/2)`

`= 5 + √3 ≈ 6.732`

### Resultant magnitude

`R = sqrt(X^2 + Y^2)`

`= sqrt((-1.464)^2 + (6.732)^2)`

`≈ 6.9 lb wt`

### Direction

X သည် negative၊ Y သည် positive ဖြစ်သောကြောင့် resultant သည် Quadrant II တွင် ရှိသည်။

`tan(theta) = Y/X = 6.732/(-1.464)`

Reference angle ကို quadrant နှင့် ပြန်ညှိလျှင်

`theta ≈ 102°16'` with the positive horizontal direction.

### အဖြေ

**Resultant ≈ 6.9 lb wt, direction ≈ 102°16' from the positive horizontal axis.**

## No. 11 — Forces 4, 3, 2, 1 lb နှင့် resultant

### Direction များ

AB ကို positive x-axis ဟု ယူလျှင်

- Force 4 သည် `0°`
- Force 3 သည် `30°`
- Force 2 သည် `60°`
- `∠DAE = 90°` ဖြစ်သောကြောင့် Force 1 သည် `150°`

### x-component

`X = 4 cos(0°) + 3 cos(30°) + 2 cos(60°) + 1 cos(150°)`

`= 4 + 3(√3/2) + 2(1/2) - √3/2`

`= 5 + √3`

### y-component

`Y = 4 sin(0°) + 3 sin(30°) + 2 sin(60°) + 1 sin(150°)`

`= 0 + 3(1/2) + 2(√3/2) + 1(1/2)`

`= 2 + √3`

### Resultant magnitude

`R = sqrt((5+√3)^2 + (2+√3)^2)`

`= sqrt(35 + 14√3) ≈ 7.7 lb wt`

### Direction

`tan(theta) = (2+√3)/(5+√3)`

ထို့ကြောင့်

`theta ≈ 29°` with AB.

### အဖြေ

**Resultant ≈ 7.7 lb wt, inclination ≈ 29° to AB.**

## အမှားမဖြစ်ရန် မှတ်ချက်

- Force 4 ကို `30°` ဟု တိုက်ရိုက်မယူရ။ Positive x-axis မှ direction သည် `150°` ဖြစ်သောကြောင့် x-component သည် negative ဖြစ်ရမည်။
- `tan(theta) = Y/X` တွင် X negative ဖြစ်လျှင် quadrant ကို စစ်ရမည်။ No. 10 တွင် angle ကို `77°` ဟု မရေးဘဲ Quadrant II ကြောင့် `102°16'` ဟု ပြင်ရသည်။
- String tension မေးခွန်းများတွင် string အရှည်များသည် triangle sides ဖြစ်သဖြင့် `3-4-5` နှင့် `9-12-15` ratios ကို အရင်ရှာပြီးမှ Lami's theorem သုံးလျှင် လွယ်ကူသည်။

### လက်ရှိအခြေအနေ

No. 5, 6, 7, 10, 11 — ရှင်းပြပြီး learner confirmation ရရှိထားသဖြင့် **ပြီးဆုံးပြီးသား**။
