# Trigonometric Ratios — Additional Foundation

ဒီ note ကို Paper 2103 Unit 1 No.10 ဖြေရှင်းရာမှာ လိုအပ်တဲ့ `sin`, `cos`, `tan` အခြေခံများကို နောင်ပြန်လေ့လာနိုင်ရန် သိမ်းထားသည်။

## ၁။ ညာထောင့်တြိဂံ၏ အနားများ

ညာထောင့်တြိဂံတစ်ခုတွင် လေ့လာမည့်ထောင့်ကို `θ` ဟုထားသည်။

- **Hypotenuse (H)** — ညာထောင့် `90°` ၏ မျက်နှာချင်းဆိုင်အနားဖြစ်ပြီး အရှည်ဆုံးအနား။
- **Opposite (O)** — `θ` ထောင့်၏ မျက်နှာချင်းဆိုင်အနား။
- **Adjacent (A)** — `θ` ထောင့်နှင့် ကပ်နေသောအနား၊ hypotenuse မဟုတ်သောအနား။

## ၂။ အခြေခံပုံသေနည်းများ

`SOH-CAH-TOA` ဟု မှတ်နိုင်သည်။

```text
sin θ = Opposite / Hypotenuse = O / H
cos θ = Adjacent / Hypotenuse = A / H
tan θ = Opposite / Adjacent   = O / A
```

`tan θ` သည် `sin θ / cos θ` နှင့်လည်း တူသည်။

```text
tan θ = sin θ / cos θ
```

## ၃။ Special-angle တန်ဖိုးများ ဘယ်ကလာသလဲ

### 30° နှင့် 60°

Equilateral triangle တစ်ခု၏ ဘေးအရှည်ကို `2` ထားပြီး တစ်ဝက်ခွဲလျှင် `30°-60°-90°` ညာထောင့်တြိဂံရသည်။ အနားအချိုးများမှာ—

```text
30° ၏ မျက်နှာချင်းဆိုင်အနား = 1
60° ၏ မျက်နှာချင်းဆိုင်အနား = √3
Hypotenuse = 2
```

ထို့ကြောင့်—

```text
sin 30° = 1 / 2
cos 30° = √3 / 2
tan 30° = 1 / √3 = √3 / 3

sin 60° = √3 / 2
cos 60° = 1 / 2
tan 60° = √3
```

### 45°

Square တစ်ခု၏ ဘေးအရှည်ကို `1` ထားပြီး ထောင့်ဖြတ်မျဉ်းဆွဲလျှင် `45°-45°-90°` ညာထောင့်တြိဂံရသည်။ Pythagoras theorem အရ hypotenuse သည် `√2` ဖြစ်သည်။

```text
sin 45° = 1 / √2 = √2 / 2
cos 45° = 1 / √2 = √2 / 2
tan 45° = 1 / 1 = 1
```

## ၄။ မကြာခဏအသုံးပြုသော တန်ဖိုးဇယား

| ထောင့် `θ` | `0°` | `30°` | `45°` | `60°` | `90°` |
|---|---:|---:|---:|---:|---:|
| `sin θ` | `0` | `1/2` | `√2/2` | `√3/2` | `1` |
| `cos θ` | `1` | `√3/2` | `√2/2` | `1/2` | `0` |
| `tan θ` | `0` | `√3/3` | `1` | `√3` | မသတ်မှတ်နိုင် |

### Sine ကို အလွယ်မှတ်နည်း

`0°, 30°, 45°, 60°, 90°` အစဉ်အတိုင်း—

```text
sin θ = √0/2, √1/2, √2/2, √3/2, √4/2
```

Cosine သည် sine စာရင်းကို ပြောင်းပြန်ဖတ်ခြင်းဖြစ်သည်။

## ၅။ Force components တွင် အသုံးပြုပုံ

Force `F` သည် positive `x`-axis နှင့် `θ` ထောင့်ရှိလျှင်—

```text
horizontal component = F cos θ
vertical component   = F sin θ
```

အကြောင်းရင်းမှာ force vector ကို ညာထောင့်တြိဂံ၏ hypotenuse အဖြစ်မြင်လျှင် horizontal ဘက်သည် adjacent side၊ vertical ဘက်သည် opposite side ဖြစ်သောကြောင့် ဖြစ်သည်။

ဥပမာ Force `2` သည် `60°` ရှိလျှင်—

```text
horizontal = 2 cos 60° = 2(1/2) = 1
vertical   = 2 sin 60° = 2(√3/2) = √3
```

Force တစ်ခု ဘယ်ဘက်သို့ ဦးတည်လျှင် horizontal component ကို negative ထားရသည်။ အပေါ်သို့ ဦးတည်လျှင် vertical component positive ဖြစ်သည်။

Paper 2103 No.10 တွင် Force `4` ၏ direction angle သည် positive `x`-axis မှ `150°` ဖြစ်သည်။ ထို့ကြောင့်—

```text
4 cos 150° = 4(-cos 30°) = -2√3
4 sin 150° = 4(sin 30°)  = 2
```

`150° = 180° - 30°` ဖြစ်သောကြောင့် second quadrant တွင် `x` သည် negative၊ `y` သည် positive ဖြစ်သည်။

## ၆။ Direction ရှာရာတွင် သတိပြုရန်

Resultant components ကို `R_x` နှင့် `R_y` ဟုထားလျှင်—

```text
R = √(R_x² + R_y²)
tan θ = R_y / R_x
```

`R_x < 0` နှင့် `R_y > 0` ဖြစ်လျှင် resultant သည် second quadrant တွင်ရှိသည်။ Calculator မှရသော negative reference angle ကို တိုက်ရိုက်မယူဘဲ quadrant ကိုစစ်ရမည်။

## ၇။ မကြာခဏမှားတတ်သောအချက်များ

- `sin` နှင့် `cos` ကို ပြောင်းပြန်မသုံးရ။ `x`-axis မှ angle တိုင်းလျှင် horizontal သည် `cos`၊ vertical သည် `sin` ဖြစ်သည်။
- Force ဘယ်ဘက်သို့ ဦးတည်လျှင် `x` component ကို negative ထားရသည်။
- `tan 90°` သည် denominator `cos 90° = 0` ဖြစ်သောကြောင့် မသတ်မှတ်နိုင်။
- Calculator ကို degree ဖြင့်တွက်မည့်အခါ `DEG` mode ထားရသည်။ `RAD` mode ဖြစ်လျှင် တန်ဖိုးများမှားနိုင်သည်။
- `1/√3` ကို rationalised form ဖြင့် `√3/3` ဟုရေးနိုင်သည်။

## ၈။ လေ့လာမှုအခြေအနေ

Learner သည် ဤအခြေခံရှင်းပြချက်များကို Paper 2103 Unit 1 No.10 နှင့်အတူ လေ့လာပြီးဖြစ်သည်။ နောင် force components၊ resultant နှင့် trigonometry မေးခွန်းများတွင် ပြန်လည်အသုံးပြုရန် သိမ်းထားသည်။
