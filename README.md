<p align="center">
    <img src="https://www.liqpay.ua/logo_liqpay_main.svg" width="250" height="119" />
</p>

# Liqpay
Android Library to implement Liqpay integration easily to application 💳

[![](https://jitpack.io/v/AleksandrHavrylenko/Liqpay.svg)](https://jitpack.io/#AleksandrHavrylenko/Liqpay)

### [Visit official documentation for the details](https://www.liqpay.ua/documentation/en/)

## Install
Step 1. Add it in your root build.gradle at the end of repositories:
```
allprojects {
    repositories {
        maven { url 'https://jitpack.io' }
    }
}
```

Step 2. Add the dependency

```
dependencies {
    implementation 'com.github.AleksandrHavrylenko:Liqpay:0.2.0'
}
```
## Usage

```
val liqpay = LiqPay(context = this, callback = this)
    liqpay.checkout(
              privateKey = LIQPAY_PRIVATE_KEY,
              publicKey = LIQPAY_PUBLIC_KEY,
              amount = 1.0,
              description = "test",
              orderId = "1231423423"
        )
```

## License

```
   Copyright 2021 Bulan Yurii

   Licensed under the Apache License, Version 2.0 (the "License");
   you may not use this file except in compliance with the License.
   You may obtain a copy of the License at

       http://www.apache.org/licenses/LICENSE-2.0

   Unless required by applicable law or agreed to in writing, software
   distributed under the License is distributed on an "AS IS" BASIS,
   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
   See the License for the specific language governing permissions and
   limitations under the License.
```
