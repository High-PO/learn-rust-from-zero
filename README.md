## 업데이트

![example workflow name](https://github.com/Dhghomon/easy_rust/workflows/github%20pages/badge.svg)

2023년 1월 19일: [Learn Rust in a Month of Lunches](https://www.manning.com/books/learn-rust-in-a-month-of-lunches)가 이제 Manning에서 구매 가능합니다. Rust in a Month of Lunches는 기존 Easy Rust의 내용을 기반으로 하되, 독자 피드백을 반영하여 개선하고 확장한 버전입니다(약 두 배의 분량).

![](Learn_Rust_in_a_Month_of_Lunches.png)

2022년 10월 31일: [이제 스페인어로도 이용 가능합니다](https://www.jmgaguilera.com/rust_facil/)

2021년 5월 23일: [Ariandy](https://github.com/ariandy)/[1kb](https://1kilobyte.github.io/) 덕분에 [이제 인도네시아어로도 이용 가능합니다](https://github.com/ariandy/easy-rust-indonesia).

2021년 4월 2일: 커피 한 잔 사주고 싶으신 분들을 위해 [BuyMeACoffee 링크를 추가했습니다](https://www.buymeacoffee.com/mithridates).

2021년 2월 1일: [이제 YouTube에서도 시청 가능합니다!](https://www.youtube.com/playlist?list=PLfllocyHVgsRwLkTAhG0E-2QxCf-ozBkk) 두 달 후: 2021년 4월 1일 기준으로 총 186개의 비디오 완성(총 23시간 약간 초과).

2020년 12월 22일: mdBook은 [여기](https://dhghomon.github.io/easy_rust)에서 찾을 수 있습니다.

2020년 11월 28일: [kumakichi](https://github.com/kumakichi) 덕분에 [이제 중국어 간체로도 이용 가능합니다](https://github.com/kumakichi/easy_rust_chs)!

2021년 11월 27일: [Easy Rust 비디오가 이제 한국어로도 녹화되고 있습니다!](https://www.youtube.com/watch?v=W9DO6m8JSSs&list=PLfllocyHVgsSJf1zO6k6o3SX2mbZjAqYE) 한국어판 비디오도 녹화 시작!


from: https://github.com/Dhghomon/easy_rust 

한국어 강의를 친절하게 올려주셨지만 보면서 함께 볼 교안을 한국어로 보고자 AI를 통해 번역을 하였습니다.

직접 작성한 지적 재산권 및 저작권은 저에게 없으며 모두 Dhghomon님이 올려주신 내용을 번역한 것이 전부입니다.

![](Easy_Rust_sample_image.png)

## 소개

Rust는 이미 좋은 교재들을 가지고 있는 새로운 언어입니다. 하지만 때때로 그 교재들은 영어 원어민을 위해 작성되어 있어 어려울 수 있습니다. 많은 회사와 사람들이 이제 Rust를 배우고 있으며, 쉬운 영어로 작성된 책이 있다면 더 빨리 배울 수 있을 것입니다. 이 교재는 이러한 회사와 사람들이 간단한 영어로 Rust를 배울 수 있도록 만들어졌습니다.

Rust는 꽤 새로운 언어이지만 이미 매우 인기가 있습니다. C나 C++의 속도와 제어력을 제공하면서도 Python과 같은 최신 언어들의 메모리 안전성을 제공하기 때문에 인기가 있습니다. 이것은 다른 언어들과는 때때로 다른 몇 가지 새로운 아이디어를 통해 이루어집니다. 즉, 배워야 할 새로운 것들이 있으며, "하면서 파악하기"만으로는 안 됩니다. Rust는 이해하기 위해 한동안 생각해야 하는 언어입니다. 하지만 다른 언어를 알고 있다면 여전히 꽤 친숙해 보이며, 좋은 코드를 작성하는 데 도움이 되도록 만들어졌습니다.

## 저자 소개

저는 한국에 사는 캐나다인이며, 한국의 회사들이 Rust를 사용하기 시작하는 것을 쉽게 만들기 위해 어떻게 할지 생각하면서 Easy Rust를 작성했습니다. 영어를 제1언어로 사용하지 않는 다른 나라들도 이것을 사용할 수 있기를 바랍니다.

## 쉬운 영어로 Rust 작성하기

*Rust in Easy English*는 2020년 7월부터 8월까지 작성되었으며, 400페이지가 넘습니다. 질문이 있으시면 여기나 [LinkedIn](https://www.linkedin.com/in/davemacleod) 또는 [Twitter](https://twitter.com/mithridates)로 연락주세요. 잘못된 부분을 발견하거나 pull request를 만들고 싶으시다면 진행해 주세요. 이미 20명 이상이 오타와 코드 문제를 수정하는 데 도움을 주었으므로 여러분도 참여할 수 있습니다. 저는 세계 최고의 Rust 전문가가 아니므로 항상 새로운 아이디어를 듣거나 책을 개선할 수 있는 부분을 보는 것을 좋아합니다.

- [파트 1 - 브라우저에서 Rust 사용하기](#파트-1---브라우저에서-rust-사용하기)
  - [Rust Playground](#rust-playground)
  - [🚧 와 ⚠️](#-와-️)
  - [주석](#주석)
  - [타입](#타입)
    - [기본 타입](#기본-타입)
  - [타입 추론](#타입-추론)
    - [부동소수점](#부동소수점)
  - [&#39;hello, world!&#39; 출력하기](#hello-world-출력하기)
    - [변수 선언과 코드 블록](#변수-선언과-코드-블록)
  - [Display와 debug](#display와-debug)
    - [가장 작은 수와 가장 큰 수](#가장-작은-수와-가장-큰-수)
  - [가변성 (변경)](#가변성-변경)
    - [섀도잉](#섀도잉)
  - [스택, 힙, 그리고 포인터](#스택-힙-그리고-포인터)
  - [출력에 대한 추가 정보](#출력에-대한-추가-정보)
  - [문자열](#문자열)
  - [const와 static](#const와-static)
  - [참조에 대한 추가 정보](#참조에-대한-추가-정보)
  - [가변 참조](#가변-참조)
    - [다시 섀도잉](#다시-섀도잉)
  - [함수에 참조 전달하기](#함수에-참조-전달하기)
  - [Copy 타입](#copy-타입)
    - [값이 없는 변수](#값이-없는-변수)
  - [컬렉션 타입](#컬렉션-타입)
    - [배열](#배열)
  - [벡터](#벡터)
  - [튜플](#튜플)
  - [제어 흐름](#제어-흐름)
  - [구조체](#구조체)
  - [열거형](#열거형)
    - [여러 타입을 사용하기 위한 열거형](#여러-타입을-사용하기-위한-열거형)
  - [루프](#루프)
  - [구조체와 열거형 구현하기](#구조체와-열거형-구현하기)
  - [구조 분해](#구조-분해)
  - [참조와 점 연산자](#참조와-점-연산자)
  - [제네릭](#제네릭)
  - [Option과 Result](#option과-result)
    - [Option](#option)
    - [Result](#result)
  - [다른 컬렉션들](#다른-컬렉션들)
    - [HashMap (그리고 BTreeMap)](#hashmap-그리고-btreemap)
    - [HashSet과 BTreeSet](#hashset과-btreeset)
    - [BinaryHeap](#binaryheap)
    - [VecDeque](#vecdeque)
  - [? 연산자](#-연산자)
    - [panic과 unwrap이 좋은 경우](#panic과-unwrap이-좋은-경우)
  - [트레이트](#트레이트)
    - [From 트레이트](#from-트레이트)
    - [함수에서 String과 &amp;str 받기](#함수에서-string과-str-받기)
  - [메서드 체이닝](#메서드-체이닝)
  - [반복자](#반복자)
    - [반복자의 작동 방식](#반복자의-작동-방식)
  - [클로저](#클로저)
    - [클로저에서의 |_|](#클로저에서의-_)
    - [클로저와 반복자를 위한 유용한 메서드](#클로저와-반복자를-위한-유용한-메서드)
  - [dbg! 매크로와 .inspect](#dbg-매크로와-inspect)
  - [&amp;str의 타입들](#str의-타입들)
  - [수명](#수명)
  - [내부 가변성](#내부-가변성)
    - [Cell](#cell)
    - [RefCell](#refcell)
    - [Mutex](#mutex)
    - [RwLock](#rwlock)
  - [Cow](#cow)
  - [타입 별칭](#타입-별칭)
    - [함수 내에서 가져오기와 이름 바꾸기](#함수-내에서-가져오기와-이름-바꾸기)
  - [todo! 매크로](#todo-매크로)
  - [Rc](#rc)
  - [다중 스레드](#다중-스레드)
  - [함수 내의 클로저](#함수-내의-클로저)
  - [impl Trait](#impl-trait)
  - [Arc](#arc)
  - [채널](#채널)
  - [Rust 문서 읽기](#rust-문서-읽기)
    - [assert_eq!](#assert_eq)
    - [검색](#검색)
    - [[src] 버튼](#src-버튼)
    - [트레이트에 대한 정보](#트레이트에-대한-정보)
  - [속성](#속성)
  - [Box](#box)
  - [트레이트에 대한 Box](#트레이트에-대한-box)
  - [Default와 빌더 패턴](#default와-빌더-패턴)
  - [Deref와 DerefMut](#deref와-derefmut)
  - [크레이트와 모듈](#크레이트와-모듈)
  - [테스팅](#테스팅)
    - [테스트 주도 개발](#테스트-주도-개발)
  - [외부 크레이트](#외부-크레이트)
    - [rand](#rand)
    - [rayon](#rayon)
    - [serde](#serde)
    - [regex](#regex)
    - [chrono](#chrono)
  - [표준 라이브러리 둘러보기](#표준-라이브러리-둘러보기)
    - [배열](#배열-1)
    - [char](#char)
    - [정수](#정수)
    - [부동소수점](#부동소수점-1)
    - [Bool](#bool)
    - [Vec](#vec)
    - [String](#string)
    - [OsString과 CString](#osstring과-cstring)
    - [Mem](#mem)
    - [Prelude](#prelude)
    - [Time](#time)
    - [기타 매크로](#기타-매크로)
  - [매크로 작성하기](#매크로-작성하기)
- [파트 2 - 컴퓨터에서 Rust 사용하기](#파트-2---컴퓨터에서-rust-사용하기)
  - [Cargo](#cargo)
  - [사용자 입력 받기](#사용자-입력-받기)
  - [파일 사용하기](#파일-사용하기)
  - [Cargo doc](#cargo-doc)
  - [끝?](#끝)

# 파트 1 - 브라우저에서 Rust 사용하기

이 책은 두 부분으로 구성되어 있습니다. 파트 1에서는 브라우저만으로 Rust를 최대한 많이 배울 수 있습니다. 실제로 Rust를 설치하지 않고도 알아야 할 거의 모든 것을 배울 수 있으므로 파트 1은 매우 깁니다. 그리고 마지막에는 파트 2가 있습니다. 이것은 훨씬 짧으며, 컴퓨터에서의 Rust에 관한 내용입니다. 여기서는 브라우저 밖에서만 할 수 있는 나머지 모든 것을 배우게 됩니다. 예를 들어: 파일 작업, 사용자 입력 받기, 그래픽, 개인 설정 등입니다. 희망적으로, 파트 1이 끝날 때쯤에는 Rust를 충분히 좋아해서 설치하게 될 것입니다. 그렇지 않더라도 문제없습니다 - 파트 1은 너무 많은 것을 가르쳐주므로 상관없을 것입니다.

## Rust Playground

**[YouTube에서 이 챕터 보기](https://youtu.be/-lYeJeQ11OI)**

아직 Rust를 설치하고 싶지 않다면 괜찮습니다. [https://play.rust-lang.org/](https://play.rust-lang.org/)로 가서 브라우저를 떠나지 않고 Rust를 작성할 수 있습니다. 거기에 코드를 작성하고 Run을 클릭하여 결과를 볼 수 있습니다. 이 책의 대부분의 샘플을 브라우저의 Playground에서 실행할 수 있습니다. 끝부분에서만 Playground에서 할 수 있는 것을 넘어서는 샘플(파일 열기 등)을 볼 수 있습니다.

Rust Playground 사용 시 팁:

- Run으로 코드를 실행하세요
- 코드를 더 빠르게 하려면 Debug를 Release로 변경하세요. Debug: 더 빠르게 컴파일되고, 더 느리게 실행되며, 디버그 정보를 포함합니다. Release: 더 느리게 컴파일되고, 훨씬 빠르게 실행되며, 디버그 정보를 제거합니다.
- Share를 클릭하여 URL 링크를 얻으세요. 도움을 받고 싶을 때 코드를 공유하는 데 사용할 수 있습니다. 공유를 클릭한 후 `Open a new thread in the Rust user forum`을 클릭하여 바로 거기에 있는 사람들에게 도움을 요청할 수 있습니다.
- Tools: Rustfmt는 코드를 멋지게 포맷합니다.
- Tools: Clippy는 코드를 개선하는 방법에 대한 추가 정보를 제공합니다.
- Config: 여기서 밤에 작업할 수 있도록 테마를 다크 모드로 변경하고, 다른 많은 구성을 할 수 있습니다.

Rust를 설치하려면 [https://www.rust-lang.org/tools/install](https://www.rust-lang.org/tools/install)로 가서 지침을 따르세요. 일반적으로 `rustup`을 사용하여 Rust를 설치하고 업데이트합니다.

## 🚧 와 ⚠️

때때로 책의 코드 예제가 작동하지 않습니다. 예제가 작동하지 않으면 🚧 또는 ⚠️가 있을 것입니다. 🚧는 "공사 중"과 같습니다: 코드가 완전하지 않다는 의미입니다. Rust는 실행하려면 `fn main()` (메인 함수)이 필요하지만, 때때로 우리는 작은 코드 조각만 보고 싶어서 `fn main()`이 없을 것입니다. 그런 예제들은 정확하지만 실행하려면 `fn main()`이 필요합니다. 그리고 일부 코드 예제는 우리가 수정할 문제를 보여줍니다. 그것들은 `fn main()`이 있을 수 있지만 오류를 생성하므로 ⚠️가 있을 것입니다.

## 주석

**[YouTube에서 이 챕터 보기](https://youtu.be/fJ7jBZG_Rpo)**

주석은 컴퓨터가 아닌 프로그래머가 읽기 위해 만들어집니다. 다른 사람들이 코드를 이해하는 데 도움이 되도록 주석을 작성하는 것이 좋습니다. 나중에 자신의 코드를 이해하는 데도 도움이 됩니다. (많은 사람들이 좋은 코드를 작성하지만 왜 작성했는지 잊어버립니다.) Rust에서 주석을 작성하려면 일반적으로 `//`를 사용합니다:

```rust
fn main() {
    // Rust 프로그램은 fn main()으로 시작합니다
    // 코드를 블록 안에 넣습니다. {로 시작하고 }로 끝납니다
    let some_number = 100; // 여기에 원하는 만큼 쓸 수 있고 컴파일러는 보지 않습니다
}
```

이렇게 하면 컴파일러는 `//` 오른쪽의 어떤 것도 보지 않습니다.

`/*`로 시작하고 `*/`로 끝나는 다른 종류의 주석도 있습니다. 이것은 코드 중간에 쓸 때 유용합니다.

```rust
fn main() {
    let some_number/*: i16*/ = 100;
}
```

컴파일러에게 `let some_number/*: i16*/ = 100;`은 `let some_number = 100;`처럼 보입니다.

`/* */` 형태는 여러 줄에 걸친 매우 긴 주석에도 유용합니다. 이 예제에서 모든 줄에 `//`를 써야 하는 것을 볼 수 있습니다. 하지만 `/*`를 입력하면 `*/`로 끝낼 때까지 멈추지 않습니다.

```rust
fn main() {
    let some_number = 100; /* 이 숫자에 대해
    조금 말씀드리겠습니다.
    이것은 100이고, 제가 좋아하는 숫자입니다.
    some_number라고 불리지만 사실 저는... */

    let some_number = 100; // 이 숫자에 대해
    // 조금 말씀드리겠습니다.
    // 이것은 100이고, 제가 좋아하는 숫자입니다.
    // some_number라고 불리지만 사실 저는...
}
```

## 타입

Rust에는 숫자, 문자 등을 작업할 수 있는 많은 타입이 있습니다. 일부는 간단하고, 다른 일부는 더 복잡하며, 자신만의 타입을 만들 수도 있습니다.

### 기본 타입

**[YouTube에서 이 챕터 보기](https://youtu.be/OxTPU5UGMhs)**

Rust에는 **기본 타입**(primitive types)이라고 불리는 간단한 타입들이 있습니다 (primitive = 매우 기본적인). 정수와 `char` (문자)부터 시작하겠습니다. 정수는 소수점이 없는 정수입니다. 정수에는 두 가지 타입이 있습니다:

- 부호 있는 정수 (Signed integers),
- 부호 없는 정수 (Unsigned integers).

부호 있음(Signed)은 `+` (더하기 기호)와 `-` (빼기 기호)를 의미하므로, 부호 있는 정수는 양수(예: +8), 음수(예: -8) 또는 0이 될 수 있습니다. 하지만 부호 없는 정수는 부호가 없기 때문에 양수 또는 0만 될 수 있습니다.

부호 있는 정수: `i8`, `i16`, `i32`, `i64`, `i128`, 그리고 `isize`.
부호 없는 정수: `u8`, `u16`, `u32`, `u64`, `u128`, 그리고 `usize`.

i 또는 u 뒤의 숫자는 해당 숫자의 비트 수를 의미하므로, 더 많은 비트를 가진 숫자는 더 클 수 있습니다. 8비트 = 1바이트이므로, `i8`은 1바이트, `i64`는 8바이트 등입니다. 더 큰 크기의 숫자 타입은 더 큰 숫자를 담을 수 있습니다. 예를 들어, `u8`은 최대 255까지 담을 수 있지만, `u16`은 최대 65535까지 담을 수 있습니다. 그리고 `u128`은 최대 340282366920938463463374607431768211455까지 담을 수 있습니다.

그럼 `isize`와 `usize`는 무엇일까요? 이것은 여러분의 컴퓨터 타입의 비트 수를 의미합니다. (컴퓨터의 비트 수를 컴퓨터의 **아키텍처**라고 부릅니다.) 그래서 32비트 컴퓨터에서 `isize`와 `usize`는 `i32`와 `u32`와 같고, 64비트 컴퓨터에서 `isize`와 `usize`는 `i64`와 `u64`와 같습니다.

다양한 정수 타입이 있는 이유는 여러 가지입니다. 한 가지 이유는 컴퓨터 성능입니다: 더 작은 바이트 수는 처리가 더 빠릅니다. 예를 들어, `i8`로서 숫자 -10은 `11110110`이지만, `i128`로서는 `11111111111111111111111111111111111111111111111111111111111111111111111111111111111111111111111111111111111111111111111111110110`입니다. 하지만 다른 용도들도 있습니다:

Rust의 문자는 `char`라고 불립니다. 모든 `char`는 숫자를 가지고 있습니다: 문자 `A`는 숫자 65이고, 문자 `友` (중국어로 "친구")는 숫자 21451입니다. 숫자 목록은 "유니코드"라고 불립니다. 유니코드는 A부터 Z, 숫자 0부터 9, 또는 공백과 같이 더 많이 사용되는 문자에 더 작은 숫자를 사용합니다.

```rust
fn main() {
    let first_letter = 'A';
    let space = ' '; // ' ' 안의 공백도 char입니다
    let other_language_char = 'Ꮔ'; // 유니코드 덕분에 체로키어 같은 다른 언어도 잘 표시됩니다
    let cat_face = '😺'; // 이모지도 char입니다
}
```

가장 많이 사용되는 문자들은 256보다 작은 숫자를 가지며, `u8`에 들어갈 수 있습니다. 기억하세요, `u8`은 0과 255까지의 모든 숫자로, 총 256개입니다. 이것은 Rust가 `as`를 사용하여 `u8`을 `char`로 안전하게 **캐스트**할 수 있다는 의미입니다. ("`u8`을 `char`로 캐스트"는 "`u8`이 `char`인 것처럼 가장하다"를 의미합니다)

`as`를 사용한 캐스팅은 Rust가 매우 엄격하기 때문에 유용합니다. 항상 타입을 알아야 하며, 둘 다 정수여도 두 개의 다른 타입을 함께 사용할 수 없습니다. 예를 들어, 이것은 작동하지 않습니다:

```rust
fn main() { // main()은 Rust 프로그램이 실행을 시작하는 곳입니다. 코드는 {} (중괄호) 안에 들어갑니다

    let my_number = 100; // 정수 타입을 쓰지 않았으므로,
                         // Rust는 i32를 선택합니다. Rust는 항상
                         // 다른 타입을 사용하라고 말하지 않으면
                         // 정수에 대해 i32를 선택합니다

    println!("{}", my_number as char); // ⚠️
}
```

이유는 다음과 같습니다:

```text
error[E0604]: only `u8` can be cast as `char`, not `i32`
| --> src\main.rs:3:20
 |
3 |     println!("{}", my_number as char);
 |                    ^^^^^^^^^^^^^^^^^
```

다행히 `as`로 쉽게 고칠 수 있습니다. `i32`를 `char`로 캐스트할 수는 없지만, `i32`를 `u8`로 캐스트할 수 있습니다. 그리고 `u8`에서 `char`로 동일하게 할 수 있습니다. 그래서 한 줄에서 `as`를 사용하여 my_number를 `u8`로 만들고, 다시 `char`로 만듭니다. 이제 컴파일됩니다:

```rust
fn main() {
    let my_number = 100;
    println!("{}", my_number as u8 as char);
}
```

100번째 위치의 `char`이기 때문에 `d`를 출력합니다.

하지만 더 쉬운 방법은 Rust에게 `my_number`가 `u8`이라고 말하는 것입니다. 방법은 다음과 같습니다:

```rust
fn main() {
    let my_number: u8 = 100; //  my_number를 my_number: u8로 변경
    println!("{}", my_number as char);
}
```

이것이 Rust의 모든 다양한 숫자 타입에 대한 두 가지 이유입니다. 또 다른 이유가 있습니다: `usize`는 Rust가 *인덱싱*에 사용하는 크기입니다. (인덱싱은 "어떤 항목이 첫 번째인지", "어떤 항목이 두 번째인지" 등을 의미합니다.) `usize`가 인덱싱에 가장 좋은 크기인 이유는:

- 인덱스는 음수가 될 수 없으므로 u가 있는 숫자여야 합니다
- 때때로 많은 것을 인덱싱해야 하므로 커야 하지만
- 32비트 컴퓨터는 u64를 사용할 수 없으므로 u64가 될 수 없습니다.

그래서 Rust는 컴퓨터가 읽을 수 있는 가장 큰 인덱싱 숫자를 얻을 수 있도록 `usize`를 사용합니다.

`char`에 대해 더 배워봅시다. `char`는 항상 하나의 문자이며 `""` 대신 `''`를 사용한다는 것을 보았습니다.

모든 `char`는 4바이트의 메모리를 사용합니다. 4바이트는 모든 종류의 문자를 담기에 충분하기 때문입니다:

- 기본 문자와 기호는 일반적으로 4바이트 중 1바이트만 필요합니다: `a b 1 2 + - = $ @`
- 독일어 움라우트나 악센트 같은 다른 문자는 4바이트 중 2바이트가 필요합니다: `ä ö ü ß è é à ñ`
- 한국어, 일본어 또는 중국어 문자는 3바이트 또는 4바이트가 필요합니다: `国 안 녕`

문자를 문자열의 일부로 사용할 때, 문자열은 각 문자에 필요한 최소한의 메모리를 사용하도록 인코딩됩니다.

`.len()`을 사용하여 직접 확인할 수 있습니다:

```rust
fn main() {
    println!("char의 크기: {}", std::mem::size_of::<char>()); // 4바이트
    println!("'a'를 포함하는 문자열의 크기: {}", "a".len()); // .len()은 문자열의 크기를 바이트로 제공합니다
    println!("'ß'를 포함하는 문자열의 크기: {}", "ß".len());
    println!("'国'를 포함하는 문자열의 크기: {}", "国".len());
    println!("'𓅱'를 포함하는 문자열의 크기: {}", "𓅱".len());
}
```

이것은 다음을 출력합니다:

```text
char의 크기: 4
'a'를 포함하는 문자열의 크기: 1
'ß'를 포함하는 문자열의 크기: 2
'国'를 포함하는 문자열의 크기: 3
'𓅱'를 포함하는 문자열의 크기: 4
```

`a`는 1바이트, 독일어 `ß`는 2바이트, 일본어 `国`는 3바이트, 고대 이집트어 `𓅱`는 4바이트인 것을 볼 수 있습니다.

```rust
fn main() {
    let slice = "Hello!";
    println!("Slice는 {} 바이트입니다.", slice.len());
    let slice2 = "안녕!"; // 한국어로 "안녕"
    println!("Slice2는 {} 바이트입니다.", slice2.len());
}
```

이것은 다음을 출력합니다:

```text
Slice는 6 바이트입니다.
Slice2는 7 바이트입니다.
```

`slice`는 길이가 6문자이고 6바이트이지만, `slice2`는 길이가 3문자이고 7바이트입니다.

`.len()`이 바이트 크기를 제공한다면, 문자 크기는 어떻게 알까요? 이 메서드들에 대해서는 나중에 배우겠지만, `.chars().count()`가 그것을 할 것이라고 기억하면 됩니다. `.chars().count()`는 작성한 것을 문자로 변환한 다음 몇 개인지 센다.

```rust
fn main() {
    let slice = "Hello!";
    println!("Slice는 {} 바이트이고 {} 문자입니다.", slice.len(), slice.chars().count());
    let slice2 = "안녕!";
    println!("Slice2는 {} 바이트이지만 {} 문자뿐입니다.", slice2.len(), slice2.chars().count());
}
```

이것은 다음을 출력합니다:

```text
Slice는 6 바이트이고 6 문자입니다.
Slice2는 7 바이트이지만 3 문자뿐입니다.
```

## 타입 추론

**[YouTube에서 이 챕터 보기](https://youtu.be/q1D2vpy3kEI)**

타입 추론은 컴파일러에게 타입을 말하지 않아도 스스로 결정할 수 있다면 결정한다는 의미입니다. 컴파일러는 항상 변수의 타입을 알아야 하지만, 항상 알려줄 필요는 없습니다. 실제로, 보통은 알려줄 필요가 없습니다. 예를 들어, `let my_number = 8`의 경우 `my_number`는 `i32`가 됩니다. 그것은 컴파일러가 당신이 말하지 않으면 정수에 대해 i32를 선택하기 때문입니다. 하지만 `let my_number: u8 = 8`이라고 말하면, `my_number`를 `u8`로 만들 것입니다. 당신이 `u8`이라고 말했기 때문입니다.

그래서 보통 컴파일러가 추측할 수 있습니다. 하지만 때때로 두 가지 이유로 알려줘야 합니다:

1) 매우 복잡한 작업을 하고 있고 컴파일러가 원하는 타입을 모릅니다.
2) 다른 타입을 원합니다 (예를 들어, `i32`가 아닌 `i128`을 원합니다).

타입을 지정하려면 변수 이름 뒤에 콜론을 추가합니다.

```rust
fn main() {
    let small_number: u8 = 10;
}
```

숫자의 경우, 숫자 뒤에 타입을 말할 수 있습니다. 공백이 필요 없습니다 - 숫자 바로 뒤에 입력하면 됩니다.

```rust
fn main() {
    let small_number = 10u8; // 10u8 = u8 타입의 10
}
```

숫자를 읽기 쉽게 만들고 싶다면 `_`를 추가할 수도 있습니다.

```rust
fn main() {
    let small_number = 10_u8; // 이것이 더 읽기 쉽습니다
    let big_number = 100_000_000_i32; // 1억은 _로 읽기 쉽습니다
}
```

`_`는 숫자를 변경하지 않습니다. 오직 읽기 쉽게 만들기 위한 것입니다. 그리고 몇 개의 `_`를 사용하든 상관없습니다:

```rust
fn main() {
    let number = 0________u8;
    let number2 = 1___6______2____4______i32;
    println!("{}, {}", number, number2);
}
```

이것은 `0, 1624`를 출력합니다.

### 부동소수점

부동소수점은 소수점이 있는 숫자입니다. 5.5는 부동소수점이고, 6은 정수입니다. 5.0도 부동소수점이고, 심지어 5.도 부동소수점입니다.

```rust
fn main() {
    let my_float = 5.; // Rust는 .를 보고 부동소수점임을 압니다
}
```

하지만 타입은 `float`라고 불리지 않고, `f32`와 `f64`라고 불립니다. 정수와 같습니다: `f` 뒤의 숫자는 비트 수를 보여줍니다. 타입을 쓰지 않으면, Rust는 `f64`를 선택합니다.

물론, 같은 타입의 부동소수점만 함께 사용할 수 있습니다. 그래서 `f32`에 `f64`를 더할 수 없습니다.

```rust
fn main() {
    let my_float: f64 = 5.0; // 이것은 f64입니다
    let my_other_float: f32 = 8.5; // 이것은 f32입니다

    let third_float = my_float + my_other_float; // ⚠️
}
```

이것을 실행하려고 하면, Rust는 다음과 같이 말합니다:

```text
error[E0308]: mismatched types
 --> src\main.rs:5:34
  |
5 |     let third_float = my_float + my_other_float;
  |                                  ^^^^^^^^^^^^^^ expected `f64`, found `f32`
```

컴파일러는 잘못된 타입을 사용할 때 "expected (type), found (type)"라고 씁니다. 코드를 이렇게 읽습니다:

```rust
fn main() {
    let my_float: f64 = 5.0; // 컴파일러는 f64를 봅니다
    let my_other_float: f32 = 8.5; // 컴파일러는 f32를 봅니다. 다른 타입입니다.
    let third_float = my_float + // my_float에 무언가를 더하려고 하므로, f64에 다른 f64를 더해야 합니다. 이제 f64를 기대합니다...
    let third_float = my_float + my_other_float;  // ⚠️ 하지만 f32를 발견했습니다. 더할 수 없습니다.
}
```

그래서 "expected (type), found (type)"를 볼 때, 컴파일러가 왜 다른 타입을 기대했는지 찾아야 합니다.

물론, 간단한 숫자로는 고치기 쉽습니다. `as`로 `f32`를 `f64`로 캐스트할 수 있습니다:

```rust
fn main() {
    let my_float: f64 = 5.0;
    let my_other_float: f32 = 8.5;

    let third_float = my_float + my_other_float as f64; // my_other_float as f64 = my_other_float를 f64처럼 사용
}
```

또는 더 간단하게, 타입 선언을 제거하세요. ("타입을 선언하다" = "Rust에게 타입을 사용하라고 말하다") Rust는 함께 더할 수 있는 타입을 선택합니다.

```rust
fn main() {
    let my_float = 5.0; // Rust는 f64를 선택합니다
    let my_other_float = 8.5; // 여기서도 f64를 선택합니다

    let third_float = my_float + my_other_float;
}
```

Rust 컴파일러는 똑똑해서 f32가 필요하면 f64를 선택하지 않습니다:

```rust
fn main() {
    let my_float: f32 = 5.0;
    let my_other_float = 8.5; // 보통 Rust는 f64를 선택하겠지만,

    let third_float = my_float + my_other_float; // 이제 f32에 더해야 한다는 것을 알았습니다. 그래서 my_other_float도 f32로 선택합니다
}
```

## 'hello, world!' 출력하기

**YouTube에서 이 챕터 보기: [비디오 1](https://youtu.be/yYlPHRl2geQ), [비디오 2](https://youtu.be/DTCSfBJJZb8)**

새로운 Rust 프로그램을 시작하면, 항상 이 코드가 있습니다:

```rust
fn main() {
    println!("Hello, world!");
}
```

- `fn`은 함수를 의미합니다,
- `main`은 프로그램을 시작하는 함수입니다,
- `()`는 함수에 시작할 변수를 주지 않았다는 의미입니다.

`{}`는 **코드 블록**이라고 불립니다. 이것은 코드가 사는 공간입니다.

`println!`은 콘솔에 출력하는 **매크로**입니다. **매크로**는 여러분을 위해 코드를 작성하는 함수와 같습니다. 매크로는 뒤에 `!`가 있습니다. 나중에 매크로 만들기에 대해 배울 것입니다. 지금은 `!`가 매크로라는 의미라는 것을 기억하세요.

`;`에 대해 배우기 위해, 다른 함수를 만들 것입니다. 먼저, `main`에서 숫자 8을 출력합니다:

```rust
fn main() {
    println!("Hello, world number {}!", 8);
}
```

`println!`의 `{}`는 "여기에 변수를 넣으세요"를 의미합니다. 이것은 `Hello, world number 8!`을 출력합니다.

더 많이 넣을 수 있습니다, 이전에 했던 것처럼:

```rust
fn main() {
    println!("Hello, worlds number {} and {}!", 8, 9);
}
```

이것은 `Hello, worlds number 8 and 9!`를 출력합니다.

이제 함수를 만들어 봅시다.

```rust
fn number() -> i32 {
    8
}

fn main() {
    println!("Hello, world number {}!", number());
}
```

이것도 `Hello, world number 8!`을 출력합니다. Rust가 `number()`를 볼 때 함수를 봅니다. 이 함수는:

- 아무것도 받지 않습니다 (`()`가 있기 때문에)
- `i32`를 반환합니다. `->` ("스키니 화살표"라고 불림)는 함수가 반환하는 것을 보여줍니다.

함수 안에는 그냥 `8`이 있습니다. `;`가 없기 때문에, 이것이 반환하는 값입니다. `;`가 있다면, 아무것도 반환하지 않을 것입니다 (`()`를 반환할 것입니다). Rust는 `;`가 있으면 컴파일하지 않을 것입니다. 왜냐하면 반환은 `i32`이고 `;`는 `i32`가 아닌 `()`를 반환하기 때문입니다:

```rust
fn main() {
    println!("Hello, world number {}", number());
}

fn number() -> i32 {
    8;  // ⚠️
}
```

```text
5 | fn number() -> i32 {
  |    ------      ^^^ expected `i32`, found `()`
  |    |
  |    implicitly returns `()` as its body has no tail or `return` expression
6 |     8;
  |      - help: consider removing this semicolon
```

이것은 "`number()`가 `i32`를 반환한다고 말했지만, `;`를 추가해서 아무것도 반환하지 않습니다"를 의미합니다. 그래서 컴파일러는 세미콜론을 제거하라고 제안합니다.

`return 8;`이라고 쓸 수도 있지만 Rust에서는 보통 `;`를 제거하여 `반환`하는 것이 정상입니다.

함수에 변수를 주고 싶을 때는 `()` 안에 넣습니다. 이름을 주고 타입을 써야 합니다.

```rust
fn multiply(number_one: i32, number_two: i32) { // 두 개의 i32가 함수에 들어갑니다. 우리는 그것들을 number_one과 number_two라고 부를 것입니다.
    let result = number_one * number_two;
    println!("{} times {} is {}", number_one, number_two, result);
}

fn main() {
    multiply(8, 9); // 숫자를 직접 줄 수 있습니다
    let some_number = 10; // 또는 두 개의 변수를 선언할 수 있습니다
    let some_other_number = 2;
    multiply(some_number, some_other_number); // 그리고 함수에 넣습니다
}
```

`i32`도 반환할 수 있습니다. 끝의 세미콜론만 제거하면 됩니다:

```rust
fn multiply(number_one: i32, number_two: i32) -> i32 {
    let result = number_one * number_two;
    println!("{} times {} is {}", number_one, number_two, result);
    result // 이것이 우리가 반환하는 i32입니다
}

fn main() {
    let multiply_result = multiply(8, 9); // multiply()를 사용하여 출력하고 결과를 multiply_result에 전달했습니다
}
```

### 변수 선언과 코드 블록

`let`을 사용하여 변수를 선언합니다 (변수를 선언한다 = Rust에게 변수를 만들라고 말한다).

```rust
fn main() {
    let my_number = 8;
    println!("Hello, number {}", my_number);
}
```

변수는 코드 블록 `{}` 내에서 시작하고 끝납니다. 이 예제에서 `my_number`는 자체 코드 블록 안에 있기 때문에 `println!`을 호출하기 전에 끝납니다.

```rust
fn main() {
    {
        let my_number = 8; // my_number는 여기서 시작합니다
                           // my_number는 여기서 끝납니다!
    }

    println!("Hello, number {}", my_number); // ⚠️ my_number가 없고
                                             // println!()이 찾을 수 없습니다
}
```

코드 블록을 사용하여 값을 반환할 수 있습니다:

```rust
fn main() {
    let my_number = {
        let second_number = 8;
        second_number + 9 // 세미콜론이 없으므로 코드 블록은 8 + 9를 반환합니다.
                          // 함수처럼 작동합니다
    };

    println!("My number is: {}", my_number);
}
```

블록 내에 세미콜론을 추가하면, `()` (아무것도 없음)를 반환합니다:

```rust
fn main() {
    let my_number = {
        let second_number = 8; // second_number를 선언하고,
        second_number + 9; // second_number에 9를 더합니다
                           // 하지만 반환하지 않았습니다!
                           // second_number는 이제 사라집니다
    };

    println!("My number is: {:?}", my_number); // my_number는 ()입니다
}
```

그런데 왜 `{}`가 아니라 `{:?}`를 썼을까요? 지금 그것에 대해 이야기하겠습니다.

## Display와 debug

**[YouTube에서 이 챕터 보기](https://youtu.be/jd3pC248c0o)**

Rust의 간단한 변수는 `println!` 내에서 `{}`로 출력할 수 있습니다. 하지만 일부 변수는 그럴 수 없고, **디버그 출력**이 필요합니다. 디버그 출력은 프로그래머를 위한 출력입니다. 보통 더 많은 정보를 보여주기 때문입니다. 디버그는 도움이 되는 추가 정보가 있어서 때때로 예쁘게 보이지 않습니다.

`{}`가 아니라 `{:?}`가 필요한지 어떻게 알 수 있을까요? 컴파일러가 알려줍니다. 예를 들어:

```rust
fn main() {
    let doesnt_print = ();
    println!("This will not print: {}", doesnt_print); // ⚠️
}
```

이것을 실행하면, 컴파일러는 다음과 같이 말합니다:

```text
error[E0277]: `()` doesn't implement `std::fmt::Display`
 --> src\main.rs:3:41
  |
3 |     println!("This will not print: {}", doesnt_print);
  |                                         ^^^^^^^^^^^^ `()` cannot be formatted with the default formatter
  |
  = help: the trait `std::fmt::Display` is not implemented for `()`
  = note: in format strings you may be able to use `{:?}` (or {:#?} for pretty-print) instead
  = note: required by `std::fmt::Display::fmt`
  = note: this error originates in a macro (in Nightly builds, run with -Z macro-backtrace for more info)
```

이것은 많은 정보입니다. 하지만 중요한 부분은: `you may be able to use {:?} (or {:#?} for pretty-print) instead`입니다. 이것은 `{:?}`를 시도할 수 있고, `{:#?}`도 시도할 수 있다는 의미입니다. `{:#?}`는 "예쁜 출력"이라고 불립니다. `{:?}`와 같지만 더 많은 줄에 걸쳐 다른 형식으로 출력합니다.

그래서 Display는 `{}`로 출력하는 것을 의미하고, Debug는 `{:?}`로 출력하는 것을 의미합니다.

한 가지 더: 새 줄을 원하지 않으면 `ln` 없이 `print!`를 사용할 수도 있습니다.

```rust
fn main() {
    print!("This will not print a new line");
    println!(" so this will be on the same line");
}
```

이것은 `This will not print a new line so this will be on the same line`을 출력합니다.

### 가장 작은 수와 가장 큰 수

가장 작은 수와 가장 큰 수를 보고 싶다면, 타입 이름 뒤에 MIN과 MAX를 사용할 수 있습니다:

```rust
fn main() {
    println!("가장 작은 i8은 {}이고 가장 큰 i8은 {}입니다.", i8::MIN, i8::MAX); // 힌트: std::i8::MIN을 출력한다는 것은 "표준 라이브러리의 i8 섹션 내의 MIN을 출력하라"는 의미입니다
    println!("가장 작은 u8은 {}이고 가장 큰 u8은 {}입니다.", u8::MIN, u8::MAX);
    println!("가장 작은 i16은 {}이고 가장 큰 i16은 {}입니다.", i16::MIN, i16::MAX);
    println!("가장 작은 u16은 {}이고 가장 큰 u16은 {}입니다.", u16::MIN, u16::MAX);
    println!("가장 작은 i32는 {}이고 가장 큰 i32는 {}입니다.", i32::MIN, i32::MAX);
    println!("가장 작은 u32는 {}이고 가장 큰 u32는 {}입니다.", u32::MIN, u32::MAX);
    println!("가장 작은 i64는 {}이고 가장 큰 i64는 {}입니다.", i64::MIN, i64::MAX);
    println!("가장 작은 u64는 {}이고 가장 큰 u64는 {}입니다.", u64::MIN, u64::MAX);
    println!("가장 작은 i128은 {}이고 가장 큰 i128은 {}입니다.", i128::MIN, i128::MAX);
    println!("가장 작은 u128은 {}이고 가장 큰 u128은 {}입니다.", u128::MIN, u128::MAX);
}
```

이것은 다음을 출력합니다:

```text
가장 작은 i8은 -128이고 가장 큰 i8은 127입니다.
가장 작은 u8은 0이고 가장 큰 u8은 255입니다.
가장 작은 i16은 -32768이고 가장 큰 i16은 32767입니다.
가장 작은 u16은 0이고 가장 큰 u16은 65535입니다.
가장 작은 i32는 -2147483648이고 가장 큰 i32는 2147483647입니다.
가장 작은 u32는 0이고 가장 큰 u32는 4294967295입니다.
가장 작은 i64는 -9223372036854775808이고 가장 큰 i64는 9223372036854775807입니다.
가장 작은 u64는 0이고 가장 큰 u64는 18446744073709551615입니다.
가장 작은 i128은 -170141183460469231731687303715884105728이고 가장 큰 i128은 170141183460469231731687303715884105727입니다.
가장 작은 u128은 0이고 가장 큰 u128은 340282366920938463463374607431768211455입니다.
```

## 가변성 (변경)

**[YouTube에서 이 챕터 보기](https://youtu.be/Nyyd6qn7dZY)**

`let`으로 변수를 선언하면, 불변(변경할 수 없음)입니다.

이것은 작동하지 않습니다:

```rust
fn main() {
    let my_number = 8;
    my_number = 10; // ⚠️
}
```

컴파일러는 다음과 같이 말합니다: `error[E0384]: cannot assign twice to immutable variable my_number`. 이것은 `let`만 쓰면 변수가 불변이기 때문입니다.

하지만 때때로 변수를 변경하고 싶을 수 있습니다. 변경할 수 있는 변수를 만들려면, `let` 뒤에 `mut`를 추가합니다:

```rust
fn main() {
    let mut my_number = 8;
    my_number = 10;
}
```

이제 문제가 없습니다.

하지만 타입은 변경할 수 없습니다: `mut`도 그것을 할 수 없습니다. 이것은 작동하지 않습니다:

```rust
fn main() {
    let mut my_variable = 8; // 이제 i32입니다. 그것은 변경할 수 없습니다
    my_variable = "Hello, world!"; // ⚠️
}
```

컴파일러에서 같은 "expected" 메시지를 볼 수 있습니다: `expected integer, found &str`. `&str`은 곧 배울 문자열 타입입니다.

### 섀도잉

**[YouTube에서 이 챕터 보기](https://youtu.be/InULHyRGw7g)**

섀도잉은 다른 변수와 같은 이름으로 새 변수를 선언하기 위해 `let`을 사용하는 것을 의미합니다. 가변성처럼 보이지만 완전히 다릅니다. 섀도잉은 이렇게 보입니다:

```rust
fn main() {
    let my_number = 8; // 이것은 i32입니다
    println!("{}", my_number); // 8을 출력합니다
    let my_number = 9.2; // 이것은 같은 이름의 f64입니다. 하지만 첫 번째 my_number가 아닙니다 - 완전히 다릅니다!
    println!("{}", my_number) // 9.2를 출력합니다
}
```

여기서 우리는 `my_number`를 새로운 "let 바인딩"으로 "섀도잉했다"고 말합니다.

그럼 첫 번째 `my_number`는 파괴되었나요? 아니요, 하지만 `my_number`를 호출하면 이제 `f64`인 `my_number`를 얻습니다. 그리고 같은 스코프 블록(같은 `{}`)에 있기 때문에, 첫 번째 `my_number`를 더 이상 볼 수 없습니다.

하지만 다른 블록에 있다면, 둘 다 볼 수 있습니다. 예를 들어:

```rust
fn main() {
    let my_number = 8; // 이것은 i32입니다
    println!("{}", my_number); // 8을 출력합니다
    {
        let my_number = 9.2; // 이것은 f64입니다. my_number가 아닙니다 - 완전히 다릅니다!
        println!("{}", my_number) // 9.2를 출력합니다
                                  // 하지만 섀도잉된 my_number는 여기까지만 살아있습니다.
                                  // 첫 번째 my_number는 여전히 살아있습니다!
    }
    println!("{}", my_number); // 8을 출력합니다
}
```

그래서 변수를 섀도잉할 때, 파괴하지 않습니다. **차단**합니다.

그럼 섀도잉의 장점은 무엇일까요? 섀도잉은 변수를 많이 변경해야 할 때 좋습니다. 변수로 많은 간단한 수학을 하고 싶다고 상상해보세요:

```rust
fn times_two(number: i32) -> i32 {
    number * 2
}

fn main() {
    let final_number = {
        let y = 10;
        let x = 9; // x는 9에서 시작합니다
        let x = times_two(x); // 새로운 x로 섀도우: 18
        let x = x + y; // 새로운 x로 섀도우: 28
        x // x를 반환: final_number는 이제 x의 값입니다
    };
    println!("The number is now: {}", final_number)
}
```

섀도잉이 없다면 x에 신경 쓰지 않더라도 다른 이름을 생각해야 합니다:

```rust
fn times_two(number: i32) -> i32 {
    number * 2
}

fn main() {
    // 섀도잉 없이 Rust를 사용한다고 가정합니다
    let final_number = {
        let y = 10;
        let x = 9; // x는 9에서 시작합니다
        let x_twice = times_two(x); // x의 두 번째 이름
        let x_twice_and_y = x_twice + y; // x의 세 번째 이름!
        x_twice_and_y // 섀도잉이 없어서 아쉽습니다 - 그냥 x를 사용할 수 있었을 텐데
    };
    println!("The number is now: {}", final_number)
}
```

일반적으로 Rust에서 이런 경우에 섀도잉을 봅니다. 변수를 빠르게 가져와서 무언가를 하고 다시 다른 작업을 하고 싶을 때 발생합니다. 그리고 보통 너무 신경 쓰지 않는 빠른 변수에 사용합니다.

## 스택, 힙, 그리고 포인터

스택, 힙, 그리고 포인터는 Rust에서 매우 중요합니다.

스택과 힙은 컴퓨터에서 메모리를 보관하는 두 곳입니다. 중요한 차이점은:

- 스택은 매우 빠르지만, 힙은 그렇게 빠르지 않습니다. 매우 느리지도 않지만, 스택은 항상 더 빠릅니다. 하지만 항상 스택을 사용할 수는 없습니다, 왜냐하면:
- Rust는 컴파일 시간에 변수의 크기를 알아야 합니다. 그래서 `i32` 같은 간단한 변수는 스택에 들어갑니다. 정확한 크기를 알기 때문입니다. `i32`는 항상 4바이트가 될 것이라는 것을 항상 압니다. 32비트 = 4바이트이기 때문입니다. 그래서 `i32`는 항상 스택에 갈 수 있습니다.
- 하지만 일부 타입은 컴파일 시간에 크기를 모릅니다. 하지만 스택은 정확한 크기를 알아야 합니다. 그래서 어떻게 하나요? 먼저 데이터를 힙에 넣습니다. 힙은 어떤 크기의 데이터도 가질 수 있기 때문입니다. 그리고 그것을 찾기 위해 포인터가 스택에 들어갑니다. 포인터의 크기는 항상 알기 때문에 괜찮습니다. 그래서 컴퓨터는 먼저 스택으로 가서 포인터를 읽고, 데이터가 있는 힙으로 따라갑니다.

포인터는 복잡하게 들리지만 쉽습니다. 포인터는 책의 목차와 같습니다. 이 책을 상상해보세요:

```text
나의 책

목차

챕터                         페이지
챕터 1: 나의 삶               1
챕터 2: 나의 고양이           15
챕터 3: 나의 직업             23
챕터 4: 나의 가족             30
챕터 5: 미래 계획             43
```

그래서 이것은 다섯 개의 포인터와 같습니다. 그것들을 읽고 그들이 말하는 정보를 찾을 수 있습니다. "나의 삶" 챕터는 어디에 있나요? 1페이지에 있습니다 (1페이지를 *가리킵니다*). "나의 직업" 챕터는 어디에 있나요? 23페이지에 있습니다.

Rust에서 보통 보는 포인터는 **참조**라고 불립니다. 알아야 할 중요한 부분은: 참조는 다른 값의 메모리를 가리킵니다. 참조는 값을 *빌린다*는 의미지만, 소유하지는 않습니다. 우리 책과 같습니다: 목차는 정보를 소유하지 않습니다. 정보를 소유하는 것은 챕터들입니다. Rust에서 참조는 앞에 `&`가 있습니다. 그래서:

- `let my_variable = 8`은 일반 변수를 만들지만
- `let my_reference = &my_variable`은 참조를 만듭니다.

`my_reference = &my_variable`은 이렇게 읽습니다: "my_reference는 my_variable에 대한 참조입니다". 또는: "my_reference는 my_variable을 참조합니다".

이것은 `my_reference`가 `my_variable`의 데이터를 보기만 한다는 의미입니다. `my_variable`은 여전히 자신의 데이터를 소유합니다.

참조의 참조, 또는 임의의 수의 참조를 가질 수도 있습니다.

```rust
fn main() {
    let my_number = 15; // 이것은 i32입니다
    let single_reference = &my_number; //  이것은 &i32입니다
    let double_reference = &single_reference; // 이것은 &&i32입니다
    let five_references = &&&&&my_number; // 이것은 &&&&&i32입니다
}
```

이것들은 모두 다른 타입입니다, "친구의 친구"가 "친구"와 다른 것처럼.

## 출력에 대한 추가 정보

Rust에서는 거의 원하는 모든 방식으로 출력할 수 있습니다. 출력에 대해 알아야 할 몇 가지 더 있습니다.

`\n`을 추가하면 새 줄을 만들고, `\t`는 탭을 만듭니다:

```rust
fn main() {
    // 주의: 이것은 println!이 아니라 print!입니다
    print!("\t 탭으로 시작\n그리고 새 줄로 이동");
}
```

이것은 다음을 출력합니다:

```text
         탭으로 시작
그리고 새 줄로 이동
```

`""` 안에서는 문제없이 여러 줄에 걸쳐 쓸 수 있지만, 간격에 주의하세요:

```rust
fn main() {
    // 주의: 첫 번째 줄 다음에는 맨 왼쪽에서 시작해야 합니다.
    // println! 바로 아래에 쓰면 공백이 추가됩니다
    println!("따옴표 안에서는
여러 줄에 걸쳐
쓸 수 있고
잘 출력됩니다.");

    println!("왼쪽에서 쓰는 것을
    잊어버리면, 공백이
    출력할 때 추가됩니다.");
}
```

이것은 다음을 출력합니다:

```text
따옴표 안에서는
여러 줄에 걸쳐
쓸 수 있고
잘 출력됩니다.
왼쪽에서 쓰는 것을
    잊어버리면, 공백이
    출력할 때 추가됩니다.
```

`\n` 같은 문자("이스케이프 문자"라고 불림)를 출력하고 싶다면, 추가 `\`를 추가할 수 있습니다:

```rust
fn main() {
    println!("여기 두 개의 이스케이프 문자가 있습니다: \\n 과 \\t");
}
```

이것은 다음을 출력합니다:

```text
여기 두 개의 이스케이프 문자가 있습니다: \n 과 \t
```

때때로 너무 많은 `"`와 이스케이프 문자가 있어서, Rust가 모든 것을 무시하게 하고 싶을 수 있습니다. 이렇게 하려면 시작 부분에 `r#`를 추가하고 끝에 `#`를 추가할 수 있습니다.

```rust
fn main() {
    println!("He said, \"You can find the file at c:\\files\\my_documents\\file.txt.\" Then I found the file."); // 여기서 \를 5번 사용했습니다
    println!(r#"He said, "You can find the file at c:\files\my_documents\file.txt." Then I found the file."#)
}
```

이것은 같은 것을 출력하지만, `r#`을 사용하면 사람이 읽기 쉬워집니다.

```text
He said, "You can find the file at c:\files\my_documents\file.txt." Then I found the file.
He said, "You can find the file at c:\files\my_documents\file.txt." Then I found the file.
```

내부에 `#`가 있어 출력해야 한다면, `r##`로 시작하고 `##`로 끝낼 수 있습니다. 그리고 더 필요하다면, 각 측면에 하나씩 더 #를 추가할 수 있습니다.

여기 네 가지 예제가 있습니다:

```rust
fn main() {
    let my_string = "'Ice to see you,' he said."; // 작은따옴표
    let quote_string = r#""Ice to see you," he said."#; // 큰따옴표
    let hashtag_string = r##"The hashtag #IceToSeeYou had become very popular."##; // #가 하나 있으므로 최소 ##가 필요합니다
    let many_hashtags = r####""You don't have to type ### to use a hashtag. You can just use #.""####; // ###가 세 개 있으므로 최소 ####가 필요합니다

    println!("{}\n{}\n{}\n{}\n", my_string, quote_string, hashtag_string, many_hashtags);
}
```

이것은 다음을 출력합니다:

```text
'Ice to see you,' he said.
"Ice to see you," he said.
The hashtag #IceToSeeYou had become very popular.
"You don't have to type ### to use a hashtag. You can just use #."
```

`r#`에는 또 다른 용도가 있습니다: 이것으로 키워드(`let`, `fn` 등과 같은 단어)를 변수 이름으로 사용할 수 있습니다.

```rust
fn main() {
    let r#let = 6; // 변수의 이름은 let입니다
    let mut r#mut = 10; // 이 변수의 이름은 mut입니다
}
```

`r#`이 이 기능을 가진 이유는 이전 버전의 Rust가 현재 Rust보다 적은 키워드를 가지고 있었기 때문입니다. 그래서 `r#`으로 이전에는 키워드가 아니었던 변수 이름으로 실수를 피할 수 있습니다.

또는 어떤 이유로 함수가 `return`과 같은 이름을 가져야 한다면. 그럼 이렇게 쓸 수 있습니다:

```rust
fn r#return() -> u8 {
    println!("여기 당신의 숫자가 있습니다.");
    8
}

fn main() {
    let my_number = r#return();
    println!("{}", my_number);
}
```

이것은 다음을 출력합니다:

```text
여기 당신의 숫자가 있습니다.
8
```

그래서 아마 필요하지 않겠지만, 변수에 키워드를 정말로 사용해야 한다면 `r#`를 사용할 수 있습니다.

`&str`이나 `char`의 바이트를 출력하고 싶다면, 문자열 앞에 `b`만 쓰면 됩니다. 이것은 모든 ASCII 문자에 작동합니다. 이것들이 모든 ASCII 문자입니다:

```text
☺☻♥♦♣♠♫☼►◄↕‼¶§▬↨↑↓→∟↔▲▼123456789:;<=>?@ABCDEFGHIJKLMNOPQRSTUVWXYZ[\]^_`abcdefghijklmnopqrstuvwxyz{|}~
```

그래서 이것을 출력할 때:

```rust
fn main() {
    println!("{:?}", b"This will look like numbers");
}
```

결과는 다음과 같습니다:

```text
[84, 104, 105, 115, 32, 119, 105, 108, 108, 32, 108, 111, 111, 107, 32, 108, 105, 107, 101, 32, 110, 117, 109, 98, 101, 114, 115]
```

`char`의 경우 이것을 *바이트*라고 하고, `&str`의 경우 *바이트 문자열*이라고 합니다.

필요하다면 `b`와 `r`을 함께 넣을 수도 있습니다:

```rust
fn main() {
    println!("{:?}", br##"I like to write "#"."##);
}
```

그것은 `[73, 32, 108, 105, 107, 101, 32, 116, 111, 32, 119, 114, 105, 116, 101, 32, 34, 35, 34, 46]`을 출력할 것입니다.

문자열 내에서 모든 유니코드 문자를 출력할 수 있는 유니코드 이스케이프도 있습니다: `\u{}`. 16진수 숫자가 `{}` 안에 들어가서 출력됩니다. 유니코드 번호를 얻는 방법과 다시 출력하는 방법의 짧은 예제입니다.

```rust
fn main() {
    println!("{:X}", '행' as u32); // char를 u32로 캐스트하여 16진수 값을 얻습니다
    println!("{:X}", 'H' as u32);
    println!("{:X}", '居' as u32);
    println!("{:X}", 'い' as u32);

    println!("\u{D589}, \u{48}, \u{5C45}, \u{3044}"); // 유니코드 이스케이프 \u로 출력해 봅니다
}
```

우리는 `println!`이 `{}`(Display용)와 `{:?}`(Debug용), 그리고 예쁜 출력을 위한 `{:#?}`로 출력할 수 있다는 것을 압니다. 하지만 다른 많은 출력 방법이 있습니다.

예를 들어, 참조가 있다면 `{:p}`를 사용하여 *포인터 주소*를 출력할 수 있습니다. 포인터 주소는 컴퓨터 메모리의 위치를 의미합니다.

```rust
fn main() {
    let number = 9;
    let number_ref = &number;
    println!("{:p}", number_ref);
}
```

이것은 `0xe2bc0ffcfc` 또는 다른 주소를 출력합니다. 컴퓨터가 저장하는 위치에 따라 매번 다를 수 있습니다.

또는 이진수, 16진수, 8진수를 출력할 수 있습니다:

```rust
fn main() {
    let number = 555;
    println!("이진수: {:b}, 16진수: {:x}, 8진수: {:o}", number, number, number);
}
```

이것은 `이진수: 1000101011, 16진수: 22b, 8진수: 1053`을 출력합니다.

또는 순서를 변경하기 위해 숫자를 추가할 수 있습니다. 첫 번째 변수는 인덱스 0에, 다음은 인덱스 1에, 그리고 계속됩니다.

```rust
fn main() {
    let father_name = "Vlad";
    let son_name = "Adrian Fahrenheit";
    let family_name = "Țepeș";
    println!("이것은 {1} {2}, {0} {2}의 아들입니다.", father_name, son_name, family_name);
}
```

`father_name`은 위치 0에, `son_name`은 위치 1에, `family_name`은 위치 2에 있습니다. 그래서 `이것은 Adrian Fahrenheit Țepeș, Vlad Țepeș의 아들입니다`를 출력합니다.

아마도 `{}` 중괄호 안에 너무 많은 변수가 있는 매우 복잡한 문자열을 출력해야 할 수도 있습니다. 또는 변수를 한 번 이상 출력해야 할 수도 있습니다. 그럼 `{}`에 이름을 추가하는 것이 도움이 될 수 있습니다:

```rust
fn main() {
    println!(
        "{city1}은 {country}에 있고 {city2}도 {country}에 있지만,
{city3}는 {country}에 없습니다.",
        city1 = "서울",
        city2 = "부산",
        city3 = "도쿄",
        country = "한국"
    );
}
```

그것은 다음을 출력합니다:

```text
서울은 한국에 있고 부산도 한국에 있지만,
도쿄는 한국에 없습니다.
```

원한다면 Rust에서 매우 복잡한 출력도 가능합니다. 방법은 다음과 같습니다:

{variable:padding alignment minimum.maximum}

이것을 이해하려면 다음을 보세요:

1) 변수 이름을 원하나요? 위에서 {country}를 쓴 것처럼 먼저 그것을 쓰세요.
   (더 많은 작업을 하려면 그 뒤에 `:`를 추가하세요)
2) 패딩 문자를 원하나요? 예를 들어, 세 개의 "패딩 제로"가 있는 55는 00055처럼 보입니다.
3) 패딩의 정렬(왼쪽 / 중간 / 오른쪽)은?
4) 최소 길이를 원하나요? (숫자만 쓰세요)
5) 최대 길이를 원하나요? (앞에 `.`가 있는 숫자를 쓰세요)

예를 들어, 왼쪽에 5개의 ㅎ 문자와 오른쪽에 5개의 ㅎ 문자로 "a"를 쓰고 싶다면:

```rust
fn main() {
    let letter = "a";
    println!("{:ㅎ^11}", letter);
}
```

이것은 `ㅎㅎㅎㅎㅎaㅎㅎㅎㅎㅎ`를 출력합니다. 컴파일러가 이것을 어떻게 읽는지 이해하기 위해 1)부터 5)까지 살펴봅시다.

- 변수 이름을 원하나요? `{:ㅎ^11}` 변수 이름이 없습니다. `:` 앞에 아무것도 없습니다.
- 패딩 문자를 원하나요? `{:ㅎ^11}` 예. ㅎ가 `:` 뒤에 오고 `^`가 있습니다. `<`는 왼쪽의 문자로 패딩을 의미하고, `>`는 오른쪽을, `^`는 중간을 의미합니다.
- 최소 길이를 원하나요? `{:ㅎ^11}` 예: 뒤에 11이 있습니다.
- 최대 길이를 원하나요? `{:ㅎ^11}` 아니요: `.` 앞에 숫자가 없습니다.

다음은 많은 종류의 포맷팅 예제입니다.

```rust
fn main() {
    let title = "TODAY'S NEWS";
    println!("{:-^30}", title); // 변수 이름 없음, -로 패딩, 중앙에 배치, 30자 길이
    let bar = "|";
    println!("{: <15}{: >15}", bar, bar); // 변수 이름 없음, 공백으로 패딩, 각각 15자, 하나는 왼쪽, 하나는 오른쪽
    let a = "SEOUL";
    let b = "TOKYO";
    println!("{city1:-<15}{city2:->15}", city1 = a, city2 = b); // city1과 city2라는 변수 이름, -로 패딩, 하나는 왼쪽, 하나는 오른쪽
}
```

이것은 다음을 출력합니다:

```text
---------TODAY'S NEWS---------
|                            |
SEOUL--------------------TOKYO
```

## 문자열

**[YouTube에서 이 챕터 보기](https://youtu.be/pSyaGzGg26o)**

Rust에는 두 가지 주요 문자열 타입이 있습니다: `String`과 `&str`. 차이점은 무엇일까요?

- `&str`은 간단한 문자열입니다. `let my_variable = "Hello, world!"`라고 쓸 때, `&str`을 만듭니다. `&str`은 매우 빠릅니다.
- `String`은 더 복잡한 문자열입니다. 약간 느리지만 더 많은 기능이 있습니다. `String`은 힙에 데이터가 있는 포인터입니다.

또한 `&str` 앞에 `&`가 있다는 점에 주목하세요. `str`을 사용하려면 참조가 필요하기 때문입니다. 위에서 본 이유 때문입니다: 스택은 크기를 알아야 합니다. 그래서 크기를 아는 `&`를 주면 만족합니다. 또한 `&`를 사용하여 `str`과 상호작용하기 때문에 소유하지 않습니다. 하지만 `String`은 *소유된* 타입입니다. 왜 이것이 중요한지 곧 배울 것입니다.

`&str`과 `String` 모두 UTF-8입니다. 예를 들어, 이렇게 쓸 수 있습니다:

```rust
fn main() {
    let name = "서태지"; // 이것은 한국 이름입니다. &str이 UTF-8이므로 문제없습니다.
    let other_name = String::from("Adrian Fahrenheit Țepeș"); // Ț와 ș는 UTF-8에서 문제없습니다.
}
```

`String::from("Adrian Fahrenheit Țepeș")`에서 `&str`에서 `String`을 만드는 것이 쉽다는 것을 볼 수 있습니다. 두 타입은 다르지만 매우 밀접하게 연결되어 있습니다.

UTF-8 덕분에 이모지도 쓸 수 있습니다.

```rust
fn main() {
    let name = "😂";
    println!("My name is actually {}", name);
}
```

컴퓨터에서는 `My name is actually 😂`를 출력하지만, 명령줄이 출력할 수 없다면 `My name is actually �`를 표시합니다. 하지만 Rust는 이모지나 다른 유니코드에 문제가 없습니다.

`str`에 `&`를 사용하는 이유를 다시 살펴봅시다.

- `str`은 동적 크기 타입입니다 (동적 크기 = 크기가 다를 수 있음). 예를 들어, "서태지"와 "Adrian Fahrenheit Țepeș"라는 이름은 같은 크기가 아닙니다:

```rust
fn main() {
    println!("String은 항상 {:?} 바이트입니다. Sized입니다.", std::mem::size_of::<String>()); // std::mem::size_of::<Type>()은 타입의 크기를 바이트로 제공합니다
    println!("그리고 i8은 항상 {:?} 바이트입니다. Sized입니다.", std::mem::size_of::<i8>());
    println!("그리고 f64는 항상 {:?} 바이트입니다. Sized입니다.", std::mem::size_of::<f64>());
    println!("하지만 &str? 무엇이든 될 수 있습니다. '서태지'는 {:?} 바이트입니다. Sized가 아닙니다.", std::mem::size_of_val("서태지")); // std::mem::size_of_val()은 변수의 크기를 바이트로 제공합니다
    println!("그리고 'Adrian Fahrenheit Țepeș'는 {:?} 바이트입니다. Sized가 아닙니다.", std::mem::size_of_val("Adrian Fahrenheit Țepeș"));
}
```

이것은 다음을 출력합니다:

```text
String은 항상 24 바이트입니다. Sized입니다.
그리고 i8은 항상 1 바이트입니다. Sized입니다.
그리고 f64는 항상 8 바이트입니다. Sized입니다.
하지만 &str? 무엇이든 될 수 있습니다. '서태지'는 9 바이트입니다. Sized가 아닙니다.
그리고 'Adrian Fahrenheit Țepeș'는 25 바이트입니다. Sized가 아닙니다.
```

그래서 &가 필요합니다. `&`는 포인터를 만들고, Rust는 포인터의 크기를 알기 때문입니다. 그래서 포인터는 스택에 들어갑니다. `str`을 쓰면 Rust는 크기를 모르기 때문에 무엇을 해야 할지 모릅니다.

`String`을 만드는 방법은 많습니다. 몇 가지 예:

- `String::from("This is the string text");` 이것은 텍스트를 받아 String을 만드는 String의 메서드입니다.
- `"This is the string text".to_string()`. 이것은 &str을 String으로 만드는 &str의 메서드입니다.
- `format!` 매크로. 이것은 `println!`과 같지만 출력 대신 String을 만듭니다. 그래서 이렇게 할 수 있습니다:

```rust
fn main() {
    let my_name = "Billybrobby";
    let my_country = "USA";
    let my_home = "Korea";

    let together = format!(
        "I am {} and I come from {} but I live in {}.",
        my_name, my_country, my_home
    );
}
```

이제 *together*라는 String이 있지만 아직 출력하지 않았습니다.

String을 만드는 또 다른 방법은 `.into()`라고 하지만 `.into()`는 단지 `String`을 만들기 위한 것이 아니므로 약간 다릅니다. 일부 타입은 `From`과 `.into()`를 사용하여 다른 타입으로 쉽게 변환할 수 있습니다. 그리고 `From`이 있으면 `.into()`도 있습니다. `From`이 더 명확합니다. 이미 타입을 알고 있기 때문입니다: `String::from("Some str")`이 `&str`에서 `String`임을 알고 있습니다. 하지만 `.into()`를 사용하면 때때로 컴파일러가 모릅니다:

```rust
fn main() {
    let my_string = "Try to make this a String".into(); // ⚠️
}
```

Rust는 많은 타입이 `&str`에서 만들어질 수 있기 때문에 원하는 타입을 모릅니다. "저는 &str을 많은 것으로 만들 수 있습니다. 어떤 것을 원하나요?"라고 말합니다.

```text
error[E0282]: type annotations needed
 --> src\main.rs:2:9
  |
2 |     let my_string = "Try to make this a String".into();
  |         ^^^^^^^^^ consider giving `my_string` a type
```

그래서 이렇게 할 수 있습니다:

```rust
fn main() {
    let my_string: String = "Try to make this a String".into();
}
```

그리고 이제 String을 얻습니다.

## const와 static

**[YouTube에서 이 챕터 보기](https://youtu.be/Ky3HqkWUcI0)**

`let`만이 아니라 값을 선언하는 두 가지 다른 방법이 있습니다. 이것들은 `const`와 `static`입니다. 또한 Rust는 타입 추론을 사용하지 않습니다: 타입을 써야 합니다. 이것들은 변경되지 않는 값을 위한 것입니다 (`const`는 상수를 의미합니다). 차이점은:

- `const`는 변경되지 않는 값을 위한 것이며, 사용될 때 이름이 값으로 대체됩니다.
- `static`은 `const`와 유사하지만 고정된 메모리 위치를 가지며 전역 변수처럼 작동할 수 있습니다.

그래서 거의 같습니다. Rust 프로그래머는 거의 항상 `const`를 사용합니다.

모두 대문자로 쓰고, 보통 `main` 밖에 써서 전체 프로그램 동안 살 수 있게 합니다.

두 가지 예: `const NUMBER_OF_MONTHS: u32 = 12;`와 `static SEASONS: [&str; 4] = ["Spring", "Summer", "Fall", "Winter"];`

## 참조에 대한 추가 정보

**[YouTube에서 이 챕터 보기](https://youtu.be/R13sQ8SNoEQ)**

참조는 Rust에서 매우 중요합니다. Rust는 모든 메모리 액세스가 안전하도록 참조를 사용합니다. `&`를 사용하여 참조를 만든다는 것을 알고 있습니다:

```rust
fn main() {
    let country = String::from("Austria");
    let ref_one = &country;
    let ref_two = &country;

    println!("{}", ref_one);
}
```

이것은 `Austria`를 출력합니다.

코드에서 `country`는 `String`입니다. 그런 다음 `country`에 대한 두 개의 참조를 만들었습니다. 그들은 `&String` 타입을 가지며, "String에 대한 참조"라고 말합니다. `country`에 대한 세 개의 참조나 백 개의 참조를 만들 수 있고 문제가 없을 것입니다.

하지만 이것은 문제입니다:

```rust
fn return_str() -> &str {
    let country = String::from("Austria");
    let country_ref = &country;
    country_ref // ⚠️
}

fn main() {
    let country = return_str();
}
```

함수 `return_str()`은 String을 만든 다음 String에 대한 참조를 만듭니다. 그런 다음 참조를 반환하려고 시도합니다. 하지만 String `country`는 함수 내에서만 살고 그다음 죽습니다. 변수가 사라지면 컴퓨터는 메모리를 정리하고 다른 것에 사용합니다. 그래서 함수가 끝난 후 `country_ref`는 이미 사라진 메모리를 참조하고 있으며, 그것은 괜찮지 않습니다. Rust는 여기서 메모리 실수를 하지 못하게 합니다.

이것이 위에서 이야기한 "소유된" 타입에 대한 중요한 부분입니다. `String`을 소유하기 때문에 전달할 수 있습니다. 하지만 `&String`은 그 `String`이 죽으면 죽으므로 "소유권"을 전달하지 않습니다.

## 가변 참조

**[YouTube에서 이 챕터 보기](https://youtu.be/G48z6Rv76vc)**

데이터를 변경하기 위해 참조를 사용하려면 가변 참조를 사용할 수 있습니다. 가변 참조의 경우 `&` 대신 `&mut`를 씁니다.

```rust
fn main() {
    let mut my_number = 8; // 여기에 mut를 쓰는 것을 잊지 마세요!
    let num_ref = &mut my_number;
}
```

그래서 두 타입은 무엇일까요? `my_number`는 `i32`이고, `num_ref`는 `&mut i32`입니다 ("`i32`에 대한 가변 참조"라고 말합니다).

그래서 my_number에 10을 더하는 데 사용해봅시다. 하지만 `num_ref += 10`을 쓸 수 없습니다. `num_ref`는 `i32` 값이 아니라 `&i32`이기 때문입니다. 값은 실제로 `i32` 안에 있습니다. 값이 있는 곳에 도달하려면 `*`를 사용합니다. `*`는 "참조를 원하지 않고, 참조 뒤의 값을 원한다"는 의미입니다. 다시 말해, 하나의 `*`는 `&`의 반대입니다. 또한 하나의 `*`는 하나의 `&`를 지웁니다.

```rust
fn main() {
    let mut my_number = 8;
    let num_ref = &mut my_number;
    *num_ref += 10; // *를 사용하여 i32 값을 변경합니다.
    println!("{}", my_number);

    let second_number = 800;
    let triple_reference = &&&second_number;
    println!("Second_number = triple_reference? {}", second_number == ***triple_reference);
}
```

이것은 다음을 출력합니다:

```text
18
Second_number = triple_reference? true
```

`&`를 사용하는 것을 "참조"라고 하므로, `*`를 사용하는 것을 "**역**참조"라고 합니다.

Rust에는 가변 및 불변 참조에 대한 두 가지 규칙이 있습니다. 매우 중요하지만 의미가 있기 때문에 기억하기 쉽습니다.

- **규칙 1**: 불변 참조만 있다면 원하는 만큼 가질 수 있습니다. 1개도 괜찮고, 3개도 괜찮고, 1000개도 괜찮습니다. 문제없습니다.
- **규칙 2**: 가변 참조가 있다면 하나만 가질 수 있습니다. 또한 불변 참조**와** 가변 참조를 함께 가질 수 없습니다.

이것은 가변 참조가 데이터를 변경할 수 있기 때문입니다. 다른 참조가 읽을 때 데이터를 변경하면 문제가 발생할 수 있습니다.

이해하는 좋은 방법은 파워포인트 프레젠테이션을 생각하는 것입니다.

상황 1은 **단 하나의 가변 참조**에 관한 것입니다.

상황 1: 직원이 파워포인트 프레젠테이션을 작성하고 있습니다. 그는 매니저가 도와주기를 원합니다. 직원은 매니저에게 로그인 정보를 주고 편집을 도와달라고 요청합니다. 이제 매니저는 직원의 프레젠테이션에 대한 "가변 참조"를 가지고 있습니다. 매니저는 원하는 변경을 할 수 있고 나중에 컴퓨터를 돌려줄 수 있습니다. 다른 사람이 프레젠테이션을 보고 있지 않기 때문에 괜찮습니다.

상황 2는 **불변 참조만**에 관한 것입니다.

상황 2: 직원이 100명에게 프레젠테이션을 하고 있습니다. 이제 100명 모두가 직원의 데이터를 볼 수 있습니다. 그들은 모두 직원의 프레젠테이션에 대한 "불변 참조"를 가지고 있습니다. 볼 수는 있지만 아무도 데이터를 변경할 수 없기 때문에 괜찮습니다.

상황 3은 **문제 상황**입니다.

상황 3: 직원이 매니저에게 로그인 정보를 줍니다. 이제 매니저는 "가변 참조"를 가지고 있습니다. 그런 다음 직원은 100명에게 프레젠테이션을 하러 갔지만 매니저는 여전히 로그인할 수 있습니다. 매니저가 로그인하여 무엇이든 할 수 있기 때문에 괜찮지 않습니다. 아마도 매니저가 컴퓨터에 로그인하여 어머니에게 이메일을 쓰기 시작할 것입니다! 이제 100명은 프레젠테이션 대신 매니저가 어머니에게 이메일을 쓰는 것을 봐야 합니다. 그들이 보기를 기대한 것이 아닙니다.

다음은 불변 차용과 함께 가변 차용의 예입니다:

```rust
fn main() {
    let mut number = 10;
    let number_ref = &number;
    let number_change = &mut number;
    *number_change += 10;
    println!("{}", number_ref); // ⚠️
}
```

컴파일러는 문제를 보여주는 유용한 메시지를 출력합니다.

```text
error[E0502]: cannot borrow `number` as mutable because it is also borrowed as immutable
 --> src\main.rs:4:25
  |
3 |     let number_ref = &number;
  |                      ------- immutable borrow occurs here
4 |     let number_change = &mut number;
  |                         ^^^^^^^^^^^ mutable borrow occurs here
5 |     *number_change += 10;
6 |     println!("{}", number_ref);
  |                    ---------- immutable borrow later used here
```

하지만 이 코드는 작동합니다. 왜일까요?

```rust
fn main() {
    let mut number = 10;
    let number_change = &mut number; // 가변 참조를 만듭니다
    *number_change += 10; // 가변 참조를 사용하여 10을 더합니다
    let number_ref = &number; // 불변 참조를 만듭니다
    println!("{}", number_ref); // 불변 참조를 출력합니다
}
```

문제없이 `20`을 출력합니다. 컴파일러가 우리 코드를 이해할 만큼 똑똑하기 때문에 작동합니다. `number_change`를 사용하여 `number`를 변경했지만 다시 사용하지 않았다는 것을 압니다. 그래서 여기에는 문제가 없습니다. 불변 참조와 가변 참조를 함께 사용하지 않습니다.

이전 Rust에서는 이런 종류의 코드가 실제로 오류를 생성했지만, 이제 컴파일러가 더 똑똑해졌습니다. 우리가 입력한 것뿐만 아니라 모든 것을 어떻게 사용하는지 이해할 수 있습니다.

### 다시 섀도잉

섀도잉이 값을 **파괴**하지 않고 **차단**한다고 말한 것을 기억하나요? 이제 참조를 사용하여 이를 볼 수 있습니다.

```rust
fn main() {
    let country = String::from("Austria");
    let country_ref = &country;
    let country = 8;
    println!("{}, {}", country_ref, country);
}
```

이것은 `Austria, 8`을 출력할까요 아니면 `8, 8`을 출력할까요? `Austria, 8`을 출력합니다. 먼저 `country`라는 `String`을 선언합니다. 그런 다음 이 문자열에 대한 참조 `country_ref`를 만듭니다. 그런 다음 `i32`인 8로 country를 섀도잉합니다. 하지만 첫 번째 `country`는 파괴되지 않았으므로 `country_ref`는 여전히 "8"이 아니라 "Austria"라고 말합니다. 작동 방식을 보여주는 주석이 있는 동일한 코드입니다:

```rust
fn main() {
    let country = String::from("Austria"); // 이제 country라는 String이 있습니다
    let country_ref = &country; // country_ref는 이 데이터에 대한 참조입니다. 변경되지 않을 것입니다
    let country = 8; // 이제 i32인 country라는 변수가 있습니다. 하지만 다른 것이나 country_ref와는 관계가 없습니다
    println!("{}, {}", country_ref, country); // country_ref는 여전히 우리가 준 String::from("Austria")의 데이터를 참조합니다.
}
```

## 함수에 참조 전달하기

**YouTube에서 이 챕터 보기: [불변 참조](https://youtu.be/mKWXt9YTavc)와 [가변 참조](https://youtu.be/kJV1wIvAbyk)**

참조는 함수에 매우 유용합니다. Rust의 값에 대한 규칙은: 값은 하나의 소유자만 가질 수 있습니다.

이 코드는 작동하지 않습니다:

```rust
fn print_country(country_name: String) {
    println!("{}", country_name);
}

fn main() {
    let country = String::from("Austria");
    print_country(country); // "Austria"를 출력합니다
    print_country(country); // ⚠️ 재미있었어요, 다시 해봅시다!
}
```

`country`가 파괴되기 때문에 작동하지 않습니다. 방법은 다음과 같습니다:

- 1단계: `country`라는 `String`을 만듭니다. `country`가 소유자입니다.
- 2단계: `country`를 `print_country`에 줍니다. `print_country`는 `->`가 없으므로 아무것도 반환하지 않습니다. `print_country`가 끝난 후, 우리의 `String`은 이제 죽었습니다.
- 3단계: `country`를 `print_country`에 주려고 시도하지만, 이미 했습니다. 더 이상 줄 `country`가 없습니다.

`print_country`가 `String`을 돌려주도록 할 수 있지만, 약간 어색합니다.

```rust
fn print_country(country_name: String) -> String {
    println!("{}", country_name);
    country_name // 여기서 반환합니다
}

fn main() {
    let country = String::from("Austria");
    let country = print_country(country); // 이제 String을 돌려받기 위해 let을 사용해야 합니다
    print_country(country);
}
```

이제 다음을 출력합니다:

```text
Austria
Austria
```

이것을 고치는 훨씬 더 좋은 방법은 `&`를 추가하는 것입니다.

```rust
fn print_country(country_name: &String) {
    println!("{}", country_name);
}

fn main() {
    let country = String::from("Austria");
    print_country(&country); // "Austria"를 출력합니다
    print_country(&country); // 재미있었어요, 다시 해봅시다!
}
```

이제 `print_country()`는 `String`에 대한 참조를 받는 함수입니다: `&String`. 또한 `&country`를 써서 country에 대한 참조를 줍니다. 이것은 "볼 수는 있지만, 내가 가지고 있을게"라고 말합니다.

이제 가변 참조로 비슷한 것을 해봅시다. 다음은 가변 변수를 사용하는 함수의 예입니다.

```rust
fn add_hungary(country_name: &mut String) { // 먼저 함수가 가변 참조를 받는다고 말합니다
    country_name.push_str("-Hungary"); // push_str()은 String에 &str을 추가합니다
    println!("Now it says: {}", country_name);
}

fn main() {
    let mut country = String::from("Austria");
    add_hungary(&mut country); // 가변 참조를 줘야 합니다.
}
```

이것은 `Now it says: Austria-Hungary`를 출력합니다.

정리하면:

- `fn function_name(variable: String)`은 `String`을 받아 소유합니다. 아무것도 반환하지 않으면, 변수는 함수 내에서 죽습니다.
- `fn function_name(variable: &String)`은 `String`을 빌려서 볼 수 있습니다
- `fn function_name(variable: &mut String)`은 `String`을 빌려서 변경할 수 있습니다

가변 참조처럼 보이지만 다른 예제가 있습니다.

```rust
fn main() {
    let country = String::from("Austria"); // country는 가변이 아니지만, Austria-Hungary를 출력할 것입니다. 어떻게?
    adds_hungary(country);
}

fn adds_hungary(mut country: String) { // 방법은 다음과 같습니다: adds_hungary는 String을 받아 가변으로 선언합니다!
    country.push_str("-Hungary");
    println!("{}", country);
}
```

어떻게 가능할까요? `mut country`는 참조가 아니기 때문입니다: `adds_hungary`는 이제 `country`를 소유합니다. (기억하세요, `&String`이 아니라 `String`을 받습니다). `adds_hungary`를 호출하는 순간, 완전한 소유자가 됩니다. `country`는 더 이상 `String::from("Austria")`와 관계가 없습니다. 그래서 `adds_hungary`는 `country`를 가변으로 받을 수 있고, 그렇게 하는 것이 완전히 안전합니다.

위의 직원 파워포인트와 매니저 상황을 기억하나요? 이 상황에서는 직원이 매니저에게 컴퓨터 전체를 주는 것과 같습니다. 직원은 다시는 만지지 않을 것이므로, 매니저는 원하는 것은 무엇이든 할 수 있습니다.

## Copy 타입

Rust의 일부 타입은 매우 간단합니다. 이들을 **copy 타입**이라고 합니다. 이 간단한 타입들은 모두 스택에 있고, 컴파일러는 크기를 압니다. 즉, 복사하기 매우 쉬우므로 함수에 보낼 때 컴파일러는 항상 복사합니다. 너무 작고 쉬워서 복사하지 않을 이유가 없기 때문에 항상 복사합니다. 그래서 이러한 타입에 대해서는 소유권을 걱정할 필요가 없습니다.

이러한 간단한 타입에는 정수, 부동소수점, 불리언 (`true`와 `false`), 그리고 `char`가 포함됩니다.

타입이 copy를 **구현**하는지 어떻게 알 수 있을까요? (구현 = 사용할 수 있음) 문서를 확인할 수 있습니다. 예를 들어, char의 문서는 다음과 같습니다:

[https://doc.rust-lang.org/std/primitive.char.html](https://doc.rust-lang.org/std/primitive.char.html)

왼쪽에서 **Trait Implementations**를 볼 수 있습니다. 예를 들어 **Copy**, **Debug**, **Display**를 볼 수 있습니다. 그래서 `char`가 다음을 알 수 있습니다:

- 함수에 보낼 때 복사됩니다 (**Copy**)
- `{}`를 사용하여 출력할 수 있습니다 (**Display**)
- `{:?}`를 사용하여 출력할 수 있습니다 (**Debug**)

```rust
fn prints_number(number: i32) { // ->가 없으므로 아무것도 반환하지 않습니다
                             // number가 copy 타입이 아니라면, 가져가서
                             // 다시 사용할 수 없을 것입니다
    println!("{}", number);
}

fn main() {
    let my_number = 8;
    prints_number(my_number); // 8을 출력합니다. prints_number는 my_number의 복사본을 받습니다
    prints_number(my_number); // 다시 8을 출력합니다.
                              // 문제없습니다, my_number는 copy 타입이니까요!
}
```

하지만 String의 문서를 보면, copy 타입이 아닙니다.

[https://doc.rust-lang.org/std/string/struct.String.html](https://doc.rust-lang.org/std/string/struct.String.html)

왼쪽의 **Trait Implementations**에서 알파벳 순서로 볼 수 있습니다. A, B, C... C에 **Copy**가 없습니다. 하지만 **Clone**이 있습니다. **Clone**은 **Copy**와 유사하지만 보통 더 많은 메모리가 필요합니다. 또한 `.clone()`으로 호출해야 합니다 - 저절로 복제되지 않습니다.

이 예제에서 `prints_country()`는 국가 이름인 `String`을 출력합니다. 두 번 출력하고 싶지만 할 수 없습니다:

```rust
fn prints_country(country_name: String) {
    println!("{}", country_name);
}

fn main() {
    let country = String::from("Kiribati");
    prints_country(country);
    prints_country(country); // ⚠️
}
```

하지만 이제 메시지를 이해합니다.

```text
error[E0382]: use of moved value: `country`
 --> src\main.rs:4:20
  |
2 |     let country = String::from("Kiribati");
  |         ------- move occurs because `country` has type `std::string::String`, which does not implement the `Copy` trait
3 |     prints_country(country);
  |                    ------- value moved here
4 |     prints_country(country);
  |                    ^^^^^^^ value used here after move
```

중요한 부분은 `which does not implement the Copy trait`입니다. 하지만 문서에서 String이 `Clone` 트레이트를 구현한다는 것을 봤습니다. 그래서 코드에 `.clone()`을 추가할 수 있습니다. 이것은 복제본을 만들고, 복제본을 함수에 보냅니다. 이제 `country`는 여전히 살아있으므로 사용할 수 있습니다.

```rust
fn prints_country(country_name: String) {
    println!("{}", country_name);
}

fn main() {
    let country = String::from("Kiribati");
    prints_country(country.clone()); // 복제본을 만들어 함수에 줍니다. 복제본만 들어가고 country는 여전히 살아있습니다
    prints_country(country);
}
```

물론 `String`이 매우 크면 `.clone()`은 많은 메모리를 사용할 수 있습니다. 하나의 `String`은 책 전체 길이가 될 수 있고, `.clone()`을 호출할 때마다 책을 복사합니다. 그래서 가능하다면 참조를 위해 `&`를 사용하는 것이 더 빠릅니다. 예를 들어, 이 코드는 `String`에 `&str`을 푸시한 다음 함수에서 사용될 때마다 복제본을 만듭니다:

```rust
fn get_length(input: String) { // String의 소유권을 가집니다
    println!("It's {} words long.", input.split_whitespace().count()); // 단어 수를 세기 위해 분할합니다
}

fn main() {
    let mut my_string = String::new();
    for _ in 0..50 {
        my_string.push_str("Here are some more words "); // 단어를 추가합니다
        get_length(my_string.clone()); // 매번 복제본을 줍니다
    }
}
```

다음을 출력합니다:

```text
It's 5 words long.
It's 10 words long.
...
It's 250 words long.
```

50개의 복제본입니다. 대신 참조를 사용하는 것이 더 좋습니다:

```rust
fn get_length(input: &String) {
    println!("It's {} words long.", input.split_whitespace().count());
}

fn main() {
    let mut my_string = String::new();
    for _ in 0..50 {
        my_string.push_str("Here are some more words ");
        get_length(&my_string);
    }
}
```

50개의 복제본 대신 0개입니다.

### 값이 없는 변수

값이 없는 변수는 "초기화되지 않은" 변수라고 합니다. 초기화되지 않음은 "아직 시작하지 않음"을 의미합니다. 간단합니다: `let`과 변수 이름만 쓰면 됩니다:

```rust
fn main() {
    let my_variable; // ⚠️
}
```

하지만 아직 사용할 수 없고, Rust는 초기화되지 않은 것이 있으면 컴파일하지 않습니다.

하지만 때때로 유용할 수 있습니다. 좋은 예는 다음과 같은 경우입니다:

- 코드 블록이 있고 변수의 값이 그 안에 있고,
- 변수가 코드 블록 밖에서 살아야 할 때.

```rust
fn loop_then_return(mut counter: i32) -> i32 {
    loop {
        counter += 1;
        if counter % 50 == 0 {
            break;
        }
    }
    counter
}

fn main() {
    let my_number;

    {
        // 이 코드 블록이 필요하다고 가정합니다
        let number = {
            // 여기에 숫자를 만드는 코드가 있다고 가정합니다
            // 많은 코드, 그리고 마침내:
            57
        };

        my_number = loop_then_return(number);
    }

    println!("{}", my_number);
}
```

이것은 `100`을 출력합니다.

`my_number`가 `main()` 함수에서 선언되었으므로 끝까지 살아있는 것을 볼 수 있습니다. 하지만 루프 내부에서 값을 얻습니다. 그러나 그 값은 `my_number`가 값을 가지고 있기 때문에 `my_number`만큼 오래 삽니다. 그리고 블록 내부에 `let my_number = loop_then_return(number)`라고 썼다면, 바로 죽을 것입니다.

코드를 단순화하면 상상하는 데 도움이 됩니다. `loop_then_return(number)`는 결과 100을 주므로, 삭제하고 대신 `100`을 쓰겠습니다. 또한 이제 `number`가 필요 없으므로 그것도 삭제합니다. 이제 이렇게 보입니다:

```rust
fn main() {
    let my_number;
    {
        my_number = 100;
    }

    println!("{}", my_number);
}
```

그래서 거의 `let my_number = { 100 };`라고 말하는 것과 같습니다.

또한 `my_number`는 `mut`가 아닙니다. 100을 얻을 때까지 값을 얻지 못했으므로 값을 변경한 적이 없습니다. 결국 `my_number`의 실제 코드는 `let my_number = 100;`입니다.

## 컬렉션 타입

Rust에는 컬렉션을 만들기 위한 많은 타입이 있습니다. 컬렉션은 한 곳에 하나 이상의 값이 필요할 때를 위한 것입니다. 예를 들어, 한 변수 안에 당신 나라의 모든 도시에 대한 정보를 가질 수 있습니다. 가장 빠르지만 기능이 가장 적은 배열부터 시작하겠습니다. 그런 면에서 `&str`과 비슷합니다.

### 배열

배열은 대괄호 `[]` 안의 데이터입니다. 배열은:

- 크기를 변경해서는 안 되며,
- 같은 타입만 포함해야 합니다.

하지만 매우 빠릅니다.

배열의 타입은: `[type; number]`입니다. 예를 들어, `["One", "Two"]`의 타입은 `[&str; 2]`입니다. 즉, 이 두 배열도 타입이 다릅니다:

```rust
fn main() {
    let array1 = ["One", "Two"]; // 이것은 [&str; 2] 타입입니다
    let array2 = ["One", "Two", "Five"]; // 하지만 이것은 [&str; 3] 타입입니다. 다른 타입!
}
```

좋은 팁이 있습니다: 변수의 타입을 알려면, 잘못된 명령을 주어 컴파일러에게 "물어볼" 수 있습니다. 예를 들어:

```rust
fn main() {
    let seasons = ["Spring", "Summer", "Autumn", "Winter"];
    let seasons2 = ["Spring", "Summer", "Fall", "Autumn", "Winter"];
    seasons.ddd(); // ⚠️
    seasons2.thd(); // ⚠️ 역시
}
```

컴파일러는 "뭐야? seasons에는 `.ddd()` 메서드가 없고 seasons2에도 `.thd()` 메서드가 없어!"라고 말합니다:

```text
error[E0599]: no method named `ddd` found for array `[&str; 4]` in the current scope
 --> src\main.rs:4:13
  |
4 |     seasons.ddd(); // 
  |             ^^^ method not found in `[&str; 4]`

error[E0599]: no method named `thd` found for array `[&str; 5]` in the current scope
 --> src\main.rs:5:14
  |
5 |     seasons2.thd(); // 
  |              ^^^ method not found in `[&str; 5]`
```

그래서 ``method not found in `[&str; 4]` ``라고 알려주는데, 이것이 타입입니다.

모두 같은 값을 가진 배열을 원한다면, 이렇게 선언할 수 있습니다:

```rust
fn main() {
    let my_array = ["a"; 10];
    println!("{:?}", my_array);
}
```

이것은 `["a", "a", "a", "a", "a", "a", "a", "a", "a", "a"]`를 출력합니다.

이 방법은 버퍼를 만드는 데 많이 사용됩니다. 예를 들어, `let mut buffer = [0; 640]`은 640개의 0으로 이루어진 배열을 만듭니다. 그런 다음 데이터를 추가하기 위해 0을 다른 숫자로 변경할 수 있습니다.

[]로 배열의 항목을 인덱싱(가져오기)할 수 있습니다. 첫 번째 항목은 [0], 두 번째는 [1] 등입니다.

```rust
fn main() {
    let my_numbers = [0, 10, -20];
    println!("{}", my_numbers[1]); // 10을 출력합니다
}
```

배열의 슬라이스(조각)를 얻을 수 있습니다. 먼저 컴파일러가 크기를 모르기 때문에 &가 필요합니다. 그런 다음 `..`를 사용하여 범위를 표시할 수 있습니다.

예를 들어, 이 배열을 사용해 봅시다: `[1, 2, 3, 4, 5, 6, 7, 8, 9, 10]`.

```rust
fn main() {
    let array_of_ten = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10];

    let three_to_five = &array_of_ten[2..5];
    let start_at_two = &array_of_ten[1..];
    let end_at_five = &array_of_ten[..5];
    let everything = &array_of_ten[..];

    println!("Three to five: {:?}, start at two: {:?}, end at five: {:?}, everything: {:?}", three_to_five, start_at_two, end_at_five, everything);
}
```

기억하세요:

- 인덱스 번호는 0부터 시작합니다 (1이 아님)
- 인덱스 범위는 **배타적**입니다 (마지막 숫자를 포함하지 않음)

그래서 `[0..2]`는 첫 번째 인덱스와 두 번째 인덱스(0과 1)를 의미합니다. 또는 "0번째와 첫 번째" 인덱스라고 부를 수 있습니다. 인덱스 2인 세 번째 항목은 없습니다.

마지막 숫자도 포함하는 **포함** 범위를 가질 수도 있습니다. 이렇게 하려면 `..` 대신 `..=`를 쓰기 위해 `=`를 추가합니다. 그래서 `[0..2]` 대신 첫 번째, 두 번째, 세 번째 항목을 원한다면 `[0..=2]`를 쓸 수 있습니다.

## 벡터

**[YouTube에서 이 챕터 보기](https://youtu.be/Eh-DsRnDKmw)**

`&str`과 `String`이 있는 것처럼, 배열과 벡터가 있습니다. 배열은 기능이 적지만 더 빠르고, 벡터는 기능이 많지만 더 느립니다. (물론 Rust는 항상 매우 빠르므로 벡터가 느린 것이 아니라 배열보다 느*린* 것입니다.) 타입은 `Vec`로 쓰고, "벡"이라고 부를 수도 있습니다.

벡터를 선언하는 두 가지 주요 방법이 있습니다. 하나는 `String`처럼 `new`를 사용하는 것입니다:

```rust
fn main() {
    let name1 = String::from("Windy");
    let name2 = String::from("Gomesy");

    let mut my_vec = Vec::new();
    // 지금 프로그램을 실행하면 컴파일러가 오류를 줄 것입니다.
    // vec의 타입을 모릅니다.

    my_vec.push(name1); // 이제 알았습니다: Vec<String>입니다
    my_vec.push(name2);
}
```

`Vec`에는 항상 다른 것이 들어 있고, 그것이 `<>` (꺾쇠 괄호)의 용도입니다. `Vec<String>`은 하나 이상의 `String`이 있는 벡터입니다. 더 많은 타입도 안에 가질 수 있습니다. 예를 들어:

- `Vec<(i32, i32)>` 이것은 각 항목이 튜플인 `Vec`입니다: `(i32, i32)`.
- `Vec<Vec<String>>` 이것은 `String`의 `Vec`들을 가진 `Vec`입니다. 예를 들어 좋아하는 책을 `Vec<String>`으로 저장하고 싶다고 해봅시다. 그런 다음 다른 책으로 다시 하고, 또 다른 `Vec<String>`을 얻습니다. 두 책을 모두 담으려면 다른 `Vec`에 넣고 그것은 `Vec<Vec<String>>`이 됩니다.

Rust가 타입을 결정하도록 `.push()`를 사용하는 대신, 타입을 선언할 수 있습니다.

```rust
fn main() {
    let mut my_vec: Vec<String> = Vec::new(); // 컴파일러가 타입을 알므로
                                              // 오류가 없습니다.
}
```

벡터의 항목들은 같은 타입이어야 함을 볼 수 있습니다.

벡터를 만드는 또 다른 쉬운 방법은 `vec!` 매크로를 사용하는 것입니다. 배열 선언처럼 보이지만 앞에 `vec!`가 있습니다.

```rust
fn main() {
    let mut my_vec = vec![8, 10, 10];
}
```

타입은 `Vec<i32>`입니다. "i32의 Vec"라고 부릅니다. 그리고 `Vec<String>`은 "문자열의 Vec"입니다. 그리고 `Vec<Vec<String>>`은 "문자열의 vec의 Vec"입니다.

배열처럼 벡터도 슬라이스할 수 있습니다.

```rust
fn main() {
    let vec_of_ten = vec![1, 2, 3, 4, 5, 6, 7, 8, 9, 10];
    // vec!를 추가한 것 외에는 위와 모두 같습니다.
    let three_to_five = &vec_of_ten[2..5];
    let start_at_two = &vec_of_ten[1..];
    let end_at_five = &vec_of_ten[..5];
    let everything = &vec_of_ten[..];

    println!("Three to five: {:?},
start at two: {:?}
end at five: {:?}
everything: {:?}", three_to_five, start_at_two, end_at_five, everything);
}
```

vec는 배열보다 느리기 때문에, 더 빠르게 만들기 위한 몇 가지 방법을 사용할 수 있습니다. vec에는 **용량**이 있는데, 이는 벡터에 주어진 공간을 의미합니다. 벡터에 새 항목을 푸시하면 용량에 점점 가까워집니다. 그런 다음 용량을 초과하면 용량을 두 배로 늘리고 항목을 새 공간으로 복사합니다. 이를 재할당이라고 합니다. 벡터에 항목을 추가하면서 용량을 보기 위해 `.capacity()`라는 메서드를 사용할 것입니다.

예를 들어:

```rust
fn main() {
    let mut num_vec = Vec::new();
    println!("{}", num_vec.capacity()); // 0 요소: 0을 출력합니다
    num_vec.push('a'); // 하나의 문자를 추가합니다
    println!("{}", num_vec.capacity()); // 1 요소: 4를 출력합니다. 1개 항목이 있는 Vec는 항상 용량 4로 시작합니다
    num_vec.push('a'); // 하나 더 추가
    num_vec.push('a'); // 하나 더 추가
    num_vec.push('a'); // 하나 더 추가
    println!("{}", num_vec.capacity()); // 4 요소: 여전히 4를 출력합니다.
    num_vec.push('a'); // 하나 더 추가
    println!("{}", num_vec.capacity()); // 8을 출력합니다. 5개의 요소가 있지만 공간을 만들기 위해 4를 8로 두 배로 늘렸습니다
}
```

이것은 다음을 출력합니다:

```text
0
4
4
8
```

그래서 이 벡터는 두 번의 재할당을 가집니다: 0에서 4로, 4에서 8로. 더 빠르게 만들 수 있습니다:

```rust
fn main() {
    let mut num_vec = Vec::with_capacity(8); // 용량 8을 줍니다
    num_vec.push('a'); // 하나의 문자를 추가합니다
    println!("{}", num_vec.capacity()); // 8을 출력합니다
    num_vec.push('a'); // 하나 더 추가
    println!("{}", num_vec.capacity()); // 8을 출력합니다
    num_vec.push('a'); // 하나 더 추가
    println!("{}", num_vec.capacity()); // 8을 출력합니다.
    num_vec.push('a'); // 하나 더 추가
    num_vec.push('a'); // 하나 더 추가 // 이제 5개의 요소가 있습니다
    println!("{}", num_vec.capacity()); // 여전히 8
}
```

이 벡터는 0번의 재할당을 가지며, 이는 더 좋습니다. 그래서 필요한 요소 수를 안다고 생각하면, `Vec::with_capacity()`를 사용하여 더 빠르게 만들 수 있습니다.

`.into()`를 사용하여 `&str`을 `String`으로 만들 수 있다는 것을 기억하세요. 배열을 `Vec`로 만드는 데도 사용할 수 있습니다. `.into()`에게 `Vec`를 원한다고 말해야 하지만, `Vec`의 타입을 선택할 필요는 없습니다. 선택하고 싶지 않다면 `Vec<_>`라고 쓸 수 있습니다.

```rust
fn main() {
    let my_vec: Vec<u8> = [1, 2, 3].into();
    let my_vec2: Vec<_> = [9, 0, 10].into(); // Vec<_>는 "Vec 타입을 나를 위해 선택해"를 의미합니다
                                             // Rust는 Vec<i32>를 선택할 것입니다
}
```

## 튜플

**[YouTube에서 이 챕터 보기](https://youtu.be/U67Diy6SlTg)**

Rust의 튜플은 `()`를 사용합니다. 우리는 이미 많은 빈 튜플을 봤습니다. 왜냐하면 함수에서 *아무것도*는 실제로 빈 튜플을 의미하기 때문입니다:

```text
fn do_something() {}
```

는 실제로 다음의 줄임말입니다:

```text
fn do_something() -> () {}
```

그 함수는 아무것도 받지 않고 (빈 튜플), 아무것도 반환하지 않습니다 (빈 튜플). 그래서 우리는 이미 튜플을 많이 사용하고 있었습니다. 함수에서 아무것도 반환하지 않을 때, 실제로는 빈 튜플을 반환합니다.

```rust
fn just_prints() {
    println!("I am printing"); // ;를 추가하면 빈 튜플을 반환한다는 의미입니다
}

fn main() {}
```

하지만 튜플은 많은 것을 담을 수 있고, 다른 타입도 담을 수 있습니다. 튜플 내부의 항목들도 0, 1, 2 등의 숫자로 인덱싱됩니다. 하지만 액세스하려면 `[]` 대신 `.`를 사용합니다. 단일 튜플에 여러 타입을 넣어봅시다.

```rust
fn main() {
    let random_tuple = ("Here is a name", 8, vec!['a'], 'b', [8, 9, 10], 7.7);
    println!(
        "튜플 안에는: 첫 번째 항목: {:?}
두 번째 항목: {:?}
세 번째 항목: {:?}
네 번째 항목: {:?}
다섯 번째 항목: {:?}
여섯 번째 항목: {:?}",
        random_tuple.0,
        random_tuple.1,
        random_tuple.2,
        random_tuple.3,
        random_tuple.4,
        random_tuple.5,
    )
}
```

이것은 다음을 출력합니다:

```text
튜플 안에는: 첫 번째 항목: "Here is a name"
두 번째 항목: 8
세 번째 항목: ['a']
네 번째 항목: 'b'
다섯 번째 항목: [8, 9, 10]
여섯 번째 항목: 7.7
```

그 튜플의 타입은 `(&str, i32, Vec<char>, char, [i32; 3], f64)`입니다.

튜플을 사용하여 여러 변수를 만들 수 있습니다. 이 코드를 보세요:

```rust
fn main() {
    let str_vec = vec!["one", "two", "three"];
}
```

`str_vec`에는 세 개의 항목이 있습니다. 그것들을 꺼내고 싶다면? 그때 튜플을 사용할 수 있습니다.

```rust
fn main() {
    let str_vec = vec!["one", "two", "three"];

    let (a, b, c) = (str_vec[0], str_vec[1], str_vec[2]); // a, b, c라고 부릅니다
    println!("{:?}", b);
}
```

`"two"`를 출력하는데, 이것이 `b`입니다. 이것을 *구조 분해*라고 부릅니다. 처음에는 변수들이 구조 안에 있었지만, 구조 안에 있지 않은 `a`, `b`, `c`를 만들었기 때문입니다.

구조 분해가 필요하지만 모든 변수를 원하지 않는다면 `_`를 사용할 수 있습니다.

```rust
fn main() {
    let str_vec = vec!["one", "two", "three"];

    let (_, _, variable) = (str_vec[0], str_vec[1], str_vec[2]);
}
```

이제 `variable`이라는 변수만 만들고 다른 것들의 변수는 만들지 않습니다.

더 많은 컬렉션 타입이 있고, 배열, vec, 튜플을 사용하는 더 많은 방법이 있습니다. 그것들에 대해서도 더 배울 것이지만, 먼저 제어 흐름을 배우겠습니다.

## 제어 흐름

**YouTube에서 이 챕터 보기: [파트 1](https://youtu.be/UAymDOpv_us)과 [파트 2](https://youtu.be/eqysTfiiQZs)**

제어 흐름은 다른 상황에서 코드가 무엇을 해야 하는지 알려주는 것을 의미합니다. 가장 간단한 제어 흐름은 `if`입니다.

```rust
fn main() {
    let my_number = 5;
    if my_number == 7 {
        println!("It's seven");
    }
}
```

또한 `=`가 아니라 `==`를 사용한다는 점에 주목하세요. `==`는 비교하는 것이고, `=`는 *할당*하는 것입니다 (값을 주는 것). 또한 `if (my_number == 7)`이 아니라 `if my_number == 7`이라고 썼습니다. Rust에서는 `if`에 괄호가 필요 없습니다.

`else if`와 `else`는 더 많은 제어를 제공합니다:

```rust
fn main() {
    let my_number = 5;
    if my_number == 7 {
        println!("It's seven");
    } else if my_number == 6 {
        println!("It's six")
    } else {
        println!("It's a different number")
    }
}
```

이것은 `It's a different number`를 출력합니다. 7이나 6과 같지 않기 때문입니다.

`&&` (그리고)와 `||` (또는)로 더 많은 조건을 추가할 수 있습니다.

```rust
fn main() {
    let my_number = 5;
    if my_number % 2 == 1 && my_number > 0 { // % 2는 2로 나눈 후 남은 숫자를 의미합니다
        println!("It's a positive odd number");
    } else if my_number == 6 {
        println!("It's six")
    } else {
        println!("It's a different number")
    }
}
```

이것은 `It's a positive odd number`를 출력합니다. 2로 나누면 나머지가 1이고, 0보다 크기 때문입니다.

너무 많은 `if`, `else`, `else if`는 읽기 어려울 수 있습니다. 이 경우 훨씬 깔끔해 보이는 `match`를 대신 사용할 수 있습니다. 하지만 가능한 모든 결과를 매치해야 합니다. 예를 들어, 이것은 작동하지 않습니다:

```rust
fn main() {
    let my_number: u8 = 5;
    match my_number {
        0 => println!("it's zero"),
        1 => println!("it's one"),
        2 => println!("it's two"),
        // ⚠️
    }
}
```

컴파일러는 다음과 같이 말합니다:

```text
error[E0004]: non-exhaustive patterns: `3u8..=std::u8::MAX` not covered
 --> src\main.rs:3:11
  |
3 |     match my_number {
  |           ^^^^^^^^^ pattern `3u8..=std::u8::MAX` not covered
```

이것은 "0부터 2까지는 말했지만, `u8`은 255까지 갈 수 있습니다. 3은 어떻게 하나요? 4는? 5는?" 등을 의미합니다. 그래서 "그 외 모든 것"을 의미하는 `_`를 추가할 수 있습니다.

```rust
fn main() {
    let my_number: u8 = 5;
    match my_number {
        0 => println!("it's zero"),
        1 => println!("it's one"),
        2 => println!("it's two"),
        _ => println!("It's some other number"),
    }
}
```

그것은 `It's some other number`를 출력합니다.

match에 대해 기억하세요:

- `match`를 쓰고 `{}` 코드 블록을 만듭니다.
- 왼쪽에 *패턴*을 쓰고 `=>` 굵은 화살표를 사용하여 매치될 때 무엇을 할지 말합니다.
- 각 줄을 "arm"이라고 부릅니다.
- arm 사이에 쉼표를 넣습니다 (세미콜론이 아님).

match로 값을 선언할 수 있습니다:

```rust
fn main() {
    let my_number = 5;
    let second_number = match my_number {
        0 => 0,
        5 => 10,
        _ => 2,
    };
}
```

`second_number`는 10이 됩니다. 끝에 세미콜론이 보이나요? 그것은 match가 끝난 후 실제로 컴파일러에게 이렇게 말했기 때문입니다: `let second_number = 10;`

더 복잡한 것들도 매치할 수 있습니다. 튜플을 사용하여 그렇게 합니다.

```rust
fn main() {
    let sky = "cloudy";
    let temperature = "warm";

    match (sky, temperature) {
        ("cloudy", "cold") => println!("It's dark and unpleasant today"),
        ("clear", "warm") => println!("It's a nice day"),
        ("cloudy", "warm") => println!("It's dark but not bad"),
        _ => println!("Not sure what the weather is."),
    }
}
```

이것은 `It's dark but not bad`를 출력합니다. `sky`와 `temperature`에 대해 "cloudy"와 "warm"과 매치하기 때문입니다.

`match` 안에 `if`를 넣을 수도 있습니다. 이것을 "match guard"라고 부릅니다:

```rust
fn main() {
    let children = 5;
    let married = true;

    match (children, married) {
        (children, married) if married == false => println!("Not married with {} children", children),
        (children, married) if children == 0 && married == true => println!("Married but no children"),
        _ => println!("Married? {}. Number of children: {}.", married, children),
    }
}
```

이것은 `Married? true. Number of children: 5.`를 출력합니다.

match에서 원하는 만큼 _를 사용할 수 있습니다. 색상에 대한 이 match에서는 세 개가 있지만 한 번에 하나만 확인합니다.

```rust
fn match_colours(rbg: (i32, i32, i32)) {
    match rbg {
        (r, _, _) if r < 10 => println!("Not much red"),
        (_, b, _) if b < 10 => println!("Not much blue"),
        (_, _, g) if g < 10 => println!("Not much green"),
        _ => println!("Each colour has at least 10"),
    }
}

fn main() {
    let first = (200, 0, 0);
    let second = (50, 50, 50);
    let third = (200, 50, 0);

    match_colours(first);
    match_colours(second);
    match_colours(third);
}
```

이것은 다음을 출력합니다:

```text
Not much blue
Each colour has at least 10
Not much green
```

이것은 또한 `match` 문이 어떻게 작동하는지 보여줍니다. 첫 번째 예제에서는 `Not much blue`만 출력했기 때문입니다. 하지만 `first`는 녹색도 부족합니다. `match` 문은 항상 매치를 찾으면 멈추고 나머지를 확인하지 않습니다. 이것은 잘 컴파일되지만 원하는 코드가 아닌 좋은 예입니다.

정말 큰 `match` 문을 만들어 고칠 수 있지만, `for` 루프를 사용하는 것이 아마 더 좋을 것입니다. 곧 루프에 대해 이야기할 것입니다.

match는 같은 타입을 반환해야 합니다. 그래서 이것을 할 수 없습니다:

```rust
fn main() {
    let my_number = 10;
    let some_variable = match my_number {
        10 => 8,
        _ => "Not ten", // ⚠️
    };
}
```

컴파일러는 다음과 같이 알려줍니다:

```text
error[E0308]: `match` arms have incompatible types
  --> src\main.rs:17:14
   |
15 |       let some_variable = match my_number {
   |  _________________________-
16 | |         10 => 8,
   | |               - this is found to be of type `{integer}`
17 | |         _ => "Not ten",
   | |              ^^^^^^^^^ expected integer, found `&str`
18 | |     };
   | |_____- `match` arms have incompatible types
```

같은 이유로 이것도 작동하지 않습니다:

```rust
fn main() {
    let some_variable = if my_number == 10 { 8 } else { "something else "}; // ⚠️
}
```

하지만 이것은 작동합니다. `match`가 아니므로 매번 다른 `let` 문을 가지기 때문입니다:

```rust
fn main() {
    let my_number = 10;

    if my_number == 10 {
        let some_variable = 8;
    } else {
        let some_variable = "Something else";
    }
}
```

`@`를 사용하여 `match` 표현식의 값에 이름을 지을 수도 있고, 그것을 사용할 수 있습니다. 이 예제에서는 함수의 `i32` 입력을 매치합니다. 4나 13이면 `println!` 문에서 그 숫자를 사용하고 싶습니다. 그렇지 않으면 사용할 필요가 없습니다.

```rust
fn match_number(input: i32) {
    match input {
    number @ 4 => println!("{} is an unlucky number in China (sounds close to 死)!", number),
    number @ 13 => println!("{} is unlucky in North America, lucky in Italy! In bocca al lupo!", number),
    _ => println!("Looks like a normal number"),
    }
}

fn main() {
    match_number(50);
    match_number(13);
    match_number(4);
}
```

이것은 다음을 출력합니다:

```text
Looks like a normal number
13 is unlucky in North America, lucky in Italy! In bocca al lupo!
4 is an unlucky number in China (sounds close to 死)!
```

## 구조체

**YouTube에서 이 챕터 보기: [파트 1](https://youtu.be/W23uQghBOFk)과 [파트 2](https://youtu.be/GSVhrjLCuNA)**

구조체로 자신만의 타입을 만들 수 있습니다. 구조체는 매우 편리하기 때문에 Rust에서 항상 사용할 것입니다. 구조체는 `struct` 키워드로 만들어집니다. 구조체의 이름은 UpperCamelCase여야 합니다 (각 단어의 첫 글자가 대문자, 공백 없음). 모두 소문자로 구조체를 쓰면 컴파일러가 알려줍니다.

세 가지 타입의 구조체가 있습니다. 하나는 "unit struct"입니다. Unit은 "아무것도 없다"는 의미입니다. unit struct의 경우 이름과 세미콜론만 쓰면 됩니다.

```rust
struct FileDirectory;
fn main() {}
```

다음은 튜플 구조체 또는 이름 없는 구조체입니다. 필드 이름이 아닌 타입만 쓰면 되기 때문에 "이름 없음"입니다. 튜플 구조체는 간단한 구조체가 필요하고 이름을 기억할 필요가 없을 때 좋습니다.

```rust
struct Colour(u8, u8, u8);

fn main() {
    let my_colour = Colour(50, 0, 50); // RGB(빨강, 초록, 파랑)로 색상을 만듭니다
    println!("The second part of the colour is: {}", my_colour.1);
}
```

이것은 `The second part of the colour is: 0`을 출력합니다.

세 번째 타입은 이름있는 구조체입니다. 이것은 아마도 가장 일반적인 구조체일 것입니다. 이 구조체에서는 `{}` 코드 블록 안에 필드 이름과 타입을 선언합니다. 이름있는 구조체 뒤에는 전체 코드 블록이 오기 때문에 세미콜론을 쓰지 않는다는 점에 주의하세요.

```rust
struct Colour(u8, u8, u8); // 같은 Colour 튜플 구조체를 선언합니다

struct SizeAndColour {
    size: u32,
    colour: Colour, // 새로운 이름있는 구조체에 넣습니다
}

fn main() {
    let my_colour = Colour(50, 0, 50);

    let size_and_colour = SizeAndColour {
        size: 150,
        colour: my_colour
    };
}
```

이름있는 구조체에서도 필드를 쉼표로 구분합니다. 마지막 필드에는 쉼표를 추가하거나 추가하지 않아도 됩니다 - 여러분의 선택입니다. `SizeAndColour`는 `colour` 뒤에 쉼표가 있었습니다:

```rust
struct Colour(u8, u8, u8); // 같은 Colour 튜플 구조체를 선언합니다

struct SizeAndColour {
    size: u32,
    colour: Colour, // 새로운 이름있는 구조체에 넣습니다
}

fn main() {}
```

하지만 필요하지는 않습니다. 하지만 항상 쉼표를 넣는 것이 좋은 아이디어일 수 있습니다. 때로는 필드의 순서를 변경할 수 있기 때문입니다:

```rust
struct Colour(u8, u8, u8); // 같은 Colour 튜플 구조체를 선언합니다

struct SizeAndColour {
    size: u32,
    colour: Colour // 여기에는 쉼표가 없습니다
}

fn main() {}
```

그런 다음 순서를 변경하기로 결정합니다...

```rust
struct SizeAndColour {
    colour: Colour // ⚠️ 앗! 이제 여기에 쉼표가 없습니다.
    size: u32,
}

fn main() {}
```

하지만 어느 쪽이든 그렇게 중요하지는 않으므로 쉼표를 사용할지 말지는 선택할 수 있습니다.

예시를 들기 위해 `Country` 구조체를 만들어 보겠습니다. `Country` 구조체에는 `population`, `capital`, `leader_name` 필드가 있습니다.

```rust
struct Country {
    population: u32,
    capital: String,
    leader_name: String
}

fn main() {
    let population = 500_000;
    let capital = String::from("Elista");
    let leader_name = String::from("Batu Khasikov");

    let kalmykia = Country {
        population: population,
        capital: capital,
        leader_name: leader_name,
    };
}
```

같은 것을 두 번 썼다는 것을 눈치채셨나요? `population: population`, `capital: capital`, `leader_name: leader_name`이라고 썼습니다. 실제로는 그럴 필요가 없습니다. 필드 이름과 변수 이름이 같다면 두 번 쓸 필요가 없습니다.

```rust
struct Country {
    population: u32,
    capital: String,
    leader_name: String
}

fn main() {
    let population = 500_000;
    let capital = String::from("Elista");
    let leader_name = String::from("Batu Khasikov");

    let kalmykia = Country {
        population,
        capital,
        leader_name,
    };
}
```

## 열거형

**YouTube에서 이 챕터 보기: [파트 1](https://youtu.be/SRnqNTJUgjs), [파트 2](https://youtu.be/F_EcbWM63lk), [파트 3](https://youtu.be/2uh64U9JesA) 그리고 [파트 4](https://youtu.be/LOHVUYTc5Us)**

`enum`은 열거형(enumerations)의 줄임말입니다. 구조체와 매우 비슷해 보이지만 다릅니다. 차이점은 다음과 같습니다:

- 한 가지 **그리고** 다른 한 가지를 원할 때 `struct`를 사용합니다.
- 한 가지 **또는** 다른 한 가지를 원할 때 `enum`을 사용합니다.

따라서 구조체는 **여러 가지**를 함께 사용하는 것이고, 열거형은 **여러 선택지** 중 하나를 선택하는 것입니다.

열거형을 선언하려면 `enum`을 쓰고 쉼표로 구분된 옵션들과 함께 코드 블록을 사용합니다. `struct`와 마찬가지로 마지막 부분에는 쉼표가 있어도 되고 없어도 됩니다. `ThingsInTheSky`라는 열거형을 만들어 보겠습니다:

```rust
enum ThingsInTheSky {
    Sun,
    Stars,
}

fn main() {}
```

이것이 열거형인 이유는 태양을 보거나 **또는** 별을 볼 수 있기 때문입니다: 하나를 선택해야 합니다. 이들을 **배리언트(variants)**라고 부릅니다.

```rust
// 두 가지 선택지가 있는 열거형을 만듭니다
enum ThingsInTheSky {
    Sun,
    Stars,
}

// 이 함수로 i32를 사용해서 ThingsInTheSky를 만들 수 있습니다.
fn create_skystate(time: i32) -> ThingsInTheSky {
    match time {
        6..=18 => ThingsInTheSky::Sun, // 6시에서 18시 사이에는 태양을 볼 수 있습니다
        _ => ThingsInTheSky::Stars, // 그렇지 않으면 별을 볼 수 있습니다
    }
}

// 이 함수로 ThingsInTheSky의 두 선택지를 매치할 수 있습니다.
fn check_skystate(state: &ThingsInTheSky) {
    match state {
        ThingsInTheSky::Sun => println!("I can see the sun!"),
        ThingsInTheSky::Stars => println!("I can see the stars!")
    }
}

fn main() {
    let time = 8; // 8시입니다
    let skystate = create_skystate(time); // create_skystate는 ThingsInTheSky를 반환합니다
    check_skystate(&skystate); // 변수 skystate를 읽을 수 있도록 참조를 전달합니다
}
```

이것은 `I can see the sun!`을 출력합니다.

열거형에 데이터를 추가할 수도 있습니다.

```rust
enum ThingsInTheSky {
    Sun(String), // 이제 각 배리언트에 문자열이 있습니다
    Stars(String),
}

fn create_skystate(time: i32) -> ThingsInTheSky {
    match time {
        6..=18 => ThingsInTheSky::Sun(String::from("I can see the sun!")), // 여기에 문자열을 작성합니다
        _ => ThingsInTheSky::Stars(String::from("I can see the stars!")),
    }
}

fn check_skystate(state: &ThingsInTheSky) {
    match state {
        ThingsInTheSky::Sun(description) => println!("{}", description), // 문자열에 description이라는 이름을 주어 사용할 수 있습니다
        ThingsInTheSky::Stars(n) => println!("{}", n), // 또는 n이라고 이름을 줄 수 있습니다. 또는 다른 어떤 이름이든 - 상관없습니다
    }
}

fn main() {
    let time = 8; // 8시입니다
    let skystate = create_skystate(time); // create_skystate는 ThingsInTheSky를 반환합니다
    check_skystate(&skystate); // 변수 skystate를 읽을 수 있도록 참조를 전달합니다
}
```

이것은 같은 것을 출력합니다: `I can see the sun!`

열거형을 "import"해서 너무 많이 타이핑하지 않아도 됩니다. 다음은 기분을 매치할 때마다 `Mood::`를 타이핑해야 하는 예시입니다:

```rust
enum Mood {
    Happy,
    Sleepy,
    NotBad,
    Angry,
}

fn match_mood(mood: &Mood) -> i32 {
    let happiness_level = match mood {
        Mood::Happy => 10, // 여기서 매번 Mood::를 타이핑합니다
        Mood::Sleepy => 6,
        Mood::NotBad => 7,
        Mood::Angry => 2,
    };
    happiness_level
}

fn main() {
    let my_mood = Mood::NotBad;
    let happiness_level = match_mood(&my_mood);
    println!("Out of 1 to 10, my happiness is {}", happiness_level);
}
```

이것은 `Out of 1 to 10, my happiness is 7`을 출력합니다. 덜 타이핑하기 위해 import해 보겠습니다. 모든 것을 import하려면 `*`를 쓰세요. 주의: 역참조를 위한 `*`와 같은 키이지만 완전히 다릅니다.

```rust
enum Mood {
    Happy,
    Sleepy,
    NotBad,
    Angry,
}

fn match_mood(mood: &Mood) -> i32 {
    use Mood::*; // Mood의 모든 것을 import했습니다. 이제 그냥 Happy, Sleepy 등을 쓸 수 있습니다.
    let happiness_level = match mood {
        Happy => 10, // 더 이상 Mood::를 쓸 필요가 없습니다
        Sleepy => 6,
        NotBad => 7,
        Angry => 2,
    };
    happiness_level
}

fn main() {
    let my_mood = Mood::Happy;
    let happiness_level = match_mood(&my_mood);
    println!("Out of 1 to 10, my happiness is {}", happiness_level);
}
```

`enum`의 부분들을 정수로 변환할 수도 있습니다. Rust가 자체적으로 사용하기 위해 `enum`의 각 arm에 0부터 시작하는 번호를 부여하기 때문입니다. enum에 다른 데이터가 없다면 이를 활용할 수 있습니다.

```rust
enum Season {
    Spring, // 만약 이게 Spring(String) 같은 형태였다면 작동하지 않을 것입니다
    Summer,
    Autumn,
    Winter,
}

fn main() {
    use Season::*;
    let four_seasons = vec![Spring, Summer, Autumn, Winter];
    for season in four_seasons {
        println!("{}", season as u32);
    }
}
```

이것은 다음을 출력합니다:

```text
0
1
2
3
```

원한다면 다른 번호를 줄 수도 있습니다 - Rust는 신경 쓰지 않고 같은 방식으로 사용할 수 있습니다. 번호를 가지고 싶은 배리언트에 `=`와 번호를 추가하기만 하면 됩니다. 모든 배리언트에 번호를 줄 필요는 없습니다. 하지만 주지 않으면 Rust는 이전 arm에서 1을 더해서 번호를 줄 것입니다.

```rust
enum Star {
    BrownDwarf = 10,
    RedDwarf = 50,
    YellowStar = 100,
    RedGiant = 1000,
    DeadStar, // 이것에 대해 생각해보세요. 어떤 번호를 가질까요?
}

fn main() {
    use Star::*;
    let starvec = vec![BrownDwarf, RedDwarf, YellowStar, RedGiant];
    for star in starvec {
        match star as u32 {
            size if size <= 80 => println!("Not the biggest star."), // 기억하세요: size는 아무 의미가 없습니다. 출력할 수 있도록 우리가 선택한 이름일 뿐입니다
            size if size >= 80 => println!("This is a good-sized star."),
            _ => println!("That star is pretty big!"),
        }
    }
    println!("What about DeadStar? It's the number {}.", DeadStar as u32);
}
```

이것은 다음을 출력합니다:

```text
Not the biggest star.
Not the biggest star.
This is a good-sized star.
This is a good-sized star.
What about DeadStar? It's the number 1001.
```

`DeadStar`는 번호 4였을 것이지만, 이제는 1001입니다.

### 여러 타입을 사용하기 위한 열거형

`Vec`, 배열 등의 항목들은 모두 같은 타입이어야 한다는 것을 알고 있습니다 (튜플만 다릅니다). 하지만 실제로는 enum을 사용해서 다른 타입들을 넣을 수 있습니다. `u32`나 `i32`가 있는 `Vec`을 원한다고 상상해보세요. 물론 `Vec<(u32, i32)>` (`(u32, i32)` 튜플이 있는 벡터)를 만들 수 있지만 우리는 매번 하나씩만 원합니다. 여기서 enum을 사용할 수 있습니다. 간단한 예시가 있습니다:

```rust
enum Number {
    U32(u32),
    I32(i32),
}

fn main() {}
```

두 개의 배리언트가 있습니다: 내부에 `u32`가 있는 `U32` 배리언트와 내부에 `i32`가 있는 `I32` 배리언트입니다. `U32`와 `I32`는 우리가 만든 이름일 뿐입니다. `UThirtyTwo`나 `IThirtyTwo` 또는 다른 어떤 것이어도 될 수 있었습니다.

이제 이들을 `Vec`에 넣으면 `Vec<Number>`만 있으면 되고, 컴파일러는 모두 같은 타입이기 때문에 만족합니다. 컴파일러는 `u32`나 `i32`가 있다는 것을 신경 쓰지 않습니다. 왜냐하면 모두 `Number`라는 단일 타입 안에 있기 때문입니다. 그리고 enum이기 때문에 하나를 선택해야 하는데, 이것이 우리가 원하는 것입니다. `.is_positive()` 메서드를 사용해서 선택할 것입니다. `true`라면 `U32`를 선택하고, `false`라면 `I32`를 선택할 것입니다.

이제 코드는 다음과 같습니다:

```rust
enum Number {
    U32(u32),
    I32(i32),
}

fn get_number(input: i32) -> Number {
    let number = match input.is_positive() {
        true => Number::U32(input as u32), // 양수라면 u32로 변경합니다
        false => Number::I32(input), // 그렇지 않으면 이미 i32이므로 그냥 숫자를 줍니다
    };
    number
}


fn main() {
    let my_vec = vec![get_number(-800), get_number(8)];

    for item in my_vec {
        match item {
            Number::U32(number) => println!("It's a u32 with the value {}", number),
            Number::I32(number) => println!("It's an i32 with the value {}", number),
        }
    }
}
```

이것은 우리가 보고 싶었던 것을 출력합니다:

```text
It's an i32 with the value -800
It's a u32 with the value 8
```

## 루프

루프를 사용하면 Rust에게 중지하라고 말할 때까지 무언가를 계속하라고 말할 수 있습니다. `loop`를 사용해서 `break`를 언제 할지 말하지 않는 한 멈추지 않는 루프를 시작합니다.

```rust
fn main() { // 이 프로그램은 절대 멈추지 않을 것입니다
    loop {

    }
}
```

그러니 컴파일러에게 언제 중단할 수 있는지 말해봅시다.

```rust
fn main() {
    let mut counter = 0; // 카운터를 0으로 설정합니다
    loop {
        counter +=1; // 카운터를 1씩 증가시킵니다
        println!("The counter is now: {}", counter);
        if counter == 5 { // counter == 5일 때 멈춥니다
            break;
        }
    }
}
```

이것은 다음을 출력할 것입니다:

```text
The counter is now: 1
The counter is now: 2
The counter is now: 3
The counter is now: 4
The counter is now: 5
```

루프 안에 루프가 있다면 이름을 줄 수 있습니다. 이름을 가지면 Rust에게 어떤 루프에서 `break`할지 말할 수 있습니다. `'` ("틱"이라고 불림)와 `:`를 사용해서 이름을 줍니다:

```rust
fn main() {
    let mut counter = 0;
    let mut counter2 = 0;
    println!("Now entering the first loop.");

    'first_loop: loop {
        // 첫 번째 루프에 이름을 줍니다
        counter += 1;
        println!("The counter is now: {}", counter);
        if counter > 9 {
            // 이 루프 안에서 두 번째 루프를 시작합니다
            println!("Now entering the second loop.");

            'second_loop: loop {
                // 이제 우리는 'second_loop 안에 있습니다
                println!("The second counter is now: {}", counter2);
                counter2 += 1;
                if counter2 == 3 {
                    break 'first_loop; // 프로그램을 종료할 수 있도록 'first_loop에서 벗어납니다
                }
            }
        }
    }
}
```

이것은 다음을 출력할 것입니다:

```text
Now entering the first loop.
The counter is now: 1
The counter is now: 2
The counter is now: 3
The counter is now: 4
The counter is now: 5
The counter is now: 6
The counter is now: 7
The counter is now: 8
The counter is now: 9
The counter is now: 10
Now entering the second loop.
The second counter is now: 0
The second counter is now: 1
The second counter is now: 2
```

`while` 루프는 무언가가 여전히 `true`인 동안 계속되는 루프입니다. 각 루프마다 Rust는 여전히 `true`인지 확인할 것입니다. `false`가 되면 Rust는 루프를 멈출 것입니다.

```rust
fn main() {
    let mut counter = 0;

    while counter < 5 {
        counter +=1;
        println!("The counter is now: {}", counter);
    }
}
```

`for` 루프는 Rust에게 매번 무엇을 할지 말할 수 있게 해줍니다. 하지만 `for` 루프에서는 루프가 정해진 횟수 후에 멈춥니다. `for` 루프는 **범위**를 매우 자주 사용합니다. 범위를 만들기 위해 `..`와 `..=`를 사용합니다.

- `..`는 **배타적** 범위를 만듭니다: `0..3`은 `0, 1, 2`를 만듭니다.
- `..=`는 **포함** 범위를 만듭니다: `0..=3` = `0, 1, 2, 3`.

```rust
fn main() {
    for number in 0..3 {
        println!("The number is: {}", number);
    }

    for number in 0..=3 {
        println!("The next number is: {}", number);
    }
}
```

이것은 다음을 출력합니다:

```text
The number is: 0
The number is: 1
The number is: 2
The next number is: 0
The next number is: 1
The next number is: 2
The next number is: 3
```

또한 `number`가 0..3의 변수 이름이 된다는 것에 주목하세요. `n`이나 `ntod_het___hno_f`, 또는 다른 어떤 것이라고 불렀을 수도 있습니다. 그러면 `println!`에서 그 이름을 사용할 수 있습니다.

변수 이름이 필요하지 않다면 `_`를 사용하세요.

```rust
fn main() {
    for _ in 0..3 {
        println!("Printing the same thing three times");
    }
}
```

이것은 다음을 출력합니다:

```text
Printing the same thing three times
Printing the same thing three times
Printing the same thing three times
```

매번 출력할 숫자를 주지 않았기 때문입니다.

그리고 실제로 변수 이름을 주고 사용하지 않으면 Rust가 알려줄 것입니다:

```rust
fn main() {
    for number in 0..3 {
        println!("Printing the same thing three times");
    }
}
```

이것은 위와 같은 것을 출력합니다. 프로그램은 잘 컴파일되지만, Rust는 `number`를 사용하지 않았다고 알려줄 것입니다:

```text
warning: unused variable: `number`
 --> src\main.rs:2:9
  |
2 |     for number in 0..3 {
  |         ^^^^^^ help: if this is intentional, prefix it with an underscore: `_number`
```

Rust는 `_` 대신 `_number`를 쓰라고 제안합니다. 변수 이름 앞에 `_`를 넣는 것은 "아마 나중에 사용할 것"을 의미합니다. 하지만 그냥 `_`만 사용하는 것은 "이 변수에 대해 전혀 신경 쓰지 않는다"는 의미입니다. 따라서 나중에 사용할 변수이고 컴파일러가 이에 대해 알려주는 것을 원하지 않는다면 변수 이름 앞에 `_`를 넣을 수 있습니다.

`break`를 사용해서 값을 반환할 수도 있습니다. `break` 바로 뒤에 값을 쓰고 `;`를 사용합니다. 다음은 `loop`와 `my_number`에 값을 주는 break의 예시입니다.

```rust
fn main() {
    let mut counter = 5;
    let my_number = loop {
        counter +=1;
        if counter % 53 == 3 {
            break counter;
        }
    };
    println!("{}", my_number);
}
```

이것은 `56`을 출력합니다. `break counter;`는 "중단하고 counter의 값을 반환한다"는 의미입니다. 그리고 전체 블록이 `let`으로 시작하기 때문에 `my_number`가 그 값을 받습니다.

이제 루프를 사용하는 방법을 알았으므로, 이전의 색상과 관련된 `match` 문제에 대한 더 나은 해결책이 있습니다. 모든 것을 비교하고 싶고 `for` 루프가 모든 항목을 보기 때문에 더 나은 해결책입니다.

```rust
fn match_colours(rbg: (i32, i32, i32)) {
    println!("Comparing a colour with {} red, {} blue, and {} green:", rbg.0, rbg.1, rbg.2);
    let new_vec = vec![(rbg.0, "red"), (rbg.1, "blue"), (rbg.2, "green")]; // 색상을 벡터에 넣습니다. 안에는 색상 이름이 있는 튜플들이 있습니다
    let mut all_have_at_least_10 = true; // true로 시작합니다. 한 색상이 10보다 작으면 false로 설정할 것입니다
    for item in new_vec {
        if item.0 < 10 {
            all_have_at_least_10 = false; // 이제 false입니다
            println!("Not much {}.", item.1) // 그리고 색상 이름을 출력합니다.
        }
    }
    if all_have_at_least_10 { // 여전히 true인지 확인하고, true라면 출력합니다
        println!("Each colour has at least 10.")
    }
    println!(); // 한 줄 더 추가합니다
}

fn main() {
    let first = (200, 0, 0);
    let second = (50, 50, 50);
    let third = (200, 50, 0);

    match_colours(first);
    match_colours(second);
    match_colours(third);
}
```

이것은 다음과 같이 출력합니다:

```text
Comparing a colour with 200 red, 0 blue, and 0 green:
Not much blue.
Not much green.

Comparing a colour with 50 red, 50 blue, and 50 green:
Each colour has at least 10.

Comparing a colour with 200 red, 50 blue, and 0 green:
Not much green.
```

## 구조체와 열거형 구현하기

여기서부터 구조체와 열거형에 진정한 힘을 줄 수 있습니다. `struct`나 `enum`에서 함수를 호출하려면 `impl` 블록을 사용합니다. 이러한 함수들을 **메서드**라고 부릅니다. `impl` 블록에는 두 종류의 메서드가 있습니다.

- 메서드: **self**(또는 **&self** 또는 **&mut self**)를 가집니다. 일반 메서드는 `.`(마침표)를 사용합니다. `.clone()`은 일반 메서드의 예입니다.
- 연관 함수(일부 언어에서는 "정적" 메서드라고 함): self를 가지지 않습니다. 연관은 "관련된"을 의미합니다. 이들은 다르게 작성되며 `::`을 사용합니다. `String::from()`은 연관 함수이고 `Vec::new()`도 마찬가지입니다. 새 변수를 만들 때 연관 함수를 가장 자주 사용합니다.

우리 예시에서는 동물들을 만들고 출력할 것입니다.

새로운 `struct`나 `enum`의 경우, 출력에 `{:?}`를 사용하려면 **Debug**를 제공해야 하므로 그렇게 할 것입니다. struct나 enum 위에 `#[derive(Debug)]`를 작성하면 `{:?}`로 출력할 수 있습니다. `#[]`가 있는 이러한 메시지를 **속성**이라고 부릅니다. 때때로 이것들을 사용해서 컴파일러에게 구조체에 `Debug`와 같은 능력을 주라고 말할 수 있습니다. 속성은 많이 있고 나중에 배울 것입니다. 하지만 `derive`는 아마도 가장 일반적이고 구조체와 열거형 위에서 많이 볼 수 있습니다.

```rust
#[derive(Debug)]
struct Animal {
    age: u8,
    animal_type: AnimalType,
}

#[derive(Debug)]
enum AnimalType {
    Cat,
    Dog,
}

impl Animal {
    fn new() -> Self {
        // Self는 Animal을 의미합니다.
        // Self 대신 Animal을 쓸 수도 있습니다

        Self {
            // Animal::new()를 쓸 때, 우리는 항상 10살인 고양이를 얻습니다
            age: 10,
            animal_type: AnimalType::Cat,
        }
    }

    fn change_to_dog(&mut self) { // Animal 안에 있기 때문에, &mut self는 &mut Animal을 의미합니다
                                  // .change_to_dog()를 사용해서 고양이를 개로 바꿉니다
                                  // &mut self로 바꿀 수 있습니다
        println!("Changing animal to dog!");
        self.animal_type = AnimalType::Dog;
    }

    fn change_to_cat(&mut self) {
        // .change_to_cat()를 사용해서 개를 고양이로 바꿉니다
        // &mut self로 바꿀 수 있습니다
        println!("Changing animal to cat!");
        self.animal_type = AnimalType::Cat;
    }

    fn check_type(&self) {
        // self를 읽고 싶습니다
        match self.animal_type {
            AnimalType::Dog => println!("The animal is a dog"),
            AnimalType::Cat => println!("The animal is a cat"),
        }
    }
}



fn main() {
    let mut new_animal = Animal::new(); // 새 동물을 만드는 연관 함수
                                        // 이것은 10살 고양이입니다
    new_animal.check_type();
    new_animal.change_to_dog();
    new_animal.check_type();
    new_animal.change_to_cat();
    new_animal.check_type();
}
```

이것은 다음과 같이 출력합니다:

```text
The animal is a cat
Changing animal to dog!
The animal is a dog
Changing animal to cat!
The animal is a cat
```

## 구조 분해

더 많은 구조 분해에 대해 살펴보겠습니다. `let`을 거꾸로 사용하여 구조체나 열거형에서 값을 가져올 수 있습니다. 이것을 `구조 분해`라고 부르는 이유는 구조의 일부가 아닌 변수들을 얻기 때문입니다. 이제 값들을 따로 가지게 됩니다. 먼저 간단한 예시를 보겠습니다:

```rust
struct Person { // 사람을 위한 간단한 구조체를 만듭니다
    name: String,
    real_name: String,
    height: u8,
    happiness: bool
}

fn main() {
    let papa_doc = Person { // papa_doc 변수를 생성합니다
        name: "Papa Doc".to_string(),
        real_name: "Clarence".to_string(),
        height: 170,
        happiness: false
    };

    let Person { // papa_doc을 구조 분해합니다
        name: a,
        real_name: b,
        height: c,
        happiness: d
    } = papa_doc;

    println!("그들은 그를 {}라고 부르지만 그의 실제 이름은 {}입니다. 그는 키가 {}cm이고 행복한가요? {}", a, b, c, d);
}
```

이것은 다음과 같이 출력합니다: `They call him Papa Doc but his real name is Clarence. He is 170 cm tall and is he happy? false`

거꾸로 된 것을 볼 수 있습니다. 먼저 구조체를 생성하기 위해 `let papa_doc = Person { fields }`라고 말합니다. 그 다음 구조 분해하기 위해 `let Person { fields } = papa_doc`라고 말합니다.

`name: a`라고 쓸 필요는 없습니다 - 그냥 `name`이라고 쓸 수 있습니다. 하지만 여기서는 `a`라는 이름의 변수를 사용하고 싶기 때문에 `name: a`라고 씁니다.

이제 더 큰 예시입니다. 이 예시에서는 `City` 구조체가 있습니다. 이것을 만들기 위해 `new` 함수를 제공합니다. 그런 다음 값들로 작업하기 위한 `process_city_values` 함수가 있습니다. 함수에서는 그냥 `Vec`을 생성하지만, 구조 분해한 후에 훨씬 더 많은 것을 할 수 있다고 상상할 수 있습니다.

```rust
struct City {
    name: String,
    name_before: String,
    population: u32,
    date_founded: u32,
}

impl City {
    fn new(name: String, name_before: String, population: u32, date_founded: u32) -> Self {
        Self {
            name,
            name_before,
            population,
            date_founded,
        }
    }
}

fn process_city_values(city: &City) {
    let City {
        name,
        name_before,
        population,
        date_founded,
    } = city;
        // 이제 값들을 따로 사용할 수 있습니다
    let two_names = vec![name, name_before];
    println!("도시의 두 이름은 {:?}입니다", two_names);
}

fn main() {
    let tallinn = City::new("Tallinn".to_string(), "Reval".to_string(), 426_538, 1219);
    process_city_values(&tallinn);
}
```

이것은 `The city's two names are ["Tallinn", "Reval"]`을 출력합니다.

## 제네릭

함수에서는 입력으로 받을 타입을 다음과 같이 명시합니다:

```rust
fn return_number(number: i32) -> i32 {
    println!("여기 당신의 숫자입니다.");
    number
}

fn main() {
    let number = return_number(5);
}
```

하지만 `i32`뿐만 아니라 더 많은 타입을 받고 싶다면 어떻게 할까요? 이를 위해 제네릭을 사용할 수 있습니다. 제네릭은 "어떤 타입일 수도 있고, 다른 타입일 수도 있다"는 의미입니다.

제네릭의 경우, 다음과 같이 타입을 내부에 넣은 꺾쇠 괄호를 사용합니다: `<T>` 이것은 "함수에 넣는 모든 타입"을 의미합니다. 보통 제네릭은 한 대문자를 사용합니다(T, U, V 등), 하지만 꼭 한 글자만 사용할 필요는 없습니다.

다음은 함수를 제네릭으로 변경하는 방법입니다:

```rust
fn return_number<T>(number: T) -> T {
    println!("여기 당신의 숫자입니다.");
    number
}

fn main() {
    let number = return_number(5);
}
```

중요한 부분은 함수 이름 뒤의 `<T>`입니다. 이것이 없으면 Rust는 T가 `String`이나 `i8`과 같은 구체적인(concrete = 제네릭이 아닌) 타입이라고 생각합니다.

타입 이름을 작성하면 이해하기 더 쉽습니다. `T`를 `MyType`으로 바꾸면 어떤 일이 일어나는지 봅시다:

```rust
fn return_number(number: MyType) -> MyType { // ⚠️
    println!("여기 당신의 숫자입니다.");
    number
}
```

보시다시피, `MyType`은 구체적이지 제네릭이 아닙니다. 그래서 다음과 같이 작성해야 하고 이제 작동합니다:

```rust
fn return_number<MyType>(number: MyType) -> MyType {
    println!("여기 당신의 숫자입니다.");
    number
}

fn main() {
    let number = return_number(5);
}
```

따라서 단일 문자 `T`는 사람의 눈을 위한 것이지만, 함수 이름 뒤의 부분은 컴파일러의 "눈"을 위한 것입니다. 이것이 없으면 제네릭이 아닙니다.

이제 Rust 코드에서 일반적으로 `T`를 사용하므로 타입 `T`로 돌아가겠습니다.

Rust의 일부 타입들이 **Copy**, **Clone**, **Display**, **Debug** 등이라는 것을 기억할 것입니다. **Debug**를 사용하면 `{:?}`로 출력할 수 있습니다. 이제 `T`를 출력하려고 할 때 문제가 있다는 것을 알 수 있습니다:

```rust
fn print_number<T>(number: T) {
    println!("여기 당신의 숫자입니다: {:?}", number); // ⚠️
}

fn main() {
    print_number(5);
}
```

`print_number`는 `number`를 출력하기 위해 **Debug**가 필요하지만, `T`가 `Debug`를 가진 타입일까요? 아닐 수도 있습니다. `#[derive(Debug)]`가 없을 수도 있습니다. 컴파일러도 모르므로 오류를 제공합니다:

```text
error[E0277]: `T` doesn't implement `std::fmt::Debug`
  --> src\main.rs:29:43
   |
29 |     println!("Here is your number: {:?}", number);
   |                                           ^^^^^^ `T` cannot be formatted using `{:?}` because it doesn't implement `std::fmt::Debug`
```

T는 **Debug**를 구현하지 않습니다. 그럼 T에 대해 Debug를 구현해야 할까요? 아니요, T가 무엇인지 모르기 때문입니다. 하지만 함수에게 "걱정하지 마세요, 이 함수의 모든 타입 T는 Debug를 가질 것입니다"라고 말할 수 있습니다.

```rust
use std::fmt::Debug; // Debug는 std::fmt::Debug에 위치합니다. 이제 그냥 'Debug'라고 쓸 수 있습니다.

fn print_number<T: Debug>(number: T) { // <T: Debug>가 중요한 부분입니다
    println!("여기 당신의 숫자입니다: {:?}", number);
}

fn main() {
    print_number(5);
}
```

이제 컴파일러가 알게 됩니다: "좋아요, 이 타입 T는 Debug를 가질 것입니다." 이제 `i32`가 Debug를 가지고 있으므로 코드가 작동합니다. 이제 Debug를 가진 모든 타입들(`String`, `&str` 등)을 제공할 수 있습니다.

이제 구조체를 만들고 #[derive(Debug)]로 Debug를 제공할 수 있으므로, 이것도 출력할 수 있습니다. 우리 함수는 `i32`, Animal 구조체 등을 받을 수 있습니다:

```rust
use std::fmt::Debug;

#[derive(Debug)]
struct Animal {
    name: String,
    age: u8,
}

fn print_item<T: Debug>(item: T) {
    println!("여기 당신의 아이템입니다: {:?}", item);
}

fn main() {
    let charlie = Animal {
        name: "Charlie".to_string(),
        age: 1,
    };

    let number = 55;

    print_item(charlie);
    print_item(number);
}
```

이것은 다음과 같이 출력합니다:

```text
여기 당신의 아이템입니다: Animal { name: "Charlie", age: 1 }
여기 당신의 아이템입니다: 55
```

때때로 제네릭 함수에서 하나 이상의 타입이 필요합니다. 각 타입 이름을 작성하고 어떻게 사용할지 생각해야 합니다. 이 예시에서는 두 가지 타입이 필요합니다. 먼저 타입 T에 대한 문장을 출력하고 싶습니다. `{}`로 출력하는 것이 더 좋으므로 `T`에 대해 `Display`를 요구할 것입니다.

다음은 타입 U이고, 두 변수 `num_1`과 `num_2`는 타입 U를 가집니다(U는 어떤 종류의 숫자입니다). 이들을 비교하고 싶으므로 `PartialOrd`가 필요합니다. 이 트레이트는 `<`, `>`, `==` 등을 사용할 수 있게 해줍니다. 이들도 출력하고 싶으므로 `U`에 대해서도 `Display`를 요구합니다.

```rust
use std::fmt::Display;
use std::cmp::PartialOrd;

fn compare_and_display<T: Display, U: Display + PartialOrd>(statement: T, num_1: U, num_2: U) {
    println!("{}! {}가 {}보다 큰가요? {}", statement, num_1, num_2, num_1 > num_2);
}

fn main() {
    compare_and_display("들어보세요!", 9, 8);
}
```

이것은 `들어보세요!! 9가 8보다 큰가요? true`를 출력합니다.

따라서 `fn compare_and_display<T: Display, U: Display + PartialOrd>(statement: T, num_1: U, num_2: U)`는 다음을 의미합니다:

- 함수 이름은 `compare_and_display`입니다,
- 첫 번째 타입은 T이고, 제네릭입니다. {}로 출력할 수 있는 타입이어야 합니다.
- 다음 타입은 U이고, 제네릭입니다. {}로 출력할 수 있는 타입이어야 합니다. 또한 비교할 수 있는 타입이어야 합니다(`>`, `<`, `==` 사용).

이제 `compare_and_display`에 다른 타입들을 제공할 수 있습니다. `statement`는 `String`, `&str`, Display를 가진 모든 것이 될 수 있습니다.

제네릭 함수를 읽기 쉽게 만들기 위해, 코드 블록 바로 앞에 `where`를 사용해서 다음과 같이 쓸 수도 있습니다:

```rust
use std::cmp::PartialOrd;
use std::fmt::Display;

fn compare_and_display<T, U>(statement: T, num_1: U, num_2: U)
where
    T: Display,
    U: Display + PartialOrd,
{
    println!("{}! {}가 {}보다 큰가요? {}", statement, num_1, num_2, num_1 > num_2);
}

fn main() {
    compare_and_display("들어보세요!", 9, 8);
}
```

많은 제네릭 타입이 있을 때 `where`를 사용하는 것이 좋은 아이디어입니다.

또한 주의하세요:

- 하나의 타입 T와 다른 타입 T가 있다면, 같은 타입이어야 합니다.
- 하나의 타입 T와 다른 타입 U가 있다면, 다를 수 있습니다. 하지만 같을 수도 있습니다.

예를 들어:

```rust
use std::fmt::Display;

fn say_two<T: Display, U: Display>(statement_1: T, statement_2: U) { // 타입 T는 Display가 필요하고, 타입 U는 Display가 필요합니다
    println!("할 말이 두 가지 있습니다: {}와 {}", statement_1, statement_2);
}

fn main() {

    say_two("안녕하세요!", String::from("나는 모래가 싫어요.")); // 타입 T는 &str이지만 타입 U는 String입니다.
    say_two(String::from("파드메는 어디에 있나요?"), String::from("그녀는 괜찮나요?")); // 두 타입 모두 String입니다.
}
```

이것은 다음과 같이 출력합니다:

```text
할 말이 두 가지 있습니다: 안녕하세요!와 나는 모래가 싫어요.
할 말이 두 가지 있습니다: 파드메는 어디에 있나요?와 그녀는 괜찮나요?
```

## Option과 Result

이제 열거형(enums)과 제네릭을 이해했으므로, `Option`과 `Result`를 이해할 수 있습니다. Rust는 이 두 열거형을 사용하여 코드를 더 안전하게 만듭니다.

먼저 `Option`부터 시작하겠습니다.

### Option

값이 존재할 수도 있고 존재하지 않을 수도 있을 때 `Option`을 사용합니다. 값이 존재하면 `Some(value)`이고, 존재하지 않으면 그냥 `None`입니다. 다음은 `Option`으로 개선할 수 있는 나쁜 코드의 예입니다.

```rust
    // ⚠️
fn take_fifth(value: Vec<i32>) -> i32 {
    value[4]
}

fn main() {
    let new_vec = vec![1, 2];
    let index = take_fifth(new_vec);
}
```

이 코드를 실행하면 패닉이 발생합니다. 메시지는 다음과 같습니다:

```text
thread 'main' panicked at 'index out of bounds: the len is 2 but the index is 4', src\main.rs:34:5
```

패닉은 문제가 발생하기 전에 프로그램이 중단되는 것을 의미합니다. Rust는 함수가 불가능한 것을 원한다는 것을 보고, 중단합니다. "스택을 되감기"(스택에서 값들을 제거) 하고 "죄송합니다, 그렇게 할 수 없습니다"라고 알려줍니다.

이제 반환 타입을 `i32`에서 `Option<i32>`로 변경하겠습니다. 이는 "값이 있으면 `Some(i32)`를 주고, 없으면 `None`을 줘"라는 의미입니다. `i32`가 `Option`에 "래핑(wrapped)"되어 있다고 말하는데, 이는 `Option` 안에 있다는 뜻입니다. 값을 꺼내려면 뭔가를 해야 합니다.

```rust
fn take_fifth(value: Vec<i32>) -> Option<i32> {
    if value.len() < 5 { // .len()은 벡터의 길이를 반환합니다.
                         // 최소 5여야 합니다.
        None
    } else {
        Some(value[4])
    }
}

fn main() {
    let new_vec = vec![1, 2];
    let bigger_vec = vec![1, 2, 3, 4, 5];
    println!("{:?}, {:?}", take_fifth(new_vec), take_fifth(bigger_vec));
}
```

이것은 `None, Some(5)`를 출력합니다. 좋습니다. 더 이상 패닉이 발생하지 않습니다. 하지만 값 5는 어떻게 얻을까요?

`.unwrap()`으로 Option 안의 값을 얻을 수 있지만, `.unwrap()`을 사용할 때는 조심해야 합니다. 선물을 푸는 것과 같습니다: 안에 좋은 것이 있을 수도 있고, 화난 뱀이 있을 수도 있습니다. 확실할 때만 `.unwrap()`을 사용하고 싶을 것입니다. `None`인 값을 unwrap하면 프로그램이 패닉을 일으킵니다.

```rust
// ⚠️
fn take_fifth(value: Vec<i32>) -> Option<i32> {
    if value.len() < 5 {
        None
    } else {
        Some(value[4])
    }
}

fn main() {
    let new_vec = vec![1, 2];
    let bigger_vec = vec![1, 2, 3, 4, 5];
    println!("{:?}, {:?}",
        take_fifth(new_vec).unwrap(), // 이것은 None입니다. .unwrap()은 패닉을 일으킬 것입니다!
        take_fifth(bigger_vec).unwrap()
    );
}
```

메시지는:

```text
thread 'main' panicked at 'called `Option::unwrap()` on a `None` value', src\main.rs:14:9
```

하지만 `.unwrap()`을 사용할 필요는 없습니다. `match`를 사용할 수 있습니다. 그러면 `Some`이 있으면 값을 출력하고, `None`이 있으면 건드리지 않을 수 있습니다. 예를 들어:

```rust
fn take_fifth(value: Vec<i32>) -> Option<i32> {
    if value.len() < 5 {
        None
    } else {
        Some(value[4])
    }
}

fn handle_option(my_option: Vec<Option<i32>>) {
  for item in my_option {
    match item {
      Some(number) => println!("{}를 찾았습니다!", number),
      None => println!("None을 찾았습니다!"),
    }
  }
}

fn main() {
    let new_vec = vec![1, 2];
    let bigger_vec = vec![1, 2, 3, 4, 5];
    let mut option_vec = Vec::new(); // Option들을 담을 새로운 벡터를 만듭니다
                                     // 벡터의 타입은: Vec<Option<i32>>입니다. Option<i32>의 벡터라는 뜻입니다.

    option_vec.push(take_fifth(new_vec)); // 이것은 "None"을 벡터에 푸시합니다
    option_vec.push(take_fifth(bigger_vec)); // 이것은 "Some(5)"를 벡터에 푸시합니다

    handle_option(option_vec); // handle_option은 벡터의 모든 옵션을 봅니다.
                               // Some이면 값을 출력합니다. None이면 건드리지 않습니다.
}
```

이것은 다음을 출력합니다:

```text
None을 찾았습니다!
5를 찾았습니다!
```

제네릭을 알고 있기 때문에, `Option`의 코드를 읽을 수 있습니다. 다음과 같이 생겼습니다:

```rust
enum Option<T> {
    None,
    Some(T),
}

fn main() {}
```

기억해야 할 중요한 점: `Some`에서는 타입 `T`의 값을 가집니다(어떤 타입이든). 또한 `enum` 이름 뒤의 `T` 주위의 꺾쇠 괄호가 컴파일러에게 제네릭이라고 알려주는 것입니다. `Display`나 다른 것 같은 트레이트가 없어서 제한이 없으므로, 어떤 것이든 될 수 있습니다. 하지만 `None`에서는 아무것도 가지지 않습니다.

따라서 Option에 대한 `match` 문에서는 다음과 같이 말할 수 없습니다:

```rust
// 🚧
Some(value) => println!("값은 {}입니다", value),
None(value) => println!("값은 {}입니다", value),
```

`None`은 그냥 `None`이기 때문입니다.

물론 Option을 사용하는 더 쉬운 방법들이 있습니다. 이 코드에서는 `Some`인지 알려주는 `.is_some()`이라는 메서드를 사용할 것입니다. (네, `.is_none()`이라는 메서드도 있습니다.) 이 더 쉬운 방법에서는 더 이상 `handle_option()`이 필요 없습니다. Option들을 위한 벡터도 필요 없습니다.

```rust
fn take_fifth(value: Vec<i32>) -> Option<i32> {
    if value.len() < 5 {
        None
    } else {
        Some(value[4])
    }
}

fn main() {
    let new_vec = vec![1, 2];
    let bigger_vec = vec![1, 2, 3, 4, 5];
    let vec_of_vecs = vec![new_vec, bigger_vec];
    for vec in vec_of_vecs {
        let inside_number = take_fifth(vec);
        if inside_number.is_some() {
            // .is_some()은 Some을 얻으면 true를, None을 얻으면 false를 반환합니다
            println!("얻은 값: {}", inside_number.unwrap()); // 이미 확인했으므로 이제 .unwrap()을 사용하는 것이 안전합니다
        } else {
            println!("아무것도 얻지 못했습니다.");
        }
    }
}
```

이것은 다음을 출력합니다:

```text
아무것도 얻지 못했습니다.
얻은 값: 5
```

### Result

Result는 Option과 비슷하지만, 차이점이 있습니다:

- Option은 `Some` 또는 `None`에 관한 것입니다 (값 또는 값 없음),
- Result는 `Ok` 또는 `Err`에 관한 것입니다 (정상 결과 또는 에러 결과).

따라서 `Option`은 "뭔가 있을 수도 있고, 없을 수도 있어"라고 생각할 때입니다. 하지만 `Result`는 "실패할 수도 있어"라고 생각할 때입니다.

비교하기 위해, Option과 Result의 시그니처를 보겠습니다.

```rust
enum Option<T> {
    None,
    Some(T),
}

enum Result<T, E> {
    Ok(T),
    Err(E),
}

fn main() {}
```

따라서 Result는 `Ok` 안에 값을 가지고, `Err` 안에도 값을 가집니다. 에러는 보통 에러를 설명하는 정보를 포함하기 때문입니다.

`Result<T, E>`는 `Ok`에 대해 무엇을 반환할지, `Err`에 대해 무엇을 반환할지 생각해야 한다는 뜻입니다. 실제로는, 어떤 것이든 결정할 수 있습니다. 이것도 괜찮습니다:

```rust
fn check_error() -> Result<(), ()> {
    Ok(())
}

fn main() {
    check_error();
}
```

`check_error`는 "`Ok`를 얻으면 `()`를 반환하고, `Err`를 얻으면 `()`를 반환해"라고 말합니다. 그리고 `()`와 함께 `Ok`를 반환합니다.

컴파일러가 흥미로운 경고를 줍니다:

```text
warning: unused `std::result::Result` that must be used
 --> src\main.rs:6:5
  |
6 |     check_error();
  |     ^^^^^^^^^^^^^^
  |
  = note: `#[warn(unused_must_use)]` on by default
  = note: this `Result` may be an `Err` variant, which should be handled
```

이것이 맞습니다: 단지 `Result`를 반환했지만 `Err`일 수도 있었습니다. 따라서 여전히 실제로는 아무것도 하지 않지만, 에러를 좀 처리해보겠습니다.

```rust
fn give_result(input: i32) -> Result<(), ()> {
    if input % 2 == 0 {
        return Ok(())
    } else {
        return Err(())
    }
}

fn main() {
    if give_result(5).is_ok() {
        println!("괜찮아요, 여러분")
    } else {
        println!("에러에요, 여러분")
    }
}
```

이것은 `에러에요, 여러분`을 출력합니다. 따라서 우리는 첫 번째 에러를 처리했습니다.

기억하세요, 쉽게 확인하는 네 가지 메서드는 `.is_some()`, `is_none()`, `is_ok()`, 그리고 `is_err()`입니다.

때로는 Result가 있는 함수가 `Err` 값에 `String`을 사용할 것입니다. 이것이 사용하기 가장 좋은 방법은 아니지만, 지금까지 우리가 한 것보다는 조금 낫습니다.

```rust
fn check_if_five(number: i32) -> Result<i32, String> {
    match number {
        5 => Ok(number),
        _ => Err("죄송합니다, 숫자가 5가 아니었습니다.".to_string()), // 이것이 우리의 에러 메시지입니다
    }
}

fn main() {
    let mut result_vec = Vec::new(); // 결과들을 위한 새로운 벡터를 만듭니다

    for number in 2..7 {
        result_vec.push(check_if_five(number)); // 각 결과를 벡터에 푸시합니다
    }

    println!("{:?}", result_vec);
}
```

우리의 벡터는 다음을 출력합니다:

```text
[Err("죄송합니다, 숫자가 5가 아니었습니다."), Err("죄송합니다, 숫자가 5가 아니었습니다."), Err("죄송합니다, 숫자가 5가 아니었습니다."), Ok(5),
Err("죄송합니다, 숫자가 5가 아니었습니다.")]
```

Option과 마찬가지로, `Err`에서 `.unwrap()`하면 패닉이 발생합니다.

```rust
    // ⚠️
fn main() {
    let error_value: Result<i32, &str> = Err("에러가 있었습니다"); // 이미 Err인 Result를 만듭니다
    println!("{}", error_value.unwrap()); // Unwrap합니다
}
```

프로그램이 패닉하며, 다음을 출력합니다:

```text
thread 'main' panicked at 'called `Result::unwrap()` on an `Err` value: "에러가 있었습니다"', src\main.rs:30:20
```

이 정보는 코드를 수정하는 데 도움이 됩니다. `src\main.rs:30:20`은 "src 디렉토리의 main.rs에서, 30번째 줄과 20번째 열에서"를 의미합니다. 따라서 거기로 가서 코드를 보고 문제를 수정할 수 있습니다.

자신만의 에러 타입을 만들 수도 있습니다. 표준 라이브러리의 Result 함수들과 다른 사람들의 코드는 보통 이렇게 합니다. 예를 들어, 표준 라이브러리의 이 함수:

```rust
// 🚧
pub fn from_utf8(vec: Vec<u8>) -> Result<String, FromUtf8Error>
```

이 함수는 바이트 벡터(`u8`)를 받아서 `String`을 만들려고 시도합니다. 따라서 Result의 성공 케이스는 `String`이고 에러 케이스는 `FromUtf8Error`입니다. 에러 타입에 원하는 어떤 이름이든 줄 수 있습니다.

`Option`과 `Result`와 함께 `match`를 사용하는 것은 때때로 많은 코드가 필요합니다. 예를 들어, `.get()` 메서드는 `Vec`에서 `Option`을 반환합니다.

```rust
fn main() {
    let my_vec = vec![2, 3, 4];
    let get_one = my_vec.get(0); // 0으로 첫 번째 숫자를 얻습니다
    let get_two = my_vec.get(10); // None을 반환합니다
    println!("{:?}", get_one);
    println!("{:?}", get_two);
}
```

이것은 다음을 출력합니다

```text
Some(2)
None
```

이제 match를 사용해서 값들을 얻을 수 있습니다. 0부터 10까지의 범위를 사용해서 `my_vec`의 숫자들과 매치되는지 보겠습니다.

```rust
fn main() {
    let my_vec = vec![2, 3, 4];

    for index in 0..10 {
      match my_vec.get(index) {
        Some(number) => println!("숫자는: {}", number),
        None => {}
      }
    }
}
```

이것은 좋지만, 신경쓰지 않기 때문에 `None`에 대해서는 아무것도 하지 않습니다. 여기서는 `if let`을 사용해서 코드를 작게 만들 수 있습니다. `if let`은 "매치되면 뭔가 하고, 매치되지 않으면 아무것도 하지 마"라는 뜻입니다. `if let`은 모든 것에 대해 매치하는 것을 신경쓰지 않을 때입니다.

```rust
fn main() {
    let my_vec = vec![2, 3, 4];

    for index in 0..10 {
      if let Some(number) = my_vec.get(index) {
        println!("숫자는: {}", number);
      }
    }
}
```

**기억해야 할 중요한 점**: `if let Some(number) = my_vec.get(index)`는 "`my_vec.get(index)`에서 `Some(number)`를 얻으면"이라는 뜻입니다.

또한 주목하세요: `=`을 하나 사용합니다. 불린이 아닙니다.

`while let`은 `if let`에 대한 while 루프와 같습니다. 다음과 같은 날씨 관측소 데이터가 있다고 상상해보세요:

```text
["Berlin", "cloudy", "5", "-7", "78"]
["Athens", "sunny", "not humid", "20", "10", "50"]
```

우리는 단어가 아닌 숫자를 얻고 싶습니다. 숫자의 경우, `parse::<i32>()`라는 메서드를 사용할 수 있습니다. `parse()`는 메서드이고, `::<i32>`는 타입입니다. `&str`을 `i32`로 바꾸려고 시도하고, 가능하면 우리에게 줄 것입니다. `Result`를 반환하는데, 동작하지 않을 수도 있기 때문입니다 (예를 들어 "Billybrobby"를 파싱하려고 한다면 - 그것은 숫자가 아닙니다).

`.pop()`도 사용할 것입니다. 이것은 벡터에서 마지막 아이템을 제거합니다.

```rust
fn main() {
    let weather_vec = vec![
        vec!["Berlin", "cloudy", "5", "-7", "78"],
        vec!["Athens", "sunny", "not humid", "20", "10", "50"],
    ];
    for mut city in weather_vec {
        println!("도시 {}에 대해:", city[0]); // 우리 데이터에서, 모든 첫 번째 아이템은 도시 이름입니다
        while let Some(information) = city.pop() {
            // 이것은 의미합니다: 더 이상 pop할 수 없을 때까지 계속하세요
            // 벡터가 0개 아이템에 도달하면, None을 반환할 것이고
            // 멈출 것입니다.
            if let Ok(number) = information.parse::<i32>() {
                // information이라고 부른 변수를 파싱해보세요
                // 이것은 결과를 반환합니다. Ok(number)이면, 출력할 것입니다
                println!("숫자는: {}", number);
            }  // 에러를 얻으면 아무것도 하지 않기 때문에 여기에는 아무것도 쓰지 않습니다. 모든 에러를 버립니다
        }
    }
}
```

이것은 다음을 출력할 것입니다:

```text
도시 Berlin에 대해:
숫자는: 78
숫자는: -7
숫자는: 5
도시 Athens에 대해:
숫자는: 50
숫자는: 10
숫자는: 20
```

## 다른 컬렉션들

Rust에는 훨씬 더 많은 타입의 컬렉션들이 있습니다. 표준 라이브러리의 https://doc.rust-lang.org/beta/std/collections/ 에서 볼 수 있습니다. 그 페이지에는 어떤 타입을 사용해야 하는지에 대한 좋은 설명이 있으므로, 어떤 타입을 원하는지 모르겠다면 그곳으로 가보세요. 이 컬렉션들은 모두 표준 라이브러리의 `std::collections` 안에 있습니다. 그것들을 사용하는 가장 좋은 방법은 우리가 `enums`에서 했던 것처럼 `use` 문을 사용하는 것입니다. 우리는 매우 일반적인 `HashMap`부터 시작하겠습니다.

### HashMap (그리고 BTreeMap)

HashMap은 *키*와 *값*으로 만들어진 컬렉션입니다. 키를 사용해서 키와 일치하는 값을 찾습니다. 그냥 `HashMap::new()`로 새로운 `HashMap`을 만들 수 있고 `.insert(key, value)`를 사용해서 아이템을 삽입할 수 있습니다.

`HashMap`은 순서가 없으므로, `HashMap`의 모든 키를 함께 출력하면 아마도 다르게 출력될 것입니다. 이것을 예시에서 볼 수 있습니다:

```rust
use std::collections::HashMap; // 이렇게 하면 매번 std::collections::HashMap 대신 HashMap만 쓸 수 있습니다

struct City {
    name: String,
    population: HashMap<u32, u32>, // 이것은 연도와 그 연도의 인구를 가질 것입니다
}

fn main() {

    let mut tallinn = City {
        name: "Tallinn".to_string(),
        population: HashMap::new(), // 지금까지 HashMap은 비어있습니다
    };

    tallinn.population.insert(1372, 3_250); // 세 개의 날짜를 삽입합니다
    tallinn.population.insert(1851, 24_000);
    tallinn.population.insert(2020, 437_619);


    for (year, population) in tallinn.population { // HashMap은 HashMap<u32, u32>이므로 매번 두 아이템을 반환합니다
        println!("In the year {} the city of {} had a population of {}.", year, tallinn.name, population);
    }
}
```

이것은 다음을 출력합니다:

```text
In the year 1372 the city of Tallinn had a population of 3250.
In the year 2020 the city of Tallinn had a population of 437619.
In the year 1851 the city of Tallinn had a population of 24000.
```

또는 다음을 출력할 수도 있습니다:

```text
In the year 1851 the city of Tallinn had a population of 24000.
In the year 2020 the city of Tallinn had a population of 437619.
In the year 1372 the city of Tallinn had a population of 3250.
```

순서가 없다는 것을 볼 수 있습니다.

정렬할 수 있는 `HashMap`을 원한다면, `BTreeMap`을 사용할 수 있습니다. 실제로 그들은 서로 매우 비슷하므로, 우리는 빠르게 `HashMap`을 `BTreeMap`으로 바꿔서 볼 수 있습니다. 거의 같은 코드라는 것을 볼 수 있습니다.

```rust
use std::collections::BTreeMap; // HashMap을 BTreeMap으로 바꾸기만 하면 됩니다

struct City {
    name: String,
    population: BTreeMap<u32, u32>, // HashMap을 BTreeMap으로 바꾸기만 하면 됩니다
}

fn main() {

    let mut tallinn = City {
        name: "Tallinn".to_string(),
        population: BTreeMap::new(), // HashMap을 BTreeMap으로 바꾸기만 하면 됩니다
    };

    tallinn.population.insert(1372, 3_250);
    tallinn.population.insert(1851, 24_000);
    tallinn.population.insert(2020, 437_619);

    for (year, population) in tallinn.population {
        println!("In the year {} the city of {} had a population of {}.", year, tallinn.name, population);
    }
}
```

이제 항상 다음을 출력할 것입니다:

```text
In the year 1372 the city of Tallinn had a population of 3250.
In the year 1851 the city of Tallinn had a population of 24000.
In the year 2020 the city of Tallinn had a population of 437619.
```

이제 우리는 `HashMap`으로 돌아가겠습니다.

키를 `[]` 대괄호에 넣기만 하면 `HashMap`에서 값을 얻을 수 있습니다. 다음 예시에서 우리는 키 `Bielefeld`의 값을 가져올 것인데, 그것은 `Germany`입니다. 하지만 조심하세요, 키가 없으면 프로그램이 충돌할 것입니다. 예를 들어 `println!("{:?}", city_hashmap["Bielefeldd"]);`라고 쓰면 충돌할 것인데, `Bielefeldd`는 존재하지 않기 때문입니다.

키가 있을지 확실하지 않다면, `Option`을 반환하는 `.get()`을 사용할 수 있습니다. 존재한다면 `Some(value)`일 것이고, 그렇지 않다면 프로그램을 충돌시키는 대신 `None`을 얻을 것입니다. 그래서 `.get()`이 `HashMap`에서 값을 얻는 더 안전한 방법입니다.

```rust
use std::collections::HashMap;

fn main() {
    let canadian_cities = vec!["Calgary", "Vancouver", "Gimli"];
    let german_cities = vec!["Karlsruhe", "Bad Doberan", "Bielefeld"];

    let mut city_hashmap = HashMap::new();

    for city in canadian_cities {
        city_hashmap.insert(city, "Canada");
    }
    for city in german_cities {
        city_hashmap.insert(city, "Germany");
    }

    println!("{:?}", city_hashmap["Bielefeld"]);
    println!("{:?}", city_hashmap.get("Bielefeld"));
    println!("{:?}", city_hashmap.get("Bielefeldd"));
}
```

이것은 다음을 출력합니다:

```text
"Germany"
Some("Germany")
None
```

이것은 *Bielefeld*는 존재하지만, *Bielefeldd*는 존재하지 않기 때문입니다.

`HashMap`에 키를 넣으려고 할 때 이미 키가 있다면, 그 값을 덮어쓸 것입니다:

```rust
use std::collections::HashMap;

fn main() {
    let mut book_hashmap = HashMap::new();

    book_hashmap.insert(1, "L'Allemagne Moderne");
    book_hashmap.insert(1, "Le Petit Prince");
    book_hashmap.insert(1, "섀도우 오브 유어 스마일");
    book_hashmap.insert(1, "Eye of the World");

    println!("{:?}", book_hashmap.get(&1));
}
```

이것은 `Some("Eye of the World")`를 출력하는데, 그것이 `.insert()`를 마지막으로 사용한 것이기 때문입니다.

엔트리가 존재하는지 확인하는 것은 쉽습니다. `Option`을 주는 `.get()`으로 확인할 수 있기 때문입니다:

```rust
use std::collections::HashMap;

fn main() {
    let mut book_hashmap = HashMap::new();

    book_hashmap.insert(1, "L'Allemagne Moderne");

    if book_hashmap.get(&1).is_none() { // is_none()은 bool을 반환합니다: None이면 true, Some이면 false
        book_hashmap.insert(1, "Le Petit Prince");
    }

    println!("{:?}", book_hashmap.get(&1));
}
```

이것은 `Some("L\'Allemagne Moderne")`를 출력하는데, `1`에 대한 키가 이미 있었으므로 `Le Petit Prince`를 삽입하지 않았기 때문입니다.

`HashMap`에는 `.entry()`라는 매우 흥미로운 메서드가 있는데, 확실히 시도해보고 싶을 것입니다. 이것으로 엔트리를 만들려고 시도할 수 있고 키가 없다면 값을 삽입하는 `.or_insert()`와 같은 다른 메서드를 사용할 수 있습니다. 흥미로운 부분은 가변 참조도 주므로 원한다면 바꿀 수 있다는 것입니다. 책 제목을 `HashMap`에 삽입할 때마다 그냥 `true`를 삽입하는 예시부터 시작하겠습니다.

도서관이 있고 우리 책들을 추적하고 싶다고 가정해봅시다.

```rust
use std::collections::HashMap;

fn main() {
    let book_collection = vec!["L'Allemagne Moderne", "Le Petit Prince", "Eye of the World", "Eye of the World"]; // Eye of the World가 두 번 나타납니다

    let mut book_hashmap = HashMap::new();

    for book in book_collection {
        book_hashmap.entry(book).or_insert(true);
    }
    for (book, true_or_false) in book_hashmap {
        println!("Do we have {}? {}", book, true_or_false);
    }
}
```

이것은 다음을 출력합니다:

```text
Do we have Eye of the World? true
Do we have Le Petit Prince? true
Do we have L'Allemagne Moderne? true
```

하지만 그것은 정확히 우리가 원하는 것이 아닙니다. 아마도 *Eye of the World*의 복사본이 두 개 있다는 것을 알 수 있도록 책의 수를 세는 것이 더 나을 것입니다. 먼저 `.entry()`가 무엇을 하는지, 그리고 `.or_insert()`가 무엇을 하는지 봅시다. `.entry()`는 실제로 `Entry`라는 `enum`을 반환합니다:

```rust
pub fn entry(&mut self, key: K) -> Entry<K, V> // 🚧
```

[여기가 Entry 페이지입니다](https://doc.rust-lang.org/std/collections/hash_map/enum.Entry.html). 여기 그 코드의 간단한 버전이 있습니다. `K`는 키를 의미하고 `V`는 값을 의미합니다.

```rust
// 🚧
use std::collections::hash_map::*;

enum Entry<K, V> {
    Occupied(OccupiedEntry<K, V>),
    Vacant(VacantEntry<K, V>),
}
```

그러면 `.or_insert()`를 호출할 때, enum을 보고 무엇을 할지 결정합니다.

```rust
fn or_insert(self, default: V) -> &mut V { // 🚧
    match self {
        Occupied(entry) => entry.into_mut(),
        Vacant(entry) => entry.insert(default),
    }
}
```

흥미로운 부분은 `mut` 참조를 반환한다는 것입니다: `&mut V`. 이것은 `let`을 사용해서 변수에 붙일 수 있고, 변수를 바꿔서 `HashMap`의 값을 바꿀 수 있다는 뜻입니다. 그래서 모든 책에 대해 엔트리가 없다면 0을 삽입할 것입니다. 그리고 있다면, 참조에 `+= 1`을 사용해서 숫자를 증가시킬 것입니다. 이제 이렇게 보입니다:

```rust
use std::collections::HashMap;

fn main() {
    let book_collection = vec!["L'Allemagne Moderne", "Le Petit Prince", "Eye of the World", "Eye of the World"];

    let mut book_hashmap = HashMap::new();

    for book in book_collection {
        let return_value = book_hashmap.entry(book).or_insert(0); // return_value는 가변 참조입니다. 아무것도 없다면, 0이 될 것입니다
        *return_value +=1; // 이제 return_value는 최소 1입니다. 그리고 다른 책이 있었다면, 1씩 올라갈 것입니다
    }

    for (book, number) in book_hashmap {
        println!("{}, {}", book, number);
    }
}
```

중요한 부분은 `let return_value = book_hashmap.entry(book).or_insert(0);`입니다. `let`을 빼면, `book_hashmap.entry(book).or_insert(0)`가 됩니다. `let` 없이는 아무것도 하지 않습니다: 0을 삽입하고, 아무도 0에 대한 가변 참조를 가져가지 않습니다. 그래서 우리는 그것을 `return_value`에 바인드해서 0을 유지할 수 있습니다. 그러면 값을 1 증가시키는데, 이것은 `HashMap`의 모든 책에 대해 최소 1을 줍니다. 그러면 `.entry()`가 *Eye of the World*를 다시 볼 때 아무것도 삽입하지 않지만, 가변 1을 줍니다. 그러면 우리는 그것을 2로 증가시키고, 그래서 이것을 출력합니다:

```text
L'Allemagne Moderne, 1
Le Petit Prince, 1
Eye of the World, 2
```

또한 vec을 삽입하고 그 vec에 push하는 것과 같은 일들을 `.or_insert()`로 할 수 있습니다. 거리에서 남자와 여자에게 정치인에 대해 어떻게 생각하는지 물어봤다고 가정해봅시다. 그들은 0부터 10까지의 점수를 줍니다. 그러면 우리는 숫자들을 함께 모아서 그 정치인이 남자들에게 더 인기가 있는지 여자들에게 더 인기가 있는지 보고 싶습니다. 이렇게 보일 수 있습니다:

```rust
use std::collections::HashMap;

fn main() {
    let data = vec![ // 이것은 원시 데이터입니다
        ("male", 9),
        ("female", 5),
        ("male", 0),
        ("female", 6),
        ("female", 5),
        ("male", 10),
    ];

    let mut survey_hash = HashMap::new();

    for item in data { // 이것은 (&str, i32)의 튜플을 줍니다
        survey_hash.entry(item.0).or_insert(Vec::new()).push(item.1); // 이것은 숫자를 안의 Vec에 push합니다
    }

    for (male_or_female, numbers) in survey_hash {
        println!("{:?}: {:?}", male_or_female, numbers);
    }
}
```

이것은 다음을 출력합니다:

```text
"female", [5, 6, 5]
"male", [9, 0, 10]
```

중요한 줄은: `survey_hash.entry(item.0).or_insert(Vec::new()).push(item.1);`입니다. 그래서 "female"을 보면 `HashMap`에 "female"이 이미 있는지 확인할 것입니다. 없다면, `Vec::new()`를 삽입하고, 그 다음 숫자를 push할 것입니다. `HashMap`에 "female"이 이미 있다면, 새로운 Vec을 삽입하지 않고, 그냥 숫자를 그 안에 push할 것입니다.

### HashSet과 BTreeSet

`HashSet`은 실제로는 키만 있는 `HashMap`입니다. [HashSet 페이지](https://doc.rust-lang.org/std/collections/struct.HashSet.html)에서 맨 위에 이것을 설명합니다:

`A hash set implemented as a HashMap where the value is ().` 그래서 그것은 키가 있고 값이 없는 `HashMap`입니다.

키가 존재하는지, 존재하지 않는지만 알고 싶을 때 `HashSet`을 자주 사용합니다.

1부터 100까지의 100개의 랜덤 숫자가 있다고 상상해보세요. 이렇게 하면, 어떤 숫자들은 한 번 이상 나타날 것이고, 어떤 것들은 전혀 나타나지 않을 것입니다. 그것들을 `HashSet`에 넣으면 나타난 모든 숫자들의 목록을 갖게 될 것입니다.

```rust
use std::collections::HashSet;

fn main() {
    let many_numbers = vec![
        94, 42, 59, 64, 32, 22, 38, 5, 59, 49, 15, 89, 74, 29, 14, 68, 82, 80, 56, 41, 36, 81, 66,
        51, 58, 34, 59, 44, 19, 93, 28, 33, 18, 46, 61, 76, 14, 87, 84, 73, 71, 29, 94, 10, 35, 20,
        35, 80, 8, 43, 79, 25, 60, 26, 11, 37, 94, 32, 90, 51, 11, 28, 76, 16, 63, 95, 13, 60, 59,
        96, 95, 55, 92, 28, 3, 17, 91, 36, 20, 24, 0, 86, 82, 58, 93, 68, 54, 80, 56, 22, 67, 82,
        58, 64, 80, 16, 61, 57, 14, 11];

    let mut number_hashset = HashSet::new();

    for number in many_numbers {
        number_hashset.insert(number);
    }

    let hashset_length = number_hashset.len(); // 길이는 그 안에 몇 개의 숫자가 있는지 알려줍니다
    println!("There are {} unique numbers, so we are missing {}.", hashset_length, 100 - hashset_length);

    // 누락된 숫자들을 봅시다
    let mut missing_vec = vec![];
    for number in 0..100 {
        if number_hashset.get(&number).is_none() { // .get()이 None을 반환하면,
            missing_vec.push(number);
        }
    }

    print!("It does not contain: ");
    for number in missing_vec {
        print!("{} ", number);
    }
}
```

이것은 다음을 출력합니다:

```text
There are 66 unique numbers, so we are missing 34.
It does not contain: 1 2 4 6 7 9 12 21 23 27 30 31 39 40 45 47 48 50 52 53 62 65 69 70 72 75 77 78 83 85 88 97 98 99
```

`BTreeSet`은 `BTreeMap`이 `HashMap`과 비슷한 것처럼 `HashSet`과 비슷합니다. `HashSet`에서 각 아이템을 출력하면, 순서가 무엇인지 모릅니다:

```rust
for entry in number_hashset { // 🚧
    print!("{} ", entry);
}
```

아마도 이것을 출력할 것입니다: `67 28 42 25 95 59 87 11 5 81 64 34 8 15 13 86 10 89 63 93 49 41 46 57 60 29 17 22 74 43 32 38 36 76 71 18 14 84 61 16 35 90 56 54 91 19 94 44 3 0 68 80 51 92 24 20 82 26 58 33 55 96 37 66 79 73`. 하지만 거의 절대로 같은 방식으로 다시 출력하지 않을 것입니다.

여기서도, 순서가 필요하다고 결정하면 `HashSet`을 `BTreeSet`으로 바꾸는 것은 쉽습니다. 우리 코드에서, `HashSet`에서 `BTreeSet`으로 바꾸기 위해 두 곳만 바꾸면 됩니다.

```rust
use std::collections::BTreeSet; // HashSet을 BTreeSet으로 바꾸기

fn main() {
    let many_numbers = vec![
        94, 42, 59, 64, 32, 22, 38, 5, 59, 49, 15, 89, 74, 29, 14, 68, 82, 80, 56, 41, 36, 81, 66,
        51, 58, 34, 59, 44, 19, 93, 28, 33, 18, 46, 61, 76, 14, 87, 84, 73, 71, 29, 94, 10, 35, 20,
        35, 80, 8, 43, 79, 25, 60, 26, 11, 37, 94, 32, 90, 51, 11, 28, 76, 16, 63, 95, 13, 60, 59,
        96, 95, 55, 92, 28, 3, 17, 91, 36, 20, 24, 0, 86, 82, 58, 93, 68, 54, 80, 56, 22, 67, 82,
        58, 64, 80, 16, 61, 57, 14, 11];

    let mut number_btreeset = BTreeSet::new(); // HashSet을 BTreeSet으로 바꾸기

    for number in many_numbers {
        number_btreeset.insert(number);
    }
    for entry in number_btreeset {
        print!("{} ", entry);
    }
}
```

이제 항상 순서대로 출력할 것입니다: `0 3 5 8 10 11 13 14 15 16 17 18 19 20 22 24 25 26 28 29 32 33 34 35 36 37 38 41 42 43 44 46 49 51 54 55 56 57 58 59 60 61 63 64 66 67 68 71 73 74 76 79 80 81 82 84 86 87 89 90 91 92 93 94 95 96`.

### BinaryHeap

`BinaryHeap`는 흥미로운 컬렉션 타입인데, 대부분 순서가 없지만 약간의 순서가 있기 때문입니다. 가장 큰 아이템을 앞에 유지하지만, 다른 아이템들은 아무 순서나 됩니다.

예시를 위해 다른 아이템 목록을 사용하겠지만, 이번에는 더 작게 하겠습니다.

```rust
use std::collections::BinaryHeap;

fn show_remainder(input: &BinaryHeap<i32>) -> Vec<i32> { // 이 함수는 BinaryHeap의 나머지를 보여줍니다. 실제로는 iterator가
                                                         // 함수보다 빠를 것입니다 - 나중에 배우겠습니다.
    let mut remainder_vec = vec![];
    for number in input {
        remainder_vec.push(*number)
    }
    remainder_vec
}

fn main() {
    let many_numbers = vec![0, 5, 10, 15, 20, 25, 30]; // 이 숫자들은 순서대로 있습니다

    let mut my_heap = BinaryHeap::new();

    for number in many_numbers {
        my_heap.push(number);
    }

    while let Some(number) = my_heap.pop() { // .pop()은 숫자가 있으면 Some(number)를, 없으면 None을 반환합니다. 앞에서부터 pop합니다
        println!("Popped off {}. Remaining numbers are: {:?}", number, show_remainder(&my_heap));
    }
}
```

이것은 다음을 출력합니다:

```text
Popped off 30. Remaining numbers are: [25, 15, 20, 0, 10, 5]
Popped off 25. Remaining numbers are: [20, 15, 5, 0, 10]
Popped off 20. Remaining numbers are: [15, 10, 5, 0]
Popped off 15. Remaining numbers are: [10, 0, 5]
Popped off 10. Remaining numbers are: [5, 0]
Popped off 5. Remaining numbers are: [0]
Popped off 0. Remaining numbers are: []
```

0 인덱스의 숫자가 항상 가장 크다는 것을 볼 수 있습니다: 25, 20, 15, 10, 5, 그리고 0. 하지만 다른 것들은 모두 다릅니다.

`BinaryHeap`을 사용하는 좋은 방법은 할 일들의 컬렉션을 위한 것입니다. 여기서 우리는 `BinaryHeap<(u8, &str)>`을 만드는데, `u8`은 작업의 중요도를 위한 숫자입니다. `&str`은 무엇을 할지에 대한 설명입니다.

```rust
use std::collections::BinaryHeap;

fn main() {
    let mut jobs = BinaryHeap::new();

    // 하루 종일 할 일들을 추가합니다
    jobs.push((100, "Write back to email from the CEO"));
    jobs.push((80, "Finish the report today"));
    jobs.push((5, "Watch some YouTube"));
    jobs.push((70, "Tell your team members thanks for always working hard"));
    jobs.push((30, "Plan who to hire next for the team"));

    while let Some(job) = jobs.pop() {
        println!("You need to: {}", job.1);
    }
}
```

이것은 항상 다음을 출력할 것입니다:

```text
You need to: Write back to email from the CEO
You need to: Finish the report today
You need to: Tell your team members thanks for always working hard
You need to: Plan who to hire next for the team
You need to: Watch some YouTube
```

### VecDeque

`VecDeque`는 앞과 뒤 둘 다에서 아이템을 pop하는 데 좋은 `Vec`입니다. Rust가 `VecDeque`를 가지고 있는 이유는 `Vec`은 뒤에서(마지막 아이템) pop하는 데는 훌륭하지만 앞에서는 그렇지 않기 때문입니다. `Vec`에서 `.pop()`을 사용하면, 그냥 오른쪽의 마지막 아이템을 제거하고 다른 것은 아무것도 움직이지 않습니다. 하지만 다른 부분에서 제거한다면, 오른쪽의 모든 아이템들이 왼쪽으로 한 위치씩 이동합니다. `.remove()`에 대한 설명에서 이것을 볼 수 있습니다:

```text
Removes and returns the element at position index within the vector, shifting all elements after it to the left.
```

그래서 이렇게 한다면:

```rust
fn main() {
    let mut my_vec = vec![9, 8, 7, 6, 5];
    my_vec.remove(0);
}
```

`9`를 제거할 것입니다. 인덱스 1의 `8`이 인덱스 0으로 이동하고, 인덱스 2의 `7`이 인덱스 1로 이동하는 식으로 계속됩니다. 한 대의 차가 떠날 때마다 오른쪽의 모든 차들이 이동해야 하는 큰 주차장을 상상해보세요.

예를 들어, 이것은 컴퓨터에게 *많은* 작업입니다. 실제로, Playground에서 실행하면 너무 많은 작업이어서 아마도 포기할 것입니다.

```rust
fn main() {
    let mut my_vec = vec![0; 600_000];
    for i in 0..600000 {
        my_vec.remove(0);
    }
}
```

이것은 600,000개의 0으로 이루어진 `Vec`입니다. `remove(0)`을 사용할 때마다, 각 0을 왼쪽으로 한 칸씩 이동시킵니다. 그리고 그것을 600,000번 합니다.

`VecDeque`로는 그것에 대해 걱정할 필요가 없습니다. 보통 `Vec`보다 약간 느리지만, 양쪽 끝에서 일을 해야 한다면 훨씬 빠릅니다. `Vec`로 `VecDeque::from`을 사용해서 하나를 만들 수 있습니다. 위의 우리 코드는 이렇게 보입니다:

```rust
use std::collections::VecDeque;

fn main() {
    let mut my_vec = VecDeque::from(vec![0; 600000]);
    for i in 0..600000 {
        my_vec.pop_front(); // pop_front는 .pop과 비슷하지만 앞을 위한 것입니다
    }
}
```

이제 훨씬 빠르고, Playground에서 포기하는 대신 1초 미만에 끝납니다.

다음 예시에서 우리는 할 일들의 `Vec`을 가지고 있습니다. 그러면 `VecDeque`를 만들고 `.push_front()`를 사용해서 그것들을 앞에 넣으므로, 우리가 추가한 첫 번째 아이템이 오른쪽에 있을 것입니다. 하지만 우리가 push하는 각 아이템은 `(&str, bool)`입니다: `&str`은 설명이고 `false`는 아직 끝나지 않았다는 뜻입니다. 우리는 `done()` 함수를 사용해서 뒤에서 아이템을 pop하지만, 그것을 삭제하고 싶지 않습니다. 대신, 우리는 `false`를 `true`로 바꾸고 그것을 앞에 push해서 유지할 수 있습니다.

이렇게 보입니다:

```rust
use std::collections::VecDeque;

fn check_remaining(input: &VecDeque<(&str, bool)>) { // 각 아이템은 (&str, bool)입니다
    for item in input {
        if item.1 == false {
            println!("You must: {}", item.0);
        }
    }
}

fn done(input: &mut VecDeque<(&str, bool)>) {
    let mut task_done = input.pop_back().unwrap(); // 뒤에서 pop합니다
    task_done.1 = true;                            // 이제 끝났습니다 - true로 표시합니다
    input.push_front(task_done);                   // 이제 앞에 넣습니다
}

fn main() {
    let mut my_vecdeque = VecDeque::new();
    let things_to_do = vec!["send email to customer", "add new product to list", "phone Loki back"];

    for thing in things_to_do {
        my_vecdeque.push_front((thing, false));
    }

    done(&mut my_vecdeque);
    done(&mut my_vecdeque);

    check_remaining(&my_vecdeque);

    for task in my_vecdeque {
        print!("{:?} ", task);
    }
}
```

이것은 다음을 출력합니다:

```text
You must: phone Loki back
("add new product to list", true) ("send email to customer", true) ("phone Loki back", false)
```

## ? 연산자

`Result` (그리고 `Option`)를 다루는 더 짧은 방법이 있습니다. `match`보다도 짧고 `if let`보다도 짧습니다. 그것은 "물음표 연산자"라고 불리고, 그냥 `?`입니다. result를 반환하는 함수 뒤에 `?`를 추가할 수 있습니다. 이것은 다음을 할 것입니다:

- `Ok`라면 `Result` 안의 내용을 반환합니다
- `Err`라면 에러를 다시 전달합니다

다른 말로, 거의 모든 것을 당신을 위해 합니다.

`.parse()`로 이것을 다시 시도해볼 수 있습니다. `&str`을 `i32`로 바꾸려고 시도하는 `parse_str`이라는 함수를 작성하겠습니다. 이렇게 보입니다:

```rust
use std::num::ParseIntError;

fn parse_str(input: &str) -> Result<i32, ParseIntError> {
    let parsed_number = input.parse::<i32>()?; // 여기가 물음표입니다
    Ok(parsed_number)
}

fn main() {}
```

이 함수는 `&str`을 받습니다. `Ok`라면, `Ok`로 감싼 `i32`를 줍니다. `Err`라면, `ParseIntError`를 반환합니다. 그러면 우리는 숫자를 파싱하려고 시도하고, `?`를 추가합니다. 그것은 "에러인지 확인하고, 괜찮다면 Result 안의 내용을 달라"는 뜻입니다. 괜찮지 않다면, 에러를 반환하고 끝날 것입니다. 하지만 괜찮다면, 다음 줄로 갈 것입니다. 다음 줄에는 `Ok()` 안의 숫자가 있습니다. 반환이 `i32`가 아니라 `Result<i32, ParseIntError>`이므로 우리는 그것을 `Ok`로 감쌀 필요가 있습니다.

이제, 우리 함수를 시도해볼 수 있습니다. `&str`들의 vec으로 무엇을 하는지 봅시다.

```rust
fn parse_str(input: &str) -> Result<i32, std::num::ParseIntError> {
    let parsed_number = input.parse::<i32>()?;
    Ok(parsed_number)
}

fn main() {
    let str_vec = vec!["Seven", "8", "9.0", "nice", "6060"];
    for item in str_vec {
        let parsed = parse_str(item);
        println!("{:?}", parsed);
    }
}
```

이것은 다음을 출력합니다:

```text
Err(ParseIntError { kind: InvalidDigit })
Ok(8)
Err(ParseIntError { kind: InvalidDigit })
Err(ParseIntError { kind: InvalidDigit })
Ok(6060)
```

어떻게 `std::num::ParseIntError`를 찾았을까요? 쉬운 방법 중 하나는 컴파일러에게 다시 "물어보는" 것입니다.

```rust
fn main() {
    let failure = "Not a number".parse::<i32>();
    failure.rbrbrb(); // ⚠️ 컴파일러: "rbrbrb()가 뭔가요???"
}
```

컴파일러는 이해하지 못하고 다음과 같이 말합니다:

```text
error[E0599]: no method named `rbrbrb` found for enum `std::result::Result<i32, std::num::ParseIntError>` in the current scope
 --> src\main.rs:3:13
  |
3 |     failure.rbrbrb();
  |             ^^^^^^ method not found in `std::result::Result<i32, std::num::ParseIntError>`
```

그래서 `std::result::Result<i32, std::num::ParseIntError>`가 우리가 필요한 시그니처입니다.

`Result`는 항상 "스코프 안에" 있기 때문에 (스코프 안에 = 사용할 준비가 됨) `std::result::Result`를 쓸 필요가 없습니다. Rust는 우리가 많이 사용하는 모든 타입들에 대해 이렇게 해서 `std::result::Result`, `std::collections::Vec` 등을 쓸 필요가 없습니다.

우리는 아직 파일과 같은 것들을 다루지 않고 있으므로, ? 연산자가 아직 그렇게 유용해 보이지 않습니다. 하지만 여기에 쓸모없지만 한 줄에서 어떻게 사용할 수 있는지 보여주는 빠른 예시가 있습니다. `.parse()`로 `i32`를 만드는 대신, 훨씬 더 많은 일을 할 것입니다. `u16`을 만들고, 그것을 `String`으로 바꾸고, `u32`로, 그리고 다시 `String`으로, 마지막으로 `i32`로 바꿀 것입니다.

```rust
use std::num::ParseIntError;

fn parse_str(input: &str) -> Result<i32, ParseIntError> {
    let parsed_number = input.parse::<u16>()?.to_string().parse::<u32>()?.to_string().parse::<i32>()?; // 매번 ?를 추가해서 확인하고 전달합니다
    Ok(parsed_number)
}

fn main() {
    let str_vec = vec!["Seven", "8", "9.0", "nice", "6060"];
    for item in str_vec {
        let parsed = parse_str(item);
        println!("{:?}", parsed);
    }
}
```

이것은 같은 것을 출력하지만, 이번에는 한 줄에서 세 개의 `Result`를 처리했습니다. 나중에 파일로 이것을 할 것인데, 많은 것들이 잘못될 수 있기 때문에 항상 `Result`를 반환합니다.

다음을 상상해보세요: 파일을 열고, 그것에 쓰고, 닫고 싶습니다. 먼저 파일을 성공적으로 찾아야 합니다 (그것은 `Result`입니다). 그러면 성공적으로 그것에 써야 합니다 (그것은 `Result`입니다). `?`로 한 줄에서 그것을 할 수 있습니다.

### panic과 unwrap이 좋을 때

Rust에는 panic하게 만들 수 있는 `panic!` 매크로가 있습니다. 사용하기 쉽습니다:

```rust
fn main() {
    panic!("Time to panic!");
}
```

프로그램을 실행할 때 `"Time to panic!"` 메시지가 나타납니다: `thread 'main' panicked at 'Time to panic!', src\main.rs:2:3`

`src\main.rs`는 디렉토리와 파일 이름이고, `2:3`은 줄과 열 번호라는 것을 기억할 것입니다. 이 정보로, 코드를 찾아서 고칠 수 있습니다.

`panic!`은 뭔가 바뀔 때 확실히 알 수 있도록 하는 좋은 매크로입니다. 예를 들어, `prints_three_things`라는 이 함수는 벡터에서 항상 인덱스 [0], [1], [2]를 출력합니다. 우리가 항상 세 개의 아이템이 있는 벡터를 주기 때문에 괜찮습니다:

```rust
fn prints_three_things(vector: Vec<i32>) {
    println!("{}, {}, {}", vector[0], vector[1], vector[2]);
}

fn main() {
    let my_vec = vec![8, 9, 10];
    prints_three_things(my_vec);
}
```

`8, 9, 10`을 출력하고 모든 것이 좋습니다.

하지만 나중에 더 많은 코드를 쓰고, `my_vec`이 세 개만 될 수 있다는 것을 잊는다고 상상해보세요. 이제 이 부분에서 `my_vec`에 여섯 개가 있습니다:

```rust
fn prints_three_things(vector: Vec<i32>) {
  println!("{}, {}, {}", vector[0], vector[1], vector[2]);
}

fn main() {
  let my_vec = vec![8, 9, 10, 10, 55, 99]; // 이제 my_vec에 여섯 개가 있습니다
  prints_three_things(my_vec);
}
```

에러가 발생하지 않는데, [0]과 [1]과 [2]가 모두 이 더 긴 `Vec` 안에 있기 때문입니다. 하지만 정말로 세 개만 갖는 것이 중요했다면? 프로그램이 panic하지 않기 때문에 문제가 있다는 것을 알 수 없을 것입니다. 대신 이렇게 했어야 합니다:

```rust
fn prints_three_things(vector: Vec<i32>) {
    if vector.len() != 3 {
        panic!("my_vec must always have three items") // 길이가 3이 아니면 panic할 것입니다
    }
    println!("{}, {}, {}", vector[0], vector[1], vector[2]);
}

fn main() {
    let my_vec = vec![8, 9, 10];
    prints_three_things(my_vec);
}
```

이제 벡터에 여섯 개의 아이템이 있으면 알 수 있을 것인데, 그래야 하는 대로 panic하기 때문입니다:

```rust
    // ⚠️
fn prints_three_things(vector: Vec<i32>) {
    if vector.len() != 3 {
        panic!("my_vec must always have three items")
    }
    println!("{}, {}, {}", vector[0], vector[1], vector[2]);
}

fn main() {
    let my_vec = vec![8, 9, 10, 10, 55, 99];
    prints_three_things(my_vec);
}
```

이것은 `thread 'main' panicked at 'my_vec must always have three items', src\main.rs:8:9`를 줍니다. `panic!` 덕분에, 우리는 이제 `my_vec`이 세 개의 아이템만 가져야 한다는 것을 기억합니다. 그래서 `panic!`은 코드에 알림을 만드는 좋은 매크로입니다.

`panic!`과 비슷한 다른 세 개의 매크로가 있는데 테스트에서 많이 사용합니다. 그것들은: `assert!`, `assert_eq!`, `assert_ne!`입니다.

그것들의 의미는 다음과 같습니다:

- `assert!()`: `()` 안의 부분이 true가 아니면, 프로그램이 panic할 것입니다.
- `assert_eq!()`: `()` 안의 두 아이템이 같아야 합니다.
- `assert_ne!()`: `()` 안의 두 아이템이 같지 않아야 합니다. (*ne*는 not equal을 의미합니다)

몇 가지 예시들:

```rust
fn main() {
    let my_name = "Loki Laufeyson";

    assert!(my_name == "Loki Laufeyson");
    assert_eq!(my_name, "Loki Laufeyson");
    assert_ne!(my_name, "Mithridates");
}
```

이것은 아무것도 하지 않을 것인데, 세 개의 assert 매크로가 모두 괜찮기 때문입니다. (이것이 우리가 원하는 것입니다)

원한다면 메시지도 추가할 수 있습니다.

```rust
fn main() {
    let my_name = "Loki Laufeyson";

    assert!(
        my_name == "Loki Laufeyson",
        "{} should be Loki Laufeyson",
        my_name
    );
    assert_eq!(
        my_name, "Loki Laufeyson",
        "{} and Loki Laufeyson should be equal",
        my_name
    );
    assert_ne!(
        my_name, "Mithridates",
        "You entered {}. Input must not equal Mithridates",
        my_name
    );
}
```

이 메시지들은 프로그램이 panic할 때만 나타날 것입니다. 그래서 이것을 실행하면:

```rust
fn main() {
    let my_name = "Mithridates";

    assert_ne!(
        my_name, "Mithridates",
        "You enter {}. Input must not equal Mithridates",
        my_name
    );
}
```

다음을 나타낼 것입니다:

```text
thread 'main' panicked at 'assertion failed: `(left != right)`
  left: `"Mithridates"`,
 right: `"Mithridates"`: You entered Mithridates. Input must not equal Mithridates', src\main.rs:4:5
```

그래서 "당신은 left != right라고 했지만, left == right입니다"라고 말하고 있습니다. 그리고 `You entered Mithridates. Input must not equal Mithridates`라고 하는 우리 메시지를 나타냅니다.

`unwrap`도 프로그램을 쓰고 있고 문제가 있을 때 충돌하게 하고 싶을 때 좋습니다. 나중에, 코드가 끝났을 때 `unwrap`을 충돌하지 않을 다른 것으로 바꾸는 것이 좋습니다.

`unwrap`과 비슷하지만 자신만의 메시지를 줄 수 있어서 약간 더 나은 `expect`도 사용할 수 있습니다. 교과서들은 보통 이런 조언을 줍니다: "`.unwrap()`을 많이 사용한다면, 최소한 더 나은 에러 메시지를 위해 `.expect()`를 사용하세요."

이것은 충돌할 것입니다:

```rust
   // ⚠️
fn get_fourth(input: &Vec<i32>) -> i32 {
    let fourth = input.get(3).unwrap();
    *fourth
}

fn main() {
    let my_vec = vec![9, 0, 10];
    let fourth = get_fourth(&my_vec);
}
```

에러 메시지는 `thread 'main' panicked at 'called Option::unwrap() on a None value', src\main.rs:7:18`입니다.

이제 `expect`로 우리만의 메시지를 씁시다:

```rust
   // ⚠️
fn get_fourth(input: &Vec<i32>) -> i32 {
    let fourth = input.get(3).expect("Input vector needs at least 4 items");
    *fourth
}

fn main() {
    let my_vec = vec![9, 0, 10];
    let fourth = get_fourth(&my_vec);
}
```

다시 충돌하지만, 에러가 더 좋습니다: `thread 'main' panicked at 'Input vector needs at least 4 items', src\main.rs:7:18`. `.expect()`는 이것 때문에 `.unwrap()`보다 약간 낫지만, `None`에서 여전히 panic할 것입니다. 여기에 나쁜 습관의 예시가 있는데, 두 번 unwrap하려고 시도하는 함수입니다. `Vec<Option<i32>>`를 받으므로, 각 부분마다 `Some<i32>`가 있을 수도 있고 `None`이 있을 수도 있습니다.

```rust
fn try_two_unwraps(input: Vec<Option<i32>>) {
    println!("Index 0 is: {}", input[0].unwrap());
    println!("Index 1 is: {}", input[1].unwrap());
}

fn main() {
    let vector = vec![None, Some(1000)]; // 이 벡터에는 None이 있으므로 panic할 것입니다
    try_two_unwraps(vector);
}
```

메시지는: `thread 'main' panicked at 'called Option::unwrap() on a None value', src\main.rs:2:32`입니다. 줄을 확인하기 전까지는 첫 번째 `.unwrap()`인지 두 번째 `.unwrap()`인지 확실하지 않습니다. 길이를 확인하고 unwrap하지 않는 것이 더 나을 것입니다. 하지만 `.expect()`로는 최소한 *조금* 더 나을 것입니다. 여기에 `.expect()`와 함께:

```rust
fn try_two_unwraps(input: Vec<Option<i32>>) {
    println!("Index 0 is: {}", input[0].expect("The first unwrap had a None!"));
    println!("Index 1 is: {}", input[1].expect("The second unwrap had a None!"));
}

fn main() {
    let vector = vec![None, Some(1000)];
    try_two_unwraps(vector);
}
```

그래서 조금 더 낫습니다: `thread 'main' panicked at 'The first unwrap had a None!', src\main.rs:2:32`. 줄 번호도 있어서 찾을 수 있습니다.

항상 선택하고 싶은 값이 있다면 `unwrap_or`도 사용할 수 있습니다. 이것을 하면 절대 panic하지 않을 것입니다. 그것은:

- 1) 프로그램이 panic하지 않기 때문에 좋지만,
- 2) 문제가 있을 때 프로그램이 panic하기를 원한다면 좋지 않을 수도 있습니다.

하지만 보통 우리는 프로그램이 panic하는 것을 원하지 않으므로, `unwrap_or`는 사용하기 좋은 메서드입니다.

```rust
fn main() {
    let my_vec = vec![8, 9, 10];

    let fourth = my_vec.get(3).unwrap_or(&0); // .get이 동작하지 않으면, 값을 &0으로 만들 것입니다.
                                              // .get은 참조를 반환하므로, 0이 아니라 &0이 필요합니다
                                              // fourth가 &0이 아니라 0이 되게 하고 싶다면 "let *fourth"를 *로 쓸 수 있지만,
                                              // 여기서는 그냥 출력하므로 상관없습니다

    println!("{}", fourth);
}
```

이것은 `None`이어도 `unwrap_or(&0)`이 0을 주기 때문에 `0`을 출력합니다.

## 트레이트

우리는 이전에 트레이트를 봤습니다: `Debug`, `Copy`, `Clone`은 모두 트레이트입니다. 타입에 트레이트를 주려면, 그것을 구현해야 합니다. `Debug`와 다른 것들은 매우 일반적이기 때문에, 자동으로 해주는 속성들이 있습니다. `#[derive(Debug)]`를 쓸 때 일어나는 일이 바로 그것입니다: 자동으로 `Debug`를 구현하고 있는 것입니다.

```rust
#[derive(Debug)]
struct MyStruct {
    number: usize,
}

fn main() {}
```

하지만 다른 트레이트들은 더 어려우므로, `impl`로 수동으로 구현해야 합니다. 예를 들어, `Add` (`std::ops::Add`에서 찾을 수 있는)는 두 개를 더하는 데 사용됩니다. 하지만 Rust는 정확히 어떻게 더하고 싶은지 모르므로, 알려줘야 합니다.

```rust
struct ThingsToAdd {
    first_thing: u32,
    second_thing: f32,
}

fn main() {}
```

`first_thing`과 `second_thing`을 더할 수 있지만, 더 많은 정보를 줘야 합니다. 아마도 `f32`를 원하므로, 이런 것:

```rust
// 🚧
let result = self.second_thing + self.first_thing as f32
```

하지만 아마도 정수를 원하므로, 이런 것:

```rust
// 🚧
let result = self.second_thing as u32 + self.first_thing
```

또는 아마도 그냥 `self.first_thing`을 `self.second_thing` 옆에 놓고 이것이 우리가 더하고 싶은 방법이라고 말하고 싶을 수도 있습니다. 그래서 55를 33.4에 더하면, 88.4가 아니라 5533.4를 보고 싶습니다.

그래서 먼저 트레이트를 만드는 방법을 봅시다. `trait`에 대해 기억해야 할 중요한 것은 행동에 관한 것이라는 것입니다. 트레이트를 만들려면, `trait`를 쓰고 함수들을 만듭니다.

```rust
struct Animal { // 간단한 구조체 - Animal은 이름만 있습니다
    name: String,
}

trait Dog { // Dog 트레이트는 일부 기능을 줍니다
    fn bark(&self) { // 짖을 수 있습니다
        println!("Woof woof!");
    }
    fn run(&self) { // 그리고 달릴 수 있습니다
        println!("The dog is running!");
    }
}

impl Dog for Animal {} // 이제 Animal은 Dog 트레이트를 가집니다

fn main() {
    let rover = Animal {
        name: "Rover".to_string(),
    };

    rover.bark(); // 이제 Animal은 bark()를 사용할 수 있습니다
    rover.run();  // 그리고 run()을 사용할 수 있습니다
}
```

이것은 괜찮지만, "The dog is running"을 출력하고 싶지 않습니다. 원한다면 `trait`가 주는 메서드들을 바꿀 수 있지만, 같은 시그니처를 가져야 합니다. 그것은 같은 것들을 받고, 같은 것들을 반환해야 한다는 뜻입니다. 예를 들어, `.run()` 메서드를 바꿀 수 있지만 시그니처를 따라야 합니다. 시그니처는 다음과 같습니다:

```rust
// 🚧
fn run(&self) {
    println!("The dog is running!");
}
```

`fn run(&self)`는 "fn `run()`은 `&self`를 받고, 아무것도 반환하지 않는다"는 뜻입니다. 그래서 이렇게 할 수 없습니다:

```rust
fn run(&self) -> i32 { // ⚠️
    5
}
```

Rust는 다음과 같이 말할 것입니다:

```text
   = note: expected fn pointer `fn(&Animal)`
              found fn pointer `fn(&Animal) -> i32`
```

하지만 이렇게 할 수 있습니다:

```rust
struct Animal { // 간단한 구조체 - Animal은 이름만 있습니다
    name: String,
}

trait Dog { // Dog 트레이트는 일부 기능을 줍니다
    fn bark(&self) { // 짖을 수 있습니다
        println!("Woof woof!");
    }
    fn run(&self) { // 그리고 달릴 수 있습니다
        println!("{} is running!", self.name()); // .name()은 우리가 만들어야 하는 메서드입니다
    }
}

impl Dog for Animal {
    fn run(&self) {
        println!("{} is running!", self.name); // 우리는 name을 가지고 있으므로 self.name.을 사용할 수 있습니다
    }
}

fn main() {
    let rover = Animal {
        name: "Rover".to_string(),
    };

    rover.run();
}
```

이것은 `Rover is running!`을 출력할 것입니다. 괜찮지만, 만약 함수 시그니처가 다르다면 어떻게 될까요? 그러면 구현할 수 없습니다. 이 함수에서는 `self.name()`을 사용하려고 하지만, `Animal`에는 `.name()` 메서드가 없습니다. 그것은 `.name`만 가지고 있습니다. 그래서 우리는 `trait`에서 이것을 구현할 수 없습니다. 하지만 trait에 함수 시그니처만 쓰고 body를 쓰지 않으면, 타입이 그것을 구현하게 만들 수 있습니다. 다음과 같이:

```rust
struct Animal { // 간단한 구조체 - Animal은 이름만 있습니다
    name: String,
}

trait Dog { // Dog 트레이트는 일부 기능을 줍니다
    fn bark(&self) { // bark()는 괜찮습니다
        println!("Woof woof!");
    }
    fn run(&self); // run()에는 body가 없으므로 Animal이 구현해야 합니다
}

impl Dog for Animal {
    fn run(&self) {
        println!("{} is running!", self.name); // 이제 self.name을 사용할 수 있습니다
    }
}

fn main() {
    let rover = Animal {
        name: "Rover".to_string(),
    };

    rover.run();
}
```

지금은 이것이 동작하고 `Rover is running!`을 출력합니다.

trait에 body가 없는 함수가 있을 때, 구현하려는 타입이 그것을 만들어야 합니다. 하지만 trait은 하나 이상의 함수를 가질 수 있고, 일부는 body를 가질 수 있고 일부는 그렇지 않을 수 있습니다. 그러나 body가 없으면, 타입이 그것을 만들어야 합니다.

### From 트레이트

*From*은 사용하기 매우 편리한 트레이트이고, 이미 매우 많이 봤기 때문에 이것을 압니다. *From*으로 `&str`로부터 `String`을 만들 수 있지만, 많은 다른 타입들로부터 많은 타입들을 만들 수 있습니다. 예를 들어, Vec은 다음에 대해 *From*을 사용합니다:

```text
From<&'_ [T]>
From<&'_ mut [T]>
From<&'_ str>
From<&'a Vec<T>>
From<[T; N]>
From<BinaryHeap<T>>
From<Box<[T]>>
From<CString>
From<Cow<'a, [T]>>
From<String>
From<Vec<NonZeroU8>>
From<Vec<T>>
From<VecDeque<T>>
```

아직 시도해보지 않은 많은 `Vec::from()`이 있습니다. 몇 개를 만들어서 무슨 일이 일어나는지 봅시다.

```rust
use std::fmt::Display; // 출력하기 위한 제네릭 함수를 만들 것이므로 Display가 필요합니다

fn print_vec<T: Display>(input: &Vec<T>) { // 타입 T가 Display를 가지면 어떤 Vec<T>든 받습니다
    for item in input {
        print!("{} ", item);
    }
    println!();
}

fn main() {

    let array_vec = Vec::from([8, 9, 10]); // 배열로부터 시도
    print_vec(&array_vec);

    let str_vec = Vec::from("What kind of vec will I be?"); // &str로부터 배열? 이것은 흥미로울 것입니다
    print_vec(&str_vec);

    let string_vec = Vec::from("What kind of vec will a String be?".to_string()); // String으로부터도
    print_vec(&string_vec);
}
```

다음을 출력합니다:

```text
8 9 10
87 104 97 116 32 107 105 110 100 32 111 102 32 118 101 99 32 119 105 108 108 32 73 32 98 101 63
87 104 97 116 32 107 105 110 100 32 111 102 32 118 101 99 32 119 105 108 108 32 97 32 83 116 114 105 110 103 32 98 101 63
```

타입을 보면, 두 번째와 세 번째 벡터는 `Vec<u8>`이고, 이것은 `&str`과 `String`의 바이트들을 의미합니다. 그래서 `From`이 매우 유연하고 많이 사용된다는 것을 볼 수 있습니다. 우리 자신의 타입들로 시도해봅시다.

두 개의 구조체를 만들고 그 중 하나에 대해 `From`을 구현할 것입니다. 하나의 구조체는 `City`이고, 다른 하나는 `Country`입니다. 이것을 할 수 있기를 원합니다: `let country_name = Country::from(vector_of_cities)`.

다음과 같습니다:

```rust
#[derive(Debug)] // City를 출력할 수 있도록
struct City {
    name: String,
    population: u32,
}

impl City {
    fn new(name: &str, population: u32) -> Self { // 그냥 new 함수
        Self {
            name: name.to_string(),
            population,
        }
    }
}
#[derive(Debug)] // Country도 출력될 필요가 있습니다
struct Country {
    cities: Vec<City>, // 우리의 도시들이 여기에 들어갑니다
}

impl From<Vec<City>> for Country { // 주목: From<City>를 쓸 필요가 없습니다, From<Vec<City>>도 할 수 있습니다.
                                   // 그래서 우리가 만들지 않은 타입에 대해서도 구현할 수 있습니다
    fn from(cities: Vec<City>) -> Self {
        Self { cities }
    }
}

impl Country {
    fn print_cities(&self) { // Country의 도시들을 출력하는 함수
        for city in &self.cities {
            // Vec<City>는 Copy가 아니므로 &
            println!("{:?} has a population of {:?}.", city.name, city.population);
        }
    }
}

fn main() {
    let helsinki = City::new("Helsinki", 631_695);
    let turku = City::new("Turku", 186_756);

    let finland_cities = vec![helsinki, turku]; // 이것이 Vec<City>입니다
    let finland = Country::from(finland_cities); // 이제 From을 사용할 수 있습니다

    finland.print_cities();
}
```

이것은 다음을 출력합니다:

```text
"Helsinki" has a population of 631695.
"Turku" has a population of 186756.
```

`From`이 `Vec`, `i32` 등과 같이 당신이 만들지 않은 타입들로부터 구현하기 쉽다는 것을 볼 수 있습니다. 여기에 두 개의 벡터를 가진 벡터를 만드는 또 다른 예시가 있습니다. 첫 번째 벡터는 짝수를 담고, 두 번째는 홀수를 담습니다. `From`으로 `i32`들의 벡터를 주면 그것을 `Vec<Vec<i32>>`로 바꿀 것입니다: `i32`들의 벡터들을 담는 벡터.

```rust
use std::convert::From;

struct EvenOddVec(Vec<Vec<i32>>);

impl From<Vec<i32>> for EvenOddVec {
    fn from(input: Vec<i32>) -> Self {
        let mut even_odd_vec: Vec<Vec<i32>> = vec![vec![], vec![]]; // 안에 두 개의 빈 벡터를 가진 벡터
                                                                    // 이것이 반환 값이지만 먼저 채워야 합니다
        for item in input {
            if item % 2 == 0 {
                even_odd_vec[0].push(item);
            } else {
                even_odd_vec[1].push(item);
            }
        }
        Self(even_odd_vec) // 이제 끝났으므로 Self로 반환합니다 (Self = EvenOddVec)
    }
}

fn main() {
    let bunch_of_numbers = vec![8, 7, -1, 3, 222, 9787, -47, 77, 0, 55, 7, 8];
    let new_vec = EvenOddVec::from(bunch_of_numbers);

    println!("Even numbers: {:?}\nOdd numbers: {:?}", new_vec.0[0], new_vec.0[1]);
}
```

이것은 다음을 출력합니다:

```text
Even numbers: [8, 222, 0, 8]
Odd numbers: [7, -1, 3, 9787, -47, 77, 55, 7]
```

`EvenOddVec` 같은 타입은 아마도 제네릭 `T`로 하는 것이 더 나을 것이므로 많은 숫자 타입들을 사용할 수 있습니다. 원한다면 연습을 위해 예시를 제네릭으로 만들어볼 수 있습니다.

### 함수에서 String과 &str 받기

때때로 `String`과 `&str` 둘 다 받을 수 있는 함수를 원합니다. 제네릭과 `AsRef` 트레이트로 이것을 할 수 있습니다. `AsRef`는 한 타입에서 다른 타입으로의 참조를 주는 데 사용됩니다. `String`의 문서를 보면, 많은 타입들에 대해 `AsRef`를 가지는 것을 볼 수 있습니다:

[https://doc.rust-lang.org/std/string/struct.String.html](https://doc.rust-lang.org/std/string/struct.String.html)

여기에 그것들에 대한 일부 함수 시그니처들이 있습니다.

`AsRef<str>`:

```rust
// 🚧
impl AsRef<str> for String

fn as_ref(&self) -> &str
```

`AsRef<[u8]>`:

```rust
// 🚧
impl AsRef<[u8]> for String

fn as_ref(&self) -> &[u8]
```

`AsRef<OsStr>`:

```rust
// 🚧
impl AsRef<OsStr> for String

fn as_ref(&self) -> &OsStr
```

그것이 `&self`를 받고 다른 타입에 대한 참조를 준다는 것을 볼 수 있습니다. 이것은 만약 제네릭 타입 T가 있다면, 그것이 `AsRef<str>`를 필요로 한다고 말할 수 있다는 뜻입니다. 그렇게 하면, 그것은 `&str`과 `String`을 받을 수 있을 것입니다.

제네릭 함수로 시작해봅시다. 이것은 아직 동작하지 않습니다:

```rust
fn print_it<T>(input: T) {
    println!("{}", input) // ⚠️
}

fn main() {
    print_it("Please print me");
}
```

Rust는 `error[E0277]: T doesn't implement std::fmt::Display`라고 말합니다. 그래서 T가 Display를 구현하도록 요구할 것입니다.

```rust
use std::fmt::Display;

fn print_it<T: Display>(input: T) {
    println!("{}", input)
}

fn main() {
    print_it("Please print me");
}
```

이제 동작하고 `Please print me`를 출력합니다. 그것은 좋지만, T는 여전히 너무 많은 것들이 될 수 있습니다. 그것은 `i8`, `f32` 그리고 단지 `Display`를 가진 다른 어떤 것이든 될 수 있습니다. 그래서 `AsRef<str>`를 추가하고, 이제 T는 `AsRef<str>`와 `Display` 둘 다 필요로 합니다.

```rust
use std::fmt::Display;

fn print_it<T: AsRef<str> + Display>(input: T) {
    println!("{}", input)
}

fn main() {
    print_it("Please print me");
    print_it("Also, please print me".to_string());
    // print_it(7); <- 이것은 출력되지 않을 것입니다
}
```

이제 그것은 `i8` 같은 타입들을 받지 않을 것입니다.

길어질 때 `where`를 사용해서 함수를 다르게 쓸 수 있다는 것을 잊지 마세요. Debug를 추가하면 `fn print_it<T: AsRef<str> + Display + Debug>(input: T)`가 되고 한 줄에 너무 깁니다. 그래서 이렇게 쓸 수 있습니다:

```rust
use std::fmt::{Debug, Display}; // Debug 추가

fn print_it<T>(input: T) // 이제 이 줄은 읽기 쉽습니다
where
    T: AsRef<str> + Debug + Display, // 그리고 이 트레이트들은 읽기 쉽습니다
{
    println!("{}", input)
}

fn main() {
    print_it("Please print me");
    print_it("Also, please print me".to_string());
}
```

## 메서드 체이닝

Rust는 C와 C++처럼 시스템 프로그래밍 언어이고, 코드를 별도의 줄에 별도의 명령어로 작성할 수 있지만, 함수형 스타일도 가지고 있습니다. 두 스타일 모두 괜찮지만, 함수형 스타일이 보통 더 짧습니다. 다음은 1부터 10까지의 `Vec`을 만드는 비함수형 스타일(명령형 스타일이라고 불리는)의 예시입니다:

```rust
fn main() {
    let mut new_vec = Vec::new();
    let mut counter = 1;

    while counter < 11 {
        new_vec.push(counter);
        counter += 1;
    }

    println!("{:?}", new_vec);
}
```

이것은 `[1, 2, 3, 4, 5, 6, 7, 8, 9, 10]`을 출력합니다.

그리고 다음은 함수형 스타일의 예시입니다:

```rust
fn main() {
    let new_vec = (1..=10).collect::<Vec<i32>>();
    // 또는 이렇게 쓸 수 있습니다:
    // let new_vec: Vec<i32> = (1..=10).collect();
    println!("{:?}", new_vec);
}
```

`.collect()`는 많은 타입의 컬렉션을 만들 수 있으므로, 타입을 알려줘야 합니다.

함수형 스타일에서는 메서드를 체이닝할 수 있습니다. "메서드 체이닝"이란 하나의 문장에서 여러 메서드를 함께 연결하는 것을 의미합니다. 다음은 많은 메서드들이 함께 체이닝된 예시입니다:

```rust
fn main() {
    let my_vec = vec![0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10];

    let new_vec = my_vec.into_iter().skip(3).take(4).collect::<Vec<i32>>();

    println!("{:?}", new_vec);
}
```

이것은 `[3, 4, 5, 6]`을 가진 Vec을 생성합니다. 이것은 한 줄에 너무 많은 정보이므로, 각 메서드를 새 줄에 놓는 것이 도움이 될 수 있습니다. 읽기 쉽게 만들기 위해 그렇게 해봅시다:

```rust
fn main() {
    let my_vec = vec![0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10];

    let new_vec = my_vec
        .into_iter() // 아이템들을 "반복"합니다 (반복 = 그 안의 각 아이템과 작업하는 것). into_iter()는 참조가 아닌 소유된 값들을 줍니다
        .skip(3) // 세 개의 아이템을 건너뜁니다: 0, 1, 그리고 2
        .take(4) // 다음 네 개를 가져옵니다: 3, 4, 5, 그리고 6
        .collect::<Vec<i32>>(); // 그것들을 새로운 Vec<i32>에 넣습니다

    println!("{:?}", new_vec);
}
```

클로저와 이터레이터를 이해할 때 이 함수형 스타일을 가장 잘 사용할 수 있습니다. 그래서 다음에 그것들을 배울 것입니다.

## 반복자

반복자는 컬렉션의 아이템들을 한 번에 하나씩 줄 수 있는 구조체입니다. 사실 우리는 이미 반복자를 많이 사용했습니다: `for` 루프가 반복자를 제공합니다. 다른 경우에 반복자를 사용하고 싶을 때는 어떤 종류를 선택해야 합니다:

- `.iter()` 참조의 반복자
- `.iter_mut()` 가변 참조의 반복자
- `.into_iter()` 값의 반복자 (참조가 아닌)

`for` 루프는 실제로는 값을 소유하는 반복자입니다. 그래서 가변으로 만들고 사용할 때 값을 변경할 수 있습니다.

다음과 같이 반복자를 사용할 수 있습니다:

```rust
fn main() {
    let vector1 = vec![1, 2, 3]; // 이것에 .iter()와 .into_iter()를 사용할 것입니다
    let vector1_a = vector1.iter().map(|x| x + 1).collect::<Vec<i32>>();
    let vector1_b = vector1.into_iter().map(|x| x * 10).collect::<Vec<i32>>();

    let mut vector2 = vec![10, 20, 30]; // 이것에 .iter_mut()를 사용할 것입니다
    vector2.iter_mut().for_each(|x| *x +=100);

    println!("{:?}", vector1_a);
    println!("{:?}", vector2);
    println!("{:?}", vector1_b);
}
```

이것은 다음을 출력합니다:

```text
[2, 3, 4]
[110, 120, 130]
[10, 20, 30]
```

첫 번째 두 개에는 `.map()`이라는 메서드를 사용했습니다. 이 메서드는 모든 아이템에 대해 무언가를 한 다음 전달할 수 있게 해줍니다. 마지막 것에는 `.for_each()`라는 메서드를 사용했습니다. 이 메서드는 모든 아이템에 대해 무언가를 할 수 있게 해줍니다. `.iter_mut()` 더하기 `for_each()`는 기본적으로 `for` 루프와 같습니다. 각 메서드 안에서 모든 아이템에 이름을 줄 수 있고 (우리는 그냥 `x`라고 했습니다) 그것을 사용해서 변경할 수 있습니다. 이것들을 클로저라고 하며 다음 섹션에서 배울 것입니다.

한 번에 하나씩 다시 살펴봅시다.

먼저 `vector1`에 `.iter()`를 사용해서 참조를 얻었습니다. 각각에 1을 더하고 새로운 Vec으로 만들었습니다. `vector1`은 참조만 사용했기 때문에 아직 살아있습니다: 값으로 가져오지 않았습니다. 이제 `vector1`과 `vector1_a`라는 새로운 Vec이 있습니다. `.map()`은 그냥 전달하기 때문에 Vec으로 만들기 위해 `.collect()`를 사용해야 했습니다.

그다음 `vector1`에서 값으로 반복자를 얻기 위해 `into_iter`를 사용했습니다. 이것은 `vector1`을 파괴합니다. `into_iter()`가 하는 일이기 때문입니다. 그래서 `vector1_b`를 만든 후에는 `vector1`을 다시 사용할 수 없습니다.

마지막으로 `vector2`에 `.iter_mut()`를 사용했습니다. 가변이므로 새로운 Vec을 만들기 위해 `.collect()`를 사용할 필요가 없습니다. 대신 가변 참조로 같은 Vec에서 값들을 변경합니다. 그래서 `vector2`는 여전히 있습니다. 새로운 Vec이 필요하지 않기 때문에 `for_each`를 사용합니다: `for` 루프와 같습니다.

### 반복자가 작동하는 방식

반복자는 `Option`을 주는 `.next()`라는 메서드를 사용해서 작동합니다. 반복자를 사용할 때 Rust는 `next()`를 계속해서 호출합니다. `Some`을 얻으면 계속 진행합니다. `None`을 얻으면 멈춥니다.

`assert_eq!` 매크로를 기억하나요? 문서에서는 항상 볼 수 있습니다. 여기서 반복자가 어떻게 작동하는지 보여줍니다.

```rust
fn main() {
    let my_vec = vec!['a', 'b', '거', '柳']; // 그냥 일반적인 Vec

    let mut my_vec_iter = my_vec.iter(); // 이것은 이제 Iterator 타입이지만 아직 호출하지 않았습니다

    assert_eq!(my_vec_iter.next(), Some(&'a'));  // .next()로 첫 번째 아이템을 호출
    assert_eq!(my_vec_iter.next(), Some(&'b'));  // 다음을 호출
    assert_eq!(my_vec_iter.next(), Some(&'거')); // 다시
    assert_eq!(my_vec_iter.next(), Some(&'柳')); // 다시
    assert_eq!(my_vec_iter.next(), None);        // 남은 것이 없습니다: 그냥 None
    assert_eq!(my_vec_iter.next(), None);        // .next()를 계속 호출할 수 있지만 항상 None일 것입니다
}
```

자신의 구조체나 열거형에 `Iterator`를 구현하는 것은 그렇게 어렵지 않습니다. 먼저 도서관을 만들고 생각해봅시다.

```rust
#[derive(Debug)] // {:?}로 출력하고 싶습니다
struct Library {
    library_type: LibraryType, // 이것은 우리의 열거형입니다
    books: Vec<String>, // 책 목록
}

#[derive(Debug)]
enum LibraryType { // 도서관은 시립 도서관이나 군립 도서관이 될 수 있습니다
    City,
    Country,
}

impl Library {
    fn add_book(&mut self, book: &str) { // add_book을 사용해서 새 책을 추가합니다
        self.books.push(book.to_string()); // &str을 가져와서 String으로 바꾸고 Vec에 추가합니다
    }

    fn new() -> Self { // 이것은 새로운 Library를 만듭니다
        Self {
            library_type: LibraryType::City, // 대부분이 시내에 있으므로 City를 선택합니다
                                             // 대부분의 경우
            books: Vec::new(),
        }
    }
}

fn main() {
    let mut my_library = Library::new(); // 새로운 도서관을 만듭니다
    my_library.add_book("The Doom of the Darksword"); // 몇 권의 책을 추가합니다
    my_library.add_book("Demian - die Geschichte einer Jugend");
    my_library.add_book("구운몽");
    my_library.add_book("吾輩は猫である");

    println!("{:?}", my_library.books); // 책 목록을 출력할 수 있습니다
}
```

잘 작동합니다. 이제 `for` 루프에서 사용할 수 있도록 도서관에 `Iterator`를 구현하고 싶습니다. 지금 `for` 루프를 시도하면 작동하지 않습니다:

```rust
for item in my_library {
    println!("{}", item); // ⚠️
}
```

다음과 같이 말합니다:

```text
error[E0277]: `Library` is not an iterator
  --> src\main.rs:47:16
   |
47 |    for item in my_library {
   |                ^^^^^^^^^^ `Library` is not an iterator
   |
   = help: the trait `std::iter::Iterator` is not implemented for `Library`
   = note: required by `std::iter::IntoIterator::into_iter`
```

하지만 `impl Iterator for Library`로 도서관을 반복자로 만들 수 있습니다. `Iterator` 트레이트에 대한 정보는 표준 라이브러리에 있습니다: [https://doc.rust-lang.org/std/iter/trait.Iterator.html](https://doc.rust-lang.org/std/iter/trait.Iterator.html)

페이지 왼쪽 상단에 `Associated Types: Item`과 `Required Methods: next`라고 되어 있습니다. "연관 타입"은 "함께 가는 타입"을 의미합니다. 우리의 연관 타입은 `String`이 될 것입니다. 반복자가 우리에게 String을 주기를 원하기 때문입니다.

페이지에는 다음과 같은 예시가 있습니다:

```rust
// Some과 None을 번갈아 가는 반복자
struct Alternate {
    state: i32,
}

impl Iterator for Alternate {
    type Item = i32;

    fn next(&mut self) -> Option<i32> {
        let val = self.state;
        self.state = self.state + 1;

        // 짝수면 Some(i32), 아니면 None
        if val % 2 == 0 {
            Some(val)
        } else {
            None
        }
    }
}

fn main() {}
```

`impl Iterator for Alternate` 아래에 `type Item = i32`라고 되어 있는 것을 볼 수 있습니다. 이것이 연관 타입입니다. 우리의 반복자는 `Vec<String>`인 책 목록을 위한 것입니다. next를 호출하면 `String`을 줄 것입니다. 그래서 `type Item = String;`을 쓸 것입니다. 그것이 연관 아이템입니다.

`Iterator`를 구현하려면 `fn next()` 함수를 써야 합니다. 여기서 반복자가 무엇을 해야 하는지 결정합니다. 우리의 `Library`에서는 마지막 책을 먼저 주기를 원합니다. 그래서 `Some`이면 마지막 아이템을 제거하는 `.pop()`으로 `match`할 것입니다. 또한 각 아이템에 대해 " is found!"를 출력하고 싶습니다. 이제 다음과 같습니다:

```rust
#[derive(Debug, Clone)]
struct Library {
    library_type: LibraryType,
    books: Vec<String>,
}

#[derive(Debug, Clone)]
enum LibraryType {
    City,
    Country,
}

impl Library {
    fn add_book(&mut self, book: &str) {
        self.books.push(book.to_string());
    }

    fn new() -> Self {
        Self {
            library_type: LibraryType::City,
            // 대부분의 경우
            books: Vec::new(),
        }
    }
}

impl Iterator for Library {
    type Item = String;

    fn next(&mut self) -> Option<String> {
        match self.books.pop() {
            Some(book) => Some(book + " is found!"), // Rust는 String + &str을 허용합니다
            None => None,
        }
    }
}

fn main() {
    let mut my_library = Library::new();
    my_library.add_book("The Doom of the Darksword");
    my_library.add_book("Demian - die Geschichte einer Jugend");
    my_library.add_book("구운몽");
    my_library.add_book("吾輩は猫である");

    for item in my_library.clone() { // 이제 for 루프를 사용할 수 있습니다. Library가 파괴되지 않도록 클론을 줍니다
        println!("{}", item);
    }
}
```

이것은 다음을 출력합니다:

```text
吾輩は猫である is found!
구운몽 is found!
Demian - die Geschichte einer Jugend is found!
The Doom of the Darksword is found!
```

## 클로저

클로저는 이름이 필요 없는 빠른 함수와 같습니다. 때로는 람다라고도 불립니다. 클로저는 `()`대신 `||`를 사용하기 때문에 쉽게 찾을 수 있습니다. Rust에서 매우 흔하게 사용되며, 클로저 사용법을 익히고 나면 클로저 없이 어떻게 살았는지 궁금해질 것입니다.

클로저를 변수에 바인딩할 수 있으며, 그러면 사용할 때 함수와 똑같이 보입니다:

```rust
fn main() {
    let my_closure = || println!("This is a closure");
    my_closure();
}
```

이 클로저는 아무것도 받지 않고(`||`) 메시지를 출력합니다: `This is a closure`.

`||` 사이에 함수의 `()` 안에서와 같이 입력 변수와 타입을 추가할 수 있습니다:

```rust
fn main() {
    let my_closure = |x: i32| println!("{}", x);

    my_closure(5);
    my_closure(5+5);
}
```

이것은 다음을 출력합니다:

```text
5
10
```

클로저가 더 복잡해지면 코드 블록을 추가할 수 있습니다. 그러면 원하는 만큼 길게 만들 수 있습니다.

```rust
fn main() {
    let my_closure = || {
        let number = 7;
        let other_number = 10;
        println!("The two numbers are {} and {}.", number, other_number);
          // 이 클로저는 함수처럼 원하는 만큼 길게 만들 수 있습니다.
    };

    my_closure();
}
```

하지만 클로저는 특별합니다. `||`만 작성하더라도 클로저 외부의 변수를 가져올 수 있기 때문입니다. 따라서 다음과 같이 할 수 있습니다:

```rust
fn main() {
    let number_one = 6;
    let number_two = 10;

    let my_closure = || println!("{}", number_one + number_two);
    my_closure();
}
```

이것은 `16`을 출력합니다. `||` 안에 아무것도 넣을 필요가 없었습니다. 클로저가 `number_one`과 `number_two`를 가져와서 더할 수 있기 때문입니다.

그런데 **클로저**라는 이름은 여기서 나왔습니다. 변수들을 가져와서 "둘러싸기" 때문입니다. 정확히 말하자면:

- 외부에서 변수를 둘러싸지 않는 `||`는 "익명 함수"입니다. 익명은 "이름이 없다"는 뜻입니다. 이것은 일반 함수처럼 작동합니다.
- 외부에서 변수를 둘러싸는 `||`는 "클로저"입니다. 주변의 변수들을 "둘러싸서" 사용합니다.

하지만 사람들은 종종 모든 `||` 함수를 클로저라고 부르므로, 이름에 대해 걱정할 필요는 없습니다. 우리는 `||`가 있는 모든 것을 "클로저"라고 하겠지만, "익명 함수"를 의미할 수도 있다는 것을 기억하세요.

왜 차이점을 아는 것이 좋을까요? 익명 함수는 실제로 이름이 있는 함수와 같은 기계어 코드를 만들기 때문입니다. "고수준"처럼 느껴지므로 때로는 사람들이 기계어 코드가 복잡할 것이라고 생각합니다. 하지만 Rust가 만드는 기계어 코드는 일반 함수만큼 빠릅니다.

이제 클로저가 할 수 있는 더 많은 것들을 살펴보겠습니다. 다음과 같이 할 수도 있습니다:

```rust
fn main() {
    let number_one = 6;
    let number_two = 10;

    let my_closure = |x: i32| println!("{}", number_one + number_two + x);
    my_closure(5);
}
```

이 클로저는 `number_one`과 `number_two`를 가져옵니다. 또한 새로운 변수 `x`를 주고 `x`가 5라고 했습니다. 그러면 세 개를 모두 더해서 `21`을 출력합니다.

보통 Rust에서는 메서드 안에서 클로저를 봅니다. 메서드 안에 클로저를 넣는 것이 매우 편리하기 때문입니다. 지난 섹션에서 `.map()`과 `.for_each()`로 클로저를 봤습니다. 그 섹션에서 우리는 `|x|`를 작성해서 반복자의 다음 항목을 가져왔는데, 그것이 클로저였습니다.

다른 예시가 있습니다: 우리가 아는 `unwrap_or` 메서드는 `unwrap`이 작동하지 않을 때 값을 줄 수 있습니다. 이전에 우리는 `let fourth = my_vec.get(3).unwrap_or(&0);`라고 썼습니다. 하지만 클로저가 들어있는 `unwrap_or_else` 메서드도 있습니다. 따라서 다음과 같이 할 수 있습니다:

```rust
fn main() {
    let my_vec = vec![8, 9, 10];

    let fourth = my_vec.get(3).unwrap_or_else(|| { // 언랩을 시도합니다. 작동하지 않으면,
        if my_vec.get(0).is_some() {               // my_vec가 인덱스 [0]에 무언가 있는지 확인합니다
            &my_vec[0]                             // 무언가 있으면 인덱스 0의 숫자를 줍니다
        } else {
            &0 // 그렇지 않으면 &0을 줍니다
        }
    });

    println!("{}", fourth);
}
```

물론 클로저는 매우 간단할 수 있습니다. 예를 들어 `let fourth = my_vec.get(3).unwrap_or_else(|| &0);`라고 쓸 수 있습니다. 클로저가 있다고 해서 항상 `{}`를 사용하고 복잡한 코드를 작성할 필요는 없습니다. `||`를 넣기만 하면 컴파일러가 필요한 클로저를 넣었다는 것을 알 수 있습니다.

가장 자주 사용되는 클로저 메서드는 아마도 `.map()`일 것입니다. 다시 살펴보겠습니다. 사용하는 한 가지 방법이 있습니다:

```rust
fn main() {
    let num_vec = vec![2, 4, 6];

    let double_vec = num_vec        // num_vec를 가져옵니다
        .iter()                     // 반복합니다
        .map(|number| number * 2)   // 각 항목에 대해 2를 곱합니다
        .collect::<Vec<i32>>();     // 그러면 이것으로부터 새로운 Vec을 만듭니다
    println!("{:?}", double_vec);
}
```

`.enumerate()` 다음에 `.for_each()`를 사용하는 좋은 예시가 있습니다. `.enumerate()` 메서드는 인덱스 번호와 항목이 있는 반복자를 줍니다. 예를 들어: `[10, 9, 8]`이 `(0, 10), (1, 9), (2, 8)`이 됩니다. 여기서 각 항목의 타입은 `(usize, i32)`입니다. 따라서 다음과 같이 할 수 있습니다:

```rust
fn main() {
    let num_vec = vec![10, 9, 8];

    num_vec
        .iter()      // num_vec를 반복합니다
        .enumerate() // (인덱스, 숫자)를 얻습니다
        .for_each(|(index, number)| println!("Index number {} has number {}", index, number)); // 각각에 대해 무언가를 합니다
}
```

이것은 다음을 출력합니다:

```text
Index number 0 has number 10
Index number 1 has number 9
Index number 2 has number 8
```

이 경우 우리는 `map` 대신 `for_each`를 사용합니다. `map`은 **각 항목에 무언가를 해서** 전달하는 것이고, `for_each`는 **각 항목을 볼 때 무언가를 하는** 것입니다. 또한 `map`은 `collect`와 같은 메서드를 사용하지 않으면 아무것도 하지 않습니다.

실제로 이것은 반복자에 대한 흥미로운 점입니다. `collect`와 같은 메서드 없이 `map`을 시도하면, 컴파일러가 아무것도 하지 않는다고 알려줍니다. 패닉이 일어나지는 않지만, 컴파일러가 아무것도 하지 않았다고 알려줍니다.

```rust
fn main() {
    let num_vec = vec![10, 9, 8];

    num_vec
        .iter()
        .enumerate()
        .map(|(index, number)| println!("Index number {} has number {}", index, number));

}
```

이것은 다음과 같이 말합니다:

```text
warning: unused `std::iter::Map` that must be used
 --> src\main.rs:4:5
  |
4 | /     num_vec
5 | |         .iter()
6 | |         .enumerate()
7 | |         .map(|(index, number)| println!("Index number {} has number {}", index, number));
  | |_________________________________________________________________________________________^
  |
  = note: `#[warn(unused_must_use)]` on by default
  = note: iterators are lazy and do nothing unless consumed
```

이것은 **경고**이므로 오류가 아닙니다: 프로그램은 잘 실행됩니다. 하지만 왜 num_vec이 아무것도 하지 않을까요? 타입을 보면 알 수 있습니다.

- `let num_vec = vec![10, 9, 8];` 지금은 `Vec<i32>`입니다.
- `.iter()` 이제 `Iter<i32>`입니다. 따라서 `i32` 항목들의 반복자입니다.
- `.enumerate()` 이제 `Enumerate<Iter<i32>>`입니다. 따라서 `i32`들의 `Iter` 타입의 `Enumerate` 타입입니다.
- `.map()` 이제 `Map<Enumerate<Iter<i32>>>` 타입입니다. 따라서 `i32`들의 `Iter` 타입의 `Enumerate` 타입의 `Map` 타입입니다.

우리가 한 것은 점점 더 복잡한 구조를 만든 것뿐입니다. 따라서 이 `Map<Enumerate<Iter<i32>>>`는 갈 준비가 된 구조이지만, 무엇을 할지 알려줄 때만 작동합니다. Rust는 빨라야 하기 때문에 이렇게 합니다. 다음과 같이 하고 싶지 않습니다:

- Vec에 있는 모든 `i32`들을 반복합니다
- 그러면 반복자에서 모든 `i32`들을 열거합니다
- 그러면 열거된 모든 `i32`들을 매핑합니다

Rust는 한 번의 계산만 하고 싶어하므로, 구조를 만들고 기다립니다. 그러면 `.collect::<Vec<i32>>()`라고 하면 무엇을 할지 알고 움직이기 시작합니다. 이것이 `iterators are lazy and do nothing unless consumed`가 의미하는 것입니다. 반복자들은 "소비"(사용)할 때까지 아무것도 하지 않습니다.

`.collect()`를 사용해서 `HashMap`과 같은 복잡한 것들도 만들 수 있으므로 매우 강력합니다. 다음은 두 개의 vec을 `HashMap`에 넣는 방법의 예시입니다. 먼저 두 개의 벡터를 만들고, 그러면 `.into_iter()`를 사용해서 값들의 반복자를 얻습니다. 그러면 `.zip()` 메서드를 사용합니다. 이 메서드는 두 개의 반복자를 가져와서 지퍼처럼 함께 붙입니다. 마지막으로 `.collect()`를 사용해서 `HashMap`을 만듭니다.

코드는 다음과 같습니다:

```rust
use std::collections::HashMap;

fn main() {
    let some_numbers = vec![0, 1, 2, 3, 4, 5]; // Vec<i32>
    let some_words = vec!["zero", "one", "two", "three", "four", "five"]; // Vec<&str>

    let number_word_hashmap = some_numbers
        .into_iter()                 // 이제 iter입니다
        .zip(some_words.into_iter()) // .zip() 안에 다른 iter를 넣습니다. 이제 함께 있습니다.
        .collect::<HashMap<_, _>>();

    println!("For key {} we get {}.", 2, number_word_hashmap.get(&2).unwrap());
}
```

이것은 다음을 출력합니다:

```text
For key 2 we get two.
```

Rust가 `HashMap<i32, &str>` 타입을 결정하는데 충분한 정보이기 때문에 `<HashMap<_, _>>`라고 썼다는 것을 볼 수 있습니다. 원한다면 `.collect::<HashMap<i32, &str>>();`라고 쓸 수 있거나, 선호한다면 다음과 같이 쓸 수 있습니다:

```rust
use std::collections::HashMap;

fn main() {
    let some_numbers = vec![0, 1, 2, 3, 4, 5]; // Vec<i32>
    let some_words = vec!["zero", "one", "two", "three", "four", "five"]; // Vec<&str>
    let number_word_hashmap: HashMap<_, _> = some_numbers  // 여기서 타입을 알려주므로...
        .into_iter()
        .zip(some_words.into_iter())
        .collect(); // 여기서는 알려줄 필요가 없습니다
}
```

`char`들을 위한 `.enumerate()`와 같은 다른 메서드가 있습니다: `char_indices()`. (Indices는 "인덱스들"을 의미합니다.) 같은 방식으로 사용합니다. 3자리 숫자로 만들어진 큰 문자열이 있다고 가정해 봅시다.

```rust
fn main() {
    let numbers_together = "140399923481800622623218009598281";

    for (index, number) in numbers_together.char_indices() {
        match (index % 3, number) {
            (0..=1, number) => print!("{}", number), // 나머지가 있으면 숫자만 출력합니다
            _ => print!("{}\t", number), // 그렇지 않으면 탭 공간과 함께 숫자를 출력합니다
        }
    }
}
```

이것은 `140     399     923     481     800     622     623     218     009     598    281`을 출력합니다.

### 클로저에서의 |_|

때로는 클로저에서 `|_|`를 볼 수 있습니다. 이것은 클로저가 인수(`x`와 같은)를 필요로 하지만, 사용하고 싶지 않다는 뜻입니다. 따라서 `|_|`는 "좋아, 이 클로저는 인수를 받지만 관심이 없기 때문에 이름을 주지 않을 거야"라는 뜻입니다.

그렇게 하지 않을 때 오류의 예시가 있습니다:

```rust
fn main() {
    let my_vec = vec![8, 9, 10];

    println!("{:?}", my_vec.iter().for_each(|| println!("We didn't use the variables at all"))); // ⚠️
}
```

Rust는 다음과 같이 말합니다:

```text
error[E0593]: closure is expected to take 1 argument, but it takes 0 arguments
  --> src\main.rs:28:36
   |
28 |     println!("{:?}", my_vec.iter().for_each(|| println!("We didn't use the variables at all")));
   |                                    ^^^^^^^^ -- takes 0 arguments
   |                                    |
   |                                    expected closure that takes 1 argument
```

컴파일러가 실제로 도움을 줍니다:

```text
help: consider changing the closure to take and ignore the expected argument
   |
28 |     println!("{:?}", my_vec.iter().for_each(|_| println!("We didn't use the variables at all")));
```

이것은 좋은 조언입니다. `||`를 `|_|`로 바꾸면 작동할 것입니다.

### 클로저와 반복자를 위한 유용한 메서드들

클로저에 익숙해지면 Rust는 매우 재미있는 언어가 됩니다. 클로저로 메서드들을 서로 *연결*할 수 있고 아주 적은 코드로 많은 일을 할 수 있습니다. 다음은 아직 보지 못한 클로저와 클로저와 함께 사용되는 메서드들입니다.

`.filter()`: 이것은 반복자에서 유지하고 싶은 항목들을 유지하게 해줍니다. 연도의 달들을 필터링해 봅시다.

```rust
fn main() {
    let months = vec!["January", "February", "March", "April", "May", "June", "July", "August", "September", "October", "November", "December"];

    let filtered_months = months
        .into_iter()                         // iter를 만듭니다
        .filter(|month| month.len() < 5)     // 길이가 5바이트보다 긴 달들은 원하지 않습니다.
                                             // 각 글자가 1바이트라는 것을 알고 있으므로 .len()이 좋습니다
        .filter(|month| month.contains("u")) // 또한 문자 u가 있는 달들만 좋아합니다
        .collect::<Vec<&str>>();

    println!("{:?}", filtered_months);
}
```

이것은 `["June", "July"]`를 출력합니다.

`.filter_map()`. 이것은 `.filter()`와 `.map()`을 하기 때문에 `filter_map()`이라고 불립니다. 클로저는 `Option<T>`를 반환해야 하고, 그러면 `filter_map()`이 `Some`인 경우 각 `Option`에서 값을 꺼냅니다. 따라서 예를 들어 `vec![Some(2), None, Some(3)]`을 `.filter_map()`하면, `[2, 3]`을 반환할 것입니다.

`Company` 구조체로 예시를 작성하겠습니다. 각 회사는 `name`을 가지고 있으므로 그 필드는 `String`이지만, CEO는 최근에 그만둔 상태일 수도 있습니다. 따라서 `ceo` 필드는 `Option<String>`입니다. 몇몇 회사들에 대해 `.filter_map()`을 사용해서 CEO 이름들만 유지하겠습니다.

```rust
struct Company {
    name: String,
    ceo: Option<String>,
}

impl Company {
    fn new(name: &str, ceo: &str) -> Self {
        let ceo = match ceo {
            "" => None,
            ceo => Some(ceo.to_string()),
        }; // ceo가 결정되었으므로, 이제 Self를 반환합니다
        Self {
            name: name.to_string(),
            ceo,
        }
    }

    fn get_ceo(&self) -> Option<String> {
        self.ceo.clone() // CEO의 클론을 반환합니다 (구조체는 Copy가 아닙니다)
    }
}

fn main() {
    let company_vec = vec![
        Company::new("Umbrella Corporation", "Unknown"),
        Company::new("Ovintiv", "Doug Suttles"),
        Company::new("The Red-Headed League", ""),
        Company::new("Stark Enterprises", ""),
    ];

    let all_the_ceos = company_vec
        .into_iter()
        .filter_map(|company| company.get_ceo()) // filter_map은 Option<T>가 필요합니다
        .collect::<Vec<String>>();

    println!("{:?}", all_the_ceos);
}
```

이것은 `["Unknown", "Doug Suttles"]`를 출력합니다.

`.filter_map()`은 `Option`이 필요한데, `Result`는 어떨까요? 문제없습니다: `Result`를 `Option`으로 바꾸는 `.ok()`라는 메서드가 있습니다. `.ok()`라고 불리는 이유는 `Ok` 결과만 보낼 수 있기 때문입니다(`Err` 정보는 사라집니다). `Option`은 `Option<T>`인 반면 `Result`는 `Ok`과 `Err` 모두에 대한 정보가 있는 `Result<T, E>`라는 것을 기억하세요. 따라서 `.ok()`를 사용하면, 모든 `Err` 정보가 사라지고 `None`이 됩니다.

`.parse()`를 사용하는 것이 이것에 대한 쉬운 예시입니다. 여기서 일부 사용자 입력을 파싱하려고 시도합니다. 여기서 `.parse()`는 `&str`을 받아서 `f32`로 바꾸려고 시도합니다. `Result`를 반환하지만, `filter_map()`을 사용하고 있으므로 오류를 버립니다. `Err`인 모든 것은 `None`이 되고 `.filter_map()`에 의해 필터링됩니다.

```rust
fn main() {
    let user_input = vec!["8.9", "Nine point nine five", "8.0", "7.6", "eleventy-twelve"];

    let actual_numbers = user_input
        .into_iter()
        .filter_map(|input| input.parse::<f32>().ok())
        .collect::<Vec<f32>>();

    println!("{:?}", actual_numbers);
}
```

이것은 `[8.9, 8.0, 7.6]`을 출력합니다.

`.ok()`의 반대편에는 `.ok_or()`와 `ok_or_else()`가 있습니다. 이것은 `Option`을 `Result`로 바꿉니다. `.ok_or()`라고 불리는 이유는 `Result`가 `Ok` **또는** `Err`을 주므로, `Err` 값이 무엇인지 알려줘야 하기 때문입니다. `Option`의 `None`은 어떤 정보도 가지고 있지 않기 때문입니다. 또한 이제 이 메서드들 이름의 *else* 부분이 클로저가 있다는 것을 의미한다는 것을 볼 수 있습니다.

`Company` 구조체에서 `Option`을 가져와서 이 방법으로 `Result`로 바꿀 수 있습니다. 장기적인 오류 처리를 위해서는 자신만의 오류 타입을 만드는 것이 좋습니다. 하지만 지금은 오류 메시지만 주므로, `Result<String, &str>`이 됩니다.

```rust
// main() 이전의 모든 것은 정확히 동일합니다
struct Company {
    name: String,
    ceo: Option<String>,
}

impl Company {
    fn new(name: &str, ceo: &str) -> Self {
        let ceo = match ceo {
            "" => None,
            ceo => Some(ceo.to_string()),
        };
        Self {
            name: name.to_string(),
            ceo,
        }
    }

    fn get_ceo(&self) -> Option<String> {
        self.ceo.clone()
    }
}

fn main() {
    let company_vec = vec![
        Company::new("Umbrella Corporation", "Unknown"),
        Company::new("Ovintiv", "Doug Suttles"),
        Company::new("The Red-Headed League", ""),
        Company::new("Stark Enterprises", ""),
    ];

    let mut results_vec = vec![]; // 오류 결과도 수집해야 한다고 가정합니다

    company_vec
        .iter()
        .for_each(|company| results_vec.push(company.get_ceo().ok_or("No CEO found")));

    for item in results_vec {
        println!("{:?}", item);
    }
}
```

이 줄이 가장 큰 변화입니다:

```rust
// 🚧
.for_each(|company| results_vec.push(company.get_ceo().ok_or("No CEO found")));
```

이것은 다음을 의미합니다: "각 회사에 대해 `get_ceo()`를 사용하세요. 얻으면 `Ok` 안의 값을 전달하세요. 얻지 못하면 `Err` 안의 "No CEO found"를 전달하세요. 그러면 이것을 vec에 푸시하세요."

따라서 `results_vec`을 출력하면 다음을 얻습니다:

```text
Ok("Unknown")
Ok("Doug Suttles")
Err("No CEO found")
Err("No CEO found")
```

이제 네 개의 항목이 모두 있습니다. 이제 `.ok_or_else()`를 사용해서 클로저를 사용하고 더 나은 오류 메시지를 얻어봅시다. 이제 `format!`을 사용해서 `String`을 만들고 회사 이름을 넣을 공간이 있습니다. 그러면 `String`을 반환합니다.

```rust
// main() 이전의 모든 것은 정확히 동일합니다
struct Company {
    name: String,
    ceo: Option<String>,
}

impl Company {
    fn new(name: &str, ceo: &str) -> Self {
        let ceo = match ceo {
            "" => None,
            name => Some(name.to_string()),
        };
        Self {
            name: name.to_string(),
            ceo,
        }
    }

    fn get_ceo(&self) -> Option<String> {
        self.ceo.clone()
    }
}

fn main() {
    let company_vec = vec![
        Company::new("Umbrella Corporation", "Unknown"),
        Company::new("Ovintiv", "Doug Suttles"),
        Company::new("The Red-Headed League", ""),
        Company::new("Stark Enterprises", ""),
    ];

    let mut results_vec = vec![];

    company_vec.iter().for_each(|company| {
        results_vec.push(company.get_ceo().ok_or_else(|| {
            let err_message = format!("No CEO found for {}", company.name);
            err_message
        }))
    });

    for item in results_vec {
        println!("{:?}", item);
    }
}
```

이것은 다음을 줍니다:

```text
Ok("Unknown")
Ok("Doug Suttles")
Err("No CEO found for The Red-Headed League")
Err("No CEO found for Stark Enterprises")
```

`.and_then()`은 `Option`을 받아서, 그 값에 무언가를 하고 전달하게 해주는 유용한 메서드입니다. 따라서 입력은 `Option`이고, 출력도 `Option`입니다. 안전한 "언랩, 그러면 무언가를 하고, 그러면 다시 랩"과 같다고 생각할 수 있습니다.

쉬운 예시는 `.get()`을 사용해서 vec에서 얻는 숫자인데, `Option`을 반환하기 때문입니다. 이제 `and_then()`에 전달할 수 있고, `Some`인 경우 수학을 할 수 있습니다. `None`인 경우, `None`이 그냥 전달됩니다.

```rust
fn main() {
    let new_vec = vec![8, 9, 0]; // 숫자들이 있는 vec

    let number_to_add = 5;       // 나중에 수학에서 사용합니다
    let mut empty_vec = vec![];  // 결과가 여기 들어갑니다


    for index in 0..5 {
        empty_vec.push(
            new_vec
               .get(index)
                .and_then(|number| Some(number + 1))
                .and_then(|number| Some(number + number_to_add))
        );
    }
    println!("{:?}", empty_vec);
}
```

이것은 `[Some(14), Some(15), Some(6), None, None]`을 출력합니다. `None`이 필터링되지 않고 그냥 전달된다는 것을 볼 수 있습니다.

`.and()`는 `Option`에 대한 `bool`과 같습니다. 많은 `Option`들을 서로 매치할 수 있고, 모두 `Some`이면 마지막 것을 줄 것입니다. 그 중 하나가 `None`이면, `None`을 줄 것입니다.

먼저 상상을 돕기 위한 `bool` 예시가 있습니다. `&&`(그리고)를 사용하고 있다면, 하나의 `false`라도 모든 것을 `false`로 만든다는 것을 볼 수 있습니다.

```rust
fn main() {
    let one = true;
    let two = false;
    let three = true;
    let four = true;

    println!("{}", one && three); // true를 출력합니다
    println!("{}", one && two && three && four); // false를 출력합니다
}
```

이제 `.and()`를 사용한 같은 것이 있습니다. 다섯 번의 작업을 했고 결과를 Vec<Option<&str>>에 넣었다고 상상해 봅시다. 값을 얻으면 vec에 `Some("success!")`을 푸시합니다. 그러면 이것을 두 번 더 합니다. 그 후에 `.and()`를 사용해서 매번 `Some`을 얻은 인덱스들만 보여줍니다.

```rust
fn main() {
    let first_try = vec![Some("success!"), None, Some("success!"), Some("success!"), None];
    let second_try = vec![None, Some("success!"), Some("success!"), Some("success!"), Some("success!")];
    let third_try = vec![Some("success!"), Some("success!"), Some("success!"), Some("success!"), None];

    for i in 0..first_try.len() {
        println!("{:?}", first_try[i].and(second_try[i]).and(third_try[i]));
    }
}
```

이것은 다음을 출력합니다:

```text
None
None
Some("success!")
Some("success!")
None
```

첫 번째(인덱스 0)는 `second_try`의 인덱스 0에 `None`이 있기 때문에 `None`입니다. 두 번째는 `first_try`에 `None`이 있기 때문에 `None`입니다. 다음은 `first_try`, `second_try`, 또는 `third_try`에 `None`이 없기 때문에 `Some("success!")`입니다.

`.any()`와 `.all()`은 반복자에서 사용하기 매우 쉽습니다. 입력에 따라 `bool`을 반환합니다. 이 예시에서 우리는 `'a'`부터 `'働'`까지의 모든 문자로 매우 큰 vec(약 20,000개 항목)을 만듭니다. 그러면 문자가 그 안에 있는지 확인하는 함수를 만듭니다.

다음에 우리는 더 작은 vec을 만들고 모든 것이 알파벳인지(`.is_alphabetic()` 메서드로) 묻습니다. 그러면 모든 문자가 한국어 문자 `'행'`보다 작은지 묻습니다.

또한 `.iter()`가 참조를 주고 다른 `&`와 비교하기 위해 `&`가 필요하기 때문에 참조를 넣는다는 것을 주목하세요.

```rust
fn in_char_vec(char_vec: &Vec<char>, check: char) {
    println!("Is {} inside? {}", check, char_vec.iter().any(|&char| char == check));
}

fn main() {
    let char_vec = ('a'..'働').collect::<Vec<char>>();
    in_char_vec(&char_vec, 'i');
    in_char_vec(&char_vec, '뷁');
    in_char_vec(&char_vec, '鑿');

    let smaller_vec = ('A'..'z').collect::<Vec<char>>();
    println!("All alphabetic? {}", smaller_vec.iter().all(|&x| x.is_alphabetic()));
    println!("All less than the character 행? {}", smaller_vec.iter().all(|&x| x < '행'));
}
```

이것은 다음을 출력합니다:

```text
Is i inside? true
Is 뷁 inside? false
Is 鑿 inside? false
All alphabetic? false
All less than the character 행? true
```

그런데 `.any()`는 일치하는 항목을 하나 찾을 때까지만 확인하고, 그러면 멈춥니다. 이미 일치하는 것을 찾았다면 모든 것을 확인하지 않을 것입니다. `Vec`에서 `.any()`를 사용할 예정이라면, 일치할 수 있는 항목들을 앞쪽 근처에 푸시하는 것이 좋은 아이디어일 수도 있습니다. 또는 `.iter()` 다음에 `.rev()`를 사용해서 반복자를 뒤집을 수 있습니다. 다음과 같은 vec이 있습니다:

```rust
fn main() {
    let mut big_vec = vec![6; 1000];
    big_vec.push(5);
}
```

따라서 이 `Vec`에는 1000개의 `6` 다음에 하나의 `5`가 있습니다. 5를 포함하는지 보기 위해 `.any()`를 사용하고 싶다고 가정해 봅시다. 먼저 `.rev()`가 작동하는지 확인해 봅시다. `Iterator`는 항상 매번 무엇을 하는지 확인하게 해주는 `.next()`를 가지고 있다는 것을 기억하세요.

```rust
fn main() {
    let mut big_vec = vec![6; 1000];
    big_vec.push(5);

    let mut iterator = big_vec.iter().rev();
    println!("{:?}", iterator.next());
    println!("{:?}", iterator.next());
}
```

이것은 다음을 출력합니다:

```text
Some(5)
Some(6)
```

우리가 맞았습니다: 하나의 `Some(5)`가 있고 그러면 1000개의 `Some(6)`이 시작합니다. 따라서 다음과 같이 쓸 수 있습니다:

```rust
fn main() {
    let mut big_vec = vec![6; 1000];
    big_vec.push(5);

    println!("{:?}", big_vec.iter().rev().any(|&number| number == 5));
}
```

그리고 `.rev()`이기 때문에, `.next()`를 한 번만 호출하고 멈춥니다. `.rev()`를 사용하지 않으면 멈추기 전에 `.next()`를 1001번 호출할 것입니다. 이 코드가 그것을 보여줍니다:

```rust
fn main() {
    let mut big_vec = vec![6; 1000];
    big_vec.push(5);

    let mut counter = 0; // 카운팅을 시작합니다
    let mut big_iter = big_vec.into_iter(); // Iterator로 만듭니다

    loop {
        counter +=1;
        if big_iter.next() == Some(5) { // Some(5)를 얻을 때까지 .next()를 계속 호출합니다
            break;
        }
    }
    println!("Final counter is: {}", counter);
}
```

이것은 `Final counter is: 1001`을 출력하므로 5를 찾기 전에 `.next()`를 1001번 호출해야 했다는 것을 알 수 있습니다.

`.find()`는 반복자가 무언가를 가지고 있는지 알려주고, `.position()`은 그것이 어디에 있는지 알려줍니다. `.find()`는 값이 들어있는 `Option`(또는 `None`)을 반환하기 때문에 `.any()`와 다릅니다. 한편, `.position()`도 위치 번호가 있는 `Option`이거나 `None`입니다. 다른 말로:

- `.find()`: "당신을 위해 그것을 얻으려고 시도하겠습니다"
- `.position()`: "당신을 위해 그것이 어디에 있는지 찾으려고 시도하겠습니다"

간단한 예시가 있습니다:

```rust
fn main() {
    let num_vec = vec![10, 20, 30, 40, 50, 60, 70, 80, 90, 100];

    println!("{:?}", num_vec.iter().find(|&number| number % 3 == 0)); // find는 참조를 받으므로 &number를 줍니다
    println!("{:?}", num_vec.iter().find(|&number| number * 2 == 30));

    println!("{:?}", num_vec.iter().position(|&number| number % 3 == 0));
    println!("{:?}", num_vec.iter().position(|&number| number * 2 == 30));

}
```

이것은 다음을 출력합니다:

```text
Some(30) // 이것은 숫자 자체입니다
None // 안에 있는 숫자에 2를 곱한 것 == 30인 것이 없습니다
Some(2) // 이것은 위치입니다
None
```

`.cycle()`로 영원히 반복하는 반복자를 만들 수 있습니다. 이 타입의 반복자는 `.zip()`와 잘 작동해서 새로운 것을 만듭니다. 이 예시처럼 `Vec<(i32, &str)>`을 만듭니다:

```rust
fn main() {
    let even_odd = vec!["even", "odd"];

    let even_odd_vec = (0..6)
        .zip(even_odd.into_iter().cycle())
        .collect::<Vec<(i32, &str)>>();
    println!("{:?}", even_odd_vec);
}
```

따라서 `.cycle()`이 절대 끝나지 않을 수도 있지만, 다른 반복자는 함께 압축할 때 여섯 번만 실행됩니다. 즉, `.cycle()`로 만들어진 반복자가 다시 `.next()` 호출을 받지 않으므로 여섯 번 후에 끝납니다. 출력은 다음과 같습니다:

```
[(0, "even"), (1, "odd"), (2, "even"), (3, "odd"), (4, "even"), (5, "odd")]
```

끝이 없는 범위로 비슷한 것을 할 수 있습니다. `0..`라고 쓰면 절대 멈추지 않는 범위를 만듭니다. 이것을 매우 쉽게 사용할 수 있습니다:

```rust
fn main() {
    let ten_chars = ('a'..).take(10).collect::<Vec<char>>();
    let skip_then_ten_chars = ('a'..).skip(1300).take(10).collect::<Vec<char>>();

    println!("{:?}", ten_chars);
    println!("{:?}", skip_then_ten_chars);
}
```

둘 다 열 개의 문자를 출력하지만, 두 번째는 1300곳을 건너뛰고 아르메니아어로 열 개의 글자를 출력합니다.

```
['a', 'b', 'c', 'd', 'e', 'f', 'g', 'h', 'i', 'j']
['յ', 'ն', 'շ', 'ո', 'չ', 'պ', 'ջ', 'ռ', 'ս', 'վ']
```

다른 인기 있는 메서드는 `.fold()`라고 불립니다. 이 메서드는 반복자의 항목들을 함께 더하는 데 많이 사용되지만, 훨씬 더 많은 것을 할 수도 있습니다. `.for_each()`와 다소 비슷합니다. `.fold()`에서는 먼저 시작 값(항목들을 함께 더하고 있다면 0)을 추가하고, 그러면 쉼표, 그러면 클로저를 추가합니다. 클로저는 두 개의 항목을 줍니다: 지금까지의 총합과 다음 항목. 먼저 항목들을 함께 더하기 위해 `.fold()`를 보여주는 간단한 예시가 있습니다.

```rust
fn main() {
    let some_numbers = vec![9, 6, 9, 10, 11];

    println!("{}", some_numbers
        .iter()
        .fold(0, |total_so_far, next_number| total_so_far + next_number)
    );
}
```

따라서:

- 1단계에서 0으로 시작하고 다음 숫자를 더합니다: 9.
- 그러면 그 9를 가져와서 6을 더합니다: 15.
- 그러면 그 15를 가져와서 9를 더합니다: 24.
- 그러면 그 24를 가져와서 10을 더합니다: 34.
- 마지막으로 그 34를 가져와서 11을 더합니다: 45. 따라서 `45`를 출력합니다.

하지만 그것으로 단지 것들을 더할 필요는 없습니다. 다음은 모든 문자에 '-'를 추가해서 `String`을 만드는 예시입니다.

```rust
fn main() {
    let a_string = "I don't have any dashes in me.";

    println!(
        "{}",
        a_string
            .chars() // 이제 반복자입니다
            .fold("-".to_string(), |mut string_so_far, next_char| { // String "-"로 시작합니다. 다음 char와 함께 매번 mutable로 가져옵니다
                string_so_far.push(next_char); // char를 푸시하고, 그러면 '-'를 푸시합니다
                string_so_far.push('-');
                string_so_far} // 다음 루프에 전달하는 것을 잊지 마세요
            ));
}
```

이것은 다음을 출력합니다:

```text
-I- -d-o-n-'-t- -h-a-v-e- -a-n-y- -d-a-s-h-e-s- -i-n- -m-e-.-
```

다음과 같은 많은 다른 편리한 메서드들이 있습니다:

- `.take_while()`: `true`를 얻는 동안 반복자에 받아들입니다(예를 들어 `take while x > 5`)
- `.cloned()`: 반복자 안에서 클론을 만듭니다. 이것은 참조를 값으로 바꿉니다.
- `.by_ref()`: 반복자가 참조를 받게 만듭니다. 반복자를 만들기 위해 사용한 후에 `Vec`이나 비슷한 것을 사용할 수 있는지 확인하는 데 좋습니다.
- 많은 다른 `_while` 메서드들: `.skip_while()`, `.map_while()`, 등등
- `.sum()`: 모든 것을 함께 더합니다.

`.chunks()`와 `.windows()`는 벡터를 원하는 크기로 자르는 두 가지 방법입니다. 원하는 크기를 괄호에 넣습니다. 10개의 항목이 있는 벡터가 있고 크기 3을 원한다고 해봅시다. 다음과 같이 작동할 것입니다:

- `.chunks()`는 네 개의 슬라이스를 줄 것입니다: [0, 1, 2], 그러면 [3, 4, 5], 그러면 [6, 7, 8], 그리고 마지막으로 [9]. 따라서 세 개 항목의 슬라이스를 만들려고 시도하지만, 세 개가 없다면 패닉하지 않을 것입니다. 남은 것을 줄 것입니다.
- `.windows()`는 먼저 [0, 1, 2]의 슬라이스를 줄 것입니다. 그러면 하나 이동해서 [1, 2, 3]을 줄 것입니다. 마지막 세 개의 슬라이스에 도달할 때까지 그렇게 할 것이고 멈출 것입니다.

따라서 간단한 숫자 벡터에서 사용해 봅시다. 다음과 같습니다:

```rust
fn main() {
    let num_vec = vec![1, 2, 3, 4, 5, 6, 7, 8, 9, 0];

    for chunk in num_vec.chunks(3) {
        println!("{:?}", chunk);
    }
    println!();
    for window in num_vec.windows(3) {
        println!("{:?}", window);
    }
}
```

이것은 다음을 출력합니다:

```text
[1, 2, 3]
[4, 5, 6]
[7, 8, 9]
[0]

[1, 2, 3]
[2, 3, 4]
[3, 4, 5]
[4, 5, 6]
[5, 6, 7]
[6, 7, 8]
[7, 8, 9]
[8, 9, 0]
```

그런데 `.chunks()`는 아무것도 주지 않으면 패닉할 것입니다. 한 개 항목이 있는 벡터에 대해 `.chunks(1000)`라고 쓸 수 있지만, 길이가 0인 것에 대해서는 `.chunks()`를 쓸 수 없습니다. [src]를 클릭하면 함수에서 그것을 볼 수 있는데 `assert!(chunk_size != 0);`라고 말하기 때문입니다.

`.match_indices()`는 입력과 일치하는 `String`이나 `&str` 안의 모든 것을 끌어내게 해주고, 인덱스도 줍니다. 두 개의 항목이 있는 튜플을 반환하기 때문에 `.enumerate()`와 비슷합니다.

```rust
fn main() {
    let rules = "Rule number 1: No fighting. Rule number 2: Go to bed at 8 pm. Rule number 3: Wake up at 6 am.";
    let rule_locations = rules.match_indices("Rule").collect::<Vec<(_, _)>>(); // 이것은 Vec<usize, &str>이지만 우리는 그냥 Rust가 하게 합니다
    println!("{:?}", rule_locations);
}
```

이것은 다음을 출력합니다:

```text
[(0, "Rule"), (28, "Rule"), (62, "Rule")]
```

`.peekable()`은 다음 항목을 볼 수 있는(엿볼 수 있는) 반복자를 만들게 해줍니다. 반복자가 움직이지 않는다는 점을 제외하고는 `.next()`를 호출하는 것과 같습니다(`Option`을 줍니다). 따라서 원하는 만큼 여러 번 사용할 수 있습니다. peekable을 "정지할 수 있는"이라고 생각할 수 있는데, 원하는 만큼 오래 멈출 수 있기 때문입니다. 다음은 모든 항목에 대해 `.peek()`를 세 번 사용하는 예시입니다. 다음 항목으로 이동하기 위해 `.next()`를 사용할 때까지 `.peek()`를 영원히 사용할 수 있습니다.

```rust
fn main() {
    let just_numbers = vec![1, 5, 100];
    let mut number_iter = just_numbers.iter().peekable(); // 이것은 실제로 Peekable이라고 불리는 반복자 타입을 만듭니다

    for _ in 0..3 {
        println!("I love the number {}", number_iter.peek().unwrap());
        println!("I really love the number {}", number_iter.peek().unwrap());
        println!("{} is such a nice number", number_iter.peek().unwrap());
        number_iter.next();
    }
}
```

이것은 다음을 출력합니다:

```text
I love the number 1
I really love the number 1
1 is such a nice number
I love the number 5
I really love the number 5
5 is such a nice number
I love the number 100
I really love the number 100
100 is such a nice number
```

다음은 `.peek()`를 사용해서 항목을 매치하는 다른 예시입니다. 사용을 마친 후에 `.next()`를 호출합니다.

```rust
fn main() {
    let locations = vec![
        ("Nevis", 25),
        ("Taber", 8428),
        ("Markerville", 45),
        ("Cardston", 3585),
    ];
    let mut location_iter = locations.iter().peekable();
    while location_iter.peek().is_some() {
        match location_iter.peek() {
            Some((name, number)) if *number < 100 => { // .peek()는 참조를 주므로 *가 필요합니다
                println!("Found a hamlet: {} with {} people", name, number)
            }
            Some((name, number)) => println!("Found a town: {} with {} people", name, number),
            None => break,
        }
        location_iter.next();
    }
}
```

이것은 다음을 출력합니다:

```text
Found a hamlet: Nevis with 25 people
Found a town: Taber with 8428 people
Found a hamlet: Markerville with 45 people
Found a town: Cardston with 3585 people
```

마지막으로, `.match_indices()`도 사용하는 예시가 있습니다. 이 예시에서 우리는 `&str`의 공백 수에 따라 이름들을 `struct`에 넣습니다.

```rust
#[derive(Debug)]
struct Names {
    one_word: Vec<String>,
    two_words: Vec<String>,
    three_words: Vec<String>,
}

fn main() {
    let vec_of_names = vec![
        "Caesar",
        "Frodo Baggins",
        "Bilbo Baggins",
        "Jean-Luc Picard",
        "Data",
        "Rand Al'Thor",
        "Paul Atreides",
        "Barack Hussein Obama",
        "Bill Jefferson Clinton",
    ];

    let mut iter_of_names = vec_of_names.iter().peekable();

    let mut all_names = Names { // 빈 Names 구조체를 시작합니다
        one_word: vec![],
        two_words: vec![],
        three_words: vec![],
    };

    while iter_of_names.peek().is_some() {
        let next_item = iter_of_names.next().unwrap(); // Some라는 것을 알고 있으므로 .unwrap()을 사용할 수 있습니다
        match next_item.match_indices(' ').collect::<Vec<_>>().len() { // .match_indices를 사용해서 빠른 vec을 만들고 길이를 확인합니다
            0 => all_names.one_word.push(next_item.to_string()),
            1 => all_names.two_words.push(next_item.to_string()),
            _ => all_names.three_words.push(next_item.to_string()),
        }
    }

    println!("{:?}", all_names);
}
```

이것은 다음을 출력할 것입니다:

```text
Names { one_word: ["Caesar", "Data"], two_words: ["Frodo Baggins", "Bilbo Baggins", "Jean-Luc Picard", "Rand Al'Thor", "Paul Atreides"], three_words:
["Barack Hussein Obama", "Bill Jefferson Clinton"] }
```

## dbg! 매크로와 .inspect

`dbg!`는 빠른 정보를 출력하는 매우 유용한 매크로입니다. 타이핑이 빠르고 더 많은 정보를 제공하기 때문에 `println!`의 좋은 대안입니다:

```rust
fn main() {
    let my_number = 8;
    dbg!(my_number);
}
```

이것은 `[src\main.rs:4] my_number = 8`을 출력합니다.

하지만 실제로는 `dbg!`를 다른 많은 곳에 넣을 수 있고, 심지어 코드를 감쌀 수도 있습니다. 예를 들어 이 코드를 보세요:

```rust
fn main() {
    let mut my_number = 9;
    my_number += 10;

    let new_vec = vec![8, 9, 10];

    let double_vec = new_vec.iter().map(|x| x * 2).collect::<Vec<i32>>();
}
```

이 코드는 새로운 가변 숫자를 만들고 그것을 변경합니다. 그런 다음 vec을 만들고, `iter`와 `map`과 `collect`를 사용해서 새로운 vec을 만듭니다. 우리는 이 코드의 거의 모든 곳에 `dbg!`를 넣을 수 있습니다. `dbg!`는 컴파일러에게 "지금 이 순간에 무엇을 하고 있나요?"라고 묻고 알려줍니다.

```rust
fn main() {
    let mut my_number = dbg!(9);
    dbg!(my_number += 10);

    let new_vec = dbg!(vec![8, 9, 10]);

    let double_vec = dbg!(new_vec.iter().map(|x| x * 2).collect::<Vec<i32>>());

    dbg!(double_vec);
}
```

그래서 이것은 다음을 출력합니다:

```text
[src\main.rs:3] 9 = 9
```

그리고:

```text
[src\main.rs:4] my_number += 10 = ()
```

그리고:

```text
[src\main.rs:6] vec![8, 9, 10] = [
    8,
    9,
    10,
]
```

그리고 이것도 있는데, 심지어 표현식의 값도 보여줍니다:

```text
[src\main.rs:8] new_vec.iter().map(|x| x * 2).collect::<Vec<i32>>() = [
    16,
    18,
    20,
]
```

그리고:

```text
[src\main.rs:10] double_vec = [
    16,
    18,
    20,
]
```

`.inspect`는 `dbg!`와 조금 비슷하지만 반복자에서 `map`처럼 사용합니다. 반복자 아이템을 제공하고 그것을 출력하거나 원하는 무엇이든 할 수 있습니다. 예를 들어, 다시 우리의 `double_vec`을 보겠습니다.

```rust
fn main() {
    let new_vec = vec![8, 9, 10];

    let double_vec = new_vec
        .iter()
        .map(|x| x * 2)
        .collect::<Vec<i32>>();
}
```

코드가 무엇을 하고 있는지 더 많은 정보를 알고 싶습니다. 그래서 두 곳에 `inspect()`를 추가합니다:

```rust
fn main() {
    let new_vec = vec![8, 9, 10];

    let double_vec = new_vec
        .iter()
        .inspect(|first_item| println!("The item is: {}", first_item))
        .map(|x| x * 2)
        .inspect(|next_item| println!("Then it is: {}", next_item))
        .collect::<Vec<i32>>();
}
```

이것은 다음을 출력합니다:

```text
The item is: 8
Then it is: 16
The item is: 9
Then it is: 18
The item is: 10
Then it is: 20
```

그리고 `.inspect`는 클로저를 받기 때문에, 원하는 만큼 쓸 수 있습니다:

```rust
fn main() {
    let new_vec = vec![8, 9, 10];

    let double_vec = new_vec
        .iter()
        .inspect(|first_item| {
            println!("The item is: {}", first_item);
            match **first_item % 2 { // first_item은 &&i32이므로 **를 사용합니다
                0 => println!("It is even."),
                _ => println!("It is odd."),
            }
            println!("In binary it is {:b}.", first_item);
        })
        .map(|x| x * 2)
        .collect::<Vec<i32>>();
}
```

이것은 다음을 출력합니다:

```text
The item is: 8
It is even.
In binary it is 1000.
The item is: 9
It is odd.
In binary it is 1001.
The item is: 10
It is even.
In binary it is 1010.
```

## &str의 타입들

`&str`에는 한 가지 이상의 타입이 있습니다. 우리에게는 다음이 있습니다:

- 문자열 리터럴: `let my_str = "I am a &str"`라고 쓸 때 이것들을 만듭니다. 이것들은 바이너리에 직접 쓰여지기 때문에 전체 프로그램 동안 지속됩니다. 이것들은 `&'static str` 타입을 가집니다. `'`는 그것의 수명을 의미하고, 문자열 리터럴은 `static`이라고 불리는 수명을 가집니다.
- 빌려온 str: 이것은 `static` 수명이 없는 일반적인 `&str` 형태입니다. `String`을 만들고 그것에 대한 참조를 얻으면, 필요할 때 Rust가 그것을 `&str`로 변환할 것입니다. 예를 들어:

```rust
fn prints_str(my_str: &str) { // &String을 &str처럼 사용할 수 있습니다
    println!("{}", my_str);
}

fn main() {
    let my_string = String::from("I am a string");
    prints_str(&my_string); // prints_str에 &String을 줍니다
}
```

그래서 수명이 무엇일까요? 이제 그것을 배워보겠습니다.

## 수명(Lifetimes)

수명은 "변수가 얼마나 오래 사는가"를 의미합니다. 참조와 함께일 때만 수명에 대해 생각하면 됩니다. 이것은 참조가 그들이 오는 객체보다 더 오래 살 수 없기 때문입니다. 예를 들어, 이 함수는 작동하지 않습니다:

```rust
fn returns_reference() -> &str {
    let my_string = String::from("I am a string");
    &my_string // ⚠️
}

fn main() {}
```

문제는 `my_string`이 `returns_reference` 안에서만 산다는 것입니다. 우리는 `&my_string`을 반환하려고 하지만, `&my_string`은 `my_string` 없이는 존재할 수 없습니다. 그래서 컴파일러는 안 된다고 말합니다.

이 코드도 작동하지 않습니다:

```rust
fn returns_str() -> &str {
    let my_string = String::from("I am a string");
    "I am a str" // ⚠️
}

fn main() {
    let my_str = returns_str();
    println!("{}", my_str);
}
```

하지만 거의 작동합니다. 컴파일러는 말합니다:

```text
error[E0106]: missing lifetime specifier
 --> src\main.rs:6:21
  |
6 | fn returns_str() -> &str {
  |                     ^ expected named lifetime parameter
  |
  = help: this function's return type contains a borrowed value, but there is no value for it to be borrowed from
help: consider using the `'static` lifetime
  |
6 | fn returns_str() -> &'static str {
  |                     ^^^^^^^^
```

`missing lifetime specifier`는 우리가 수명과 함께 `'`를 추가해야 한다는 것을 의미합니다. 그런 다음 그것은 `contains a borrowed value, but there is no value for it to be borrowed from`라고 말합니다. 그것은 `I am a str`이 어떤 것으로부터도 빌려오지 않았다는 것을 의미합니다. 그것은 `&'static str`을 쓰는 것으로 `consider using the 'static lifetime`라고 말합니다. 그래서 그것은 우리가 이것이 문자열 리터럴이라고 말해야 한다고 생각합니다.

이제 작동합니다:

```rust
fn returns_str() -> &'static str {
    let my_string = String::from("I am a string");
    "I am a str"
}

fn main() {
    let my_str = returns_str();
    println!("{}", my_str);
}
```

그것은 우리가 `static`의 수명을 가진 `&str`을 반환했기 때문입니다. 한편, `my_string`은 `String`으로만 반환될 수 있습니다: 그것은 다음 줄에서 죽을 것이기 때문에 그것에 대한 참조를 반환할 수 없습니다.

그래서 이제 `fn returns_str() -> &'static str`은 Rust에게 말합니다: "걱정하지 마세요, 우리는 문자열 리터럴만 반환할 것입니다". 문자열 리터럴은 전체 프로그램 동안 살기 때문에, Rust는 행복합니다. 이것이 제네릭과 비슷하다는 것을 알아차릴 것입니다. 컴파일러에게 `<T: Display>`와 같은 것을 말할 때, 우리는 `Display`를 가진 입력만 사용할 것이라고 약속합니다. 수명은 비슷합니다: 우리는 어떤 변수 수명도 바꾸지 않습니다. 우리는 단지 컴파일러에게 입력의 수명이 무엇일지 말하고 있습니다.

하지만 `'static`이 유일한 수명은 아닙니다. 실제로, 모든 변수는 수명을 가지지만, 보통 우리는 그것을 쓸 필요가 없습니다. 컴파일러는 꽤 똑똑하고 보통 스스로 알아낼 수 있습니다. 컴파일러가 모를 때만 수명을 써야 합니다.

다른 수명의 예시가 여기 있습니다. `City` 구조체를 만들고 이름에 `&str`을 주고 싶다고 상상해보세요. `String`보다 더 빠른 성능을 제공하기 때문에 그렇게 하고 싶을지도 모릅니다. 그래서 이렇게 쓰지만, 아직 작동하지 않을 것입니다:

```rust
#[derive(Debug)]
struct City {
    name: &str, // ⚠️
    date_founded: u32,
}

fn main() {
    let my_city = City {
        name: "Ichinomiya",
        date_founded: 1921,
    };
}
```

컴파일러는 말합니다:

```text
error[E0106]: missing lifetime specifier
 --> src\main.rs:3:11
  |
3 |     name: &str,
  |           ^ expected named lifetime parameter
  |
help: consider introducing a named lifetime parameter
  |
2 | struct City<'a> {
3 |     name: &'a str,
  |
```

Rust는 `&str`이 참조이기 때문에 `&str`에 대한 수명이 필요합니다. `name`이 가리키는 값이 삭제되면 어떻게 될까요? 그것은 안전하지 않을 것입니다.

`'static`은 어떨까요, 그것이 작동할까요? 우리는 전에 그것을 사용했습니다. 시도해보겠습니다:

```rust
#[derive(Debug)]
struct City {
    name: &'static str, // &str을 &'static str로 변경
    date_founded: u32,
}

fn main() {
    let my_city = City {
        name: "Ichinomiya",
        date_founded: 1921,
    };

    println!("{} was founded in {}", my_city.name, my_city.date_founded);
}
```

좋습니다, 그것이 작동합니다. 그리고 아마 이것이 구조체에 대해 당신이 원했던 것일지도 모릅니다. 하지만, 우리는 "문자열 리터럴"만 받을 수 있다는 것을 주목하세요, 그래서 다른 것에 대한 참조는 안 됩니다. 그래서 이것은 작동하지 않을 것입니다:

```rust
#[derive(Debug)]
struct City {
    name: &'static str, // 전체 프로그램 동안 살아야 합니다
    date_founded: u32,
}

fn main() {
    let city_names = vec!["Ichinomiya".to_string(), "Kurume".to_string()]; // city_names는 전체 프로그램 동안 살지 않습니다

    let my_city = City {
        name: &city_names[0], // ⚠️ 이것은 &str이지만 &'static str이 아닙니다. 이것은 city_names 안의 값에 대한 참조입니다
        date_founded: 1921,
    };

    println!("{} was founded in {}", my_city.name, my_city.date_founded);
}
```

컴파일러는 말합니다:

```text
error[E0597]: `city_names` does not live long enough
  --> src\main.rs:12:16
   |
12 |         name: &city_names[0],
   |                ^^^^^^^^^^
   |                |
   |                borrowed value does not live long enough
   |                requires that `city_names` is borrowed for `'static`
...
18 | }
   | - `city_names` dropped here while still borrowed
```

이것은 이해하기 중요합니다, 왜냐하면 우리가 준 참조는 실제로 충분히 오래 살기 때문입니다. 하지만 우리는 `&'static str`만 줄 것이라고 약속했고, 그것이 문제입니다.

그래서 이제 컴파일러가 전에 제안한 것을 시도해보겠습니다. 그것은 `struct City<'a>`와 `name: &'a str`을 쓰라고 말했습니다. 이것은 `City`만큼 오래 산다면 `name`에 대한 참조만 받을 것이라는 의미입니다.

```rust
#[derive(Debug)]
struct City<'a> { // City는 수명 'a를 가집니다
    name: &'a str, // 그리고 name도 수명 'a를 가집니다.
    date_founded: u32,
}

fn main() {
    let city_names = vec!["Ichinomiya".to_string(), "Kurume".to_string()];

    let my_city = City {
        name: &city_names[0],
        date_founded: 1921,
    };

    println!("{} was founded in {}", my_city.name, my_city.date_founded);
}
```

또한 원한다면 `'a` 대신 무엇이든 쓸 수 있다는 것을 기억하세요. 이것은 또한 `T`와 `U`를 쓰지만 실제로 무엇이든 쓸 수 있는 제네릭과 비슷합니다.

```rust
#[derive(Debug)]
struct City<'city> { // 수명은 이제 'city라고 불립니다
    name: &'city str, // 그리고 name은 'city 수명을 가집니다
    date_founded: u32,
}

fn main() {}
```

그래서 보통 당신은 `'a, 'b, 'c` 등을 쓸 것입니다 왜냐하면 그것이 빠르고 쓰는 일반적인 방법이기 때문입니다. 하지만 원한다면 언제든 바꿀 수 있습니다. 하나의 좋은 팁은 수명을 "인간이 읽기 쉬운" 이름으로 바꾸는 것이 매우 복잡한 코드를 읽는데 도움이 될 수 있다는 것입니다.

제네릭에 대한 트레이트와의 비교를 다시 보겠습니다. 예를 들어:

```rust
use std::fmt::Display;

fn prints<T: Display>(input: T) {
    println!("T is {}", input);
}

fn main() {}
```

`T: Display`를 쓸 때, 그것은 "Display를 가지고 있다면 T만 받아주세요"를 의미합니다.
그것은 "나는 T에게 Display를 주고 있습니다"를 의미하지 않습니다.

수명도 마찬가지입니다. 여기서 'a를 쓸 때:

```rust
#[derive(Debug)]
struct City<'a> {
    name: &'a str,
    date_founded: u32,
}

fn main() {}
```

그것은 "`name`이 최소한 `City`만큼 오래 산다면 `name`에 대한 입력만 받아주세요"를 의미합니다.
그것은 "나는 `name`에 대한 입력이 `City`만큼 오래 살도록 만들 것입니다"를 의미하지 않습니다.

이제 우리가 전에 본 `<'_>`에 대해 배울 수 있습니다. 이것은 "익명 수명"이라고 불리고 참조가 사용되고 있다는 표시자입니다. 예를 들어 구조체를 구현할 때 Rust가 그것을 제안할 것입니다. 여기 거의 작동하지만 아직은 아닌 하나의 구조체가 있습니다:

```rust
    // ⚠️
struct Adventurer<'a> {
    name: &'a str,
    hit_points: u32,
}

impl Adventurer {
    fn take_damage(&mut self) {
        self.hit_points -= 20;
        println!("{} has {} hit points left!", self.name, self.hit_points);
    }
}

fn main() {}
```

그래서 우리는 `struct`에 대해 해야 할 것을 했습니다: 먼저 우리는 `name`이 `&str`에서 온다고 말했습니다. 그것은 수명이 필요하다는 것을 의미하므로, 우리는 그것에 `<'a>`를 주었습니다. 그런 다음 우리는 그들이 최소한 이 수명만큼 길다는 것을 보여주기 위해 `struct`에 대해서도 같은 것을 해야 했습니다. 하지만 그런 다음 Rust는 우리에게 이것을 하라고 말합니다:

```text
error[E0726]: implicit elided lifetime not allowed here
 --> src\main.rs:6:6
  |
6 | impl Adventurer {
  |      ^^^^^^^^^^- help: indicate the anonymous lifetime: `<'_>`
```

그것은 참조가 사용되고 있다는 것을 보여주기 위해 그 익명 수명을 추가하기를 원합니다. 그래서 그것을 쓰면, 행복할 것입니다:

```rust
struct Adventurer<'a> {
    name: &'a str,
    hit_points: u32,
}

impl Adventurer<'_> {
    fn take_damage(&mut self) {
        self.hit_points -= 20;
        println!("{} has {} hit points left!", self.name, self.hit_points);
    }
}

fn main() {}
```

이 수명은 구조체가 이미 수명을 보여주기 때문에 항상 `impl<'a> Adventurer<'a>`와 같은 것을 쓸 필요가 없도록 만들어졌습니다.

Rust에서 수명은 어려울 수 있지만, 그것들에 대해 너무 스트레스받지 않기 위한 몇 가지 팁이 있습니다:

- 당분간 그것들을 피하고 싶다면, 소유된 타입을 그대로 두고, 클론을 사용하는 등을 할 수 있습니다.
- 대부분의 경우, 컴파일러가 수명을 원할 때 당신은 결국 여기저기에 <'a>를 쓰게 되고 그러면 작동할 것입니다. 그것은 단지 "걱정하지 마세요, 충분히 오래 살지 않는 것은 주지 않을 것입니다"라고 말하는 방법입니다.
- 한 번에 조금씩 수명을 탐구할 수 있습니다. 소유된 값들로 코드를 쓰고, 그런 다음 하나를 참조로 만드세요. 컴파일러는 불평하기 시작하지만, 몇 가지 제안도 줄 것입니다. 그리고 너무 복잡해지면, 되돌리고 다음에 다시 시도할 수 있습니다.

우리 코드로 이것을 해보고 컴파일러가 무엇을 말하는지 보겠습니다. 먼저 뒤로 가서 수명을 빼고, `Display`도 구현할 것입니다. `Display`는 단지 `Adventurer`의 이름을 출력할 것입니다.

```rust
// ⚠️
struct Adventurer {
    name: &str,
    hit_points: u32,
}

impl Adventurer {
    fn take_damage(&mut self) {
        self.hit_points -= 20;
        println!("{} has {} hit points left!", self.name, self.hit_points);
    }
}

impl std::fmt::Display for Adventurer {
        fn fmt(&self, f: &mut std::fmt::Formatter<'_>) -> std::fmt::Result {
            write!(f, "{} has {} hit points.", self.name, self.hit_points)
        }
}

fn main() {}
```

첫 번째 불만은 이것입니다:

```text
error[E0106]: missing lifetime specifier
 --> src\main.rs:2:11
  |
2 |     name: &str,
  |           ^ expected named lifetime parameter
  |
help: consider introducing a named lifetime parameter
  |
1 | struct Adventurer<'a> {
2 |     name: &'a str,
  |
```

그것은 무엇을 할지 제안합니다: Adventurer 뒤에 `<'a>`, 그리고 `&'a str`. 그래서 우리는 그것을 합니다:

```rust
// ⚠️
struct Adventurer<'a> {
    name: &'a str,
    hit_points: u32,
}

impl Adventurer {
    fn take_damage(&mut self) {
        self.hit_points -= 20;
        println!("{} has {} hit points left!", self.name, self.hit_points);
    }
}

impl std::fmt::Display for Adventurer {
        fn fmt(&self, f: &mut std::fmt::Formatter<'_>) -> std::fmt::Result {
            write!(f, "{} has {} hit points.", self.name, self.hit_points)
        }
}

fn main() {}
```

이제 그것은 그 부분들에 대해 행복하지만, `impl` 블록들에 대해 궁금해합니다. 그것은 우리가 참조를 사용하고 있다는 것을 언급하기를 원합니다:

```text
error[E0726]: implicit elided lifetime not allowed here
 --> src\main.rs:6:6
  |
6 | impl Adventurer {
  |      ^^^^^^^^^^- help: indicate the anonymous lifetime: `<'_>`

error[E0726]: implicit elided lifetime not allowed here
 --> src\main.rs:12:28
   |
12 | impl std::fmt::Display for Adventurer {
   |                            ^^^^^^^^^^- help: indicate the anonymous lifetime: `<'_>`
```

좋습니다, 그래서 우리는 그것들을 써넣을 것입니다...그리고 이제 작동합니다! 이제 우리는 `Adventurer`를 만들고 그것으로 몇 가지를 할 수 있습니다.

```rust
struct Adventurer<'a> {
    name: &'a str,
    hit_points: u32,
}

impl Adventurer<'_> {
    fn take_damage(&mut self) {
        self.hit_points -= 20;
        println!("{} has {} hit points left!", self.name, self.hit_points);
    }
}

impl std::fmt::Display for Adventurer<'_> {

        fn fmt(&self, f: &mut std::fmt::Formatter<'_>) -> std::fmt::Result {
            write!(f, "{} has {} hit points.", self.name, self.hit_points)
        }
}

fn main() {
    let mut billy = Adventurer {
        name: "Billy",
        hit_points: 100_000,
    };
    println!("{}", billy);
    billy.take_damage();
}
```

이것은 다음을 출력합니다:

```text
Billy has 100000 hit points.
Billy has 99980 hit points left!
```

그래서 수명이 종종 단지 컴파일러가 확실하게 하고 싶어하는 것이라는 것을 볼 수 있습니다. 그리고 그것은 보통 당신이 원하는 수명을 거의 추측할 만큼 똑똑하고, 단지 당신이 그것에게 말해주어서 확실할 수 있기를 원합니다.

## 내부 가변성(Interior mutability)

### Cell

**내부 가변성**은 안쪽에 조금의 가변성을 갖는 것을 의미합니다. Rust에서 변수를 바꾸려면 `mut`을 사용해야 한다는 것을 기억하세요? `mut`이라는 단어 없이도 그것들을 바꾸는 몇 가지 방법들이 있습니다. 이것은 Rust가 불변인 구조체 안의 값들을 안전하게 바꿀 수 있게 해주는 몇 가지 방법들을 가지고 있기 때문입니다. 그것들 각각은 값들을 바꾸는 것이 여전히 안전하다는 것을 확실하게 하는 몇 가지 규칙들을 따릅니다.

먼저, 우리가 이것을 원할 간단한 예시를 보겠습니다. 많은 필드를 가진 `PhoneModel`이라고 불리는 `struct`를 상상해보세요:

```rust
struct PhoneModel {
    company_name: String,
    model_name: String,
    screen_size: f32,
    memory: usize,
    date_issued: u32,
    on_sale: bool,
}

fn main() {
    let super_phone_3000 = PhoneModel {
        company_name: "YY Electronics".to_string(),
        model_name: "Super Phone 3000".to_string(),
        screen_size: 7.5,
        memory: 4_000_000,
        date_issued: 2020,
        on_sale: true,
    };

}
```

`PhoneModel`의 필드들이 불변인 것이 더 좋습니다, 왜냐하면 우리는 데이터가 바뀌는 것을 원하지 않기 때문입니다. 예를 들어, `date_issued`와 `screen_size`는 절대 바뀌지 않습니다.

하지만 안에는 `on_sale`이라고 불리는 하나의 필드가 있습니다. 폰 모델은 먼저 판매중일 것이고 (`true`), 하지만 나중에 회사는 그것을 판매하는 것을 중단할 것입니다. 우리가 이 하나의 필드만 가변으로 만들 수 있을까요? 왜냐하면 우리는 `let mut super_phone_3000`을 쓰고 싶지 않기 때문입니다. 우리가 그렇게 하면, 모든 필드가 가변이 될 것입니다.

Rust는 불변인 것 안에서 안전한 가변성을 허용하는 많은 방법들을 가지고 있습니다. 가장 간단한 방법은 `Cell`이라고 불립니다. 먼저 우리는 `use std::cell::Cell`을 사용해서 매번 `std::cell::Cell` 대신 `Cell`만 쓸 수 있도록 합니다.

그런 다음 우리는 `on_sale: bool`을 `on_sale: Cell<bool>`로 바꿉니다. 이제 그것은 bool이 아닙니다: 그것은 `bool`을 보유하는 `Cell`입니다.

`Cell`은 값을 바꿀 수 있는 `.set()`이라고 불리는 메서드를 가지고 있습니다. 우리는 `.set()`을 사용해서 `on_sale: true`를 `on_sale: Cell::new(true)`로 바꿉니다.

```rust
use std::cell::Cell;

struct PhoneModel {
    company_name: String,
    model_name: String,
    screen_size: f32,
    memory: usize,
    date_issued: u32,
    on_sale: Cell<bool>,
}

fn main() {
    let super_phone_3000 = PhoneModel {
        company_name: "YY Electronics".to_string(),
        model_name: "Super Phone 3000".to_string(),
        screen_size: 7.5,
        memory: 4_000_000,
        date_issued: 2020,
        on_sale: Cell::new(true),
    };

    // 10년 후, super_phone_3000은 더 이상 판매되지 않습니다
    super_phone_3000.on_sale.set(false);
}
```

`Cell`은 모든 타입에 작동하지만, 값을 주고 참조를 주지 않기 때문에 간단한 Copy 타입에 가장 잘 작동합니다. 예를 들어 `Cell`은 Copy 타입에만 작동하는 `get()`이라고 불리는 메서드를 가지고 있습니다.

당신이 사용할 수 있는 다른 타입은 `RefCell`입니다.

### RefCell

`RefCell`은 `mut`을 선언할 필요 없이 값들을 바꾸는 다른 방법입니다. 그것은 "reference cell"을 의미하고, `Cell`과 같지만 복사 대신 참조를 사용합니다.

우리는 `User` 구조체를 만들 것입니다. 지금까지 당신은 그것이 `Cell`과 비슷하다는 것을 볼 수 있습니다:

```rust
use std::cell::RefCell;

#[derive(Debug)]
struct User {
    id: u32,
    year_registered: u32,
    username: String,
    active: RefCell<bool>,
    // 많은 다른 필드들
}

fn main() {
    let user_1 = User {
        id: 1,
        year_registered: 2020,
        username: "User 1".to_string(),
        active: RefCell::new(true),
    };

    println!("{:?}", user_1.active);
}
```

이것은 `RefCell { value: true }`를 출력합니다.

`RefCell`에는 많은 메서드들이 있습니다. 그 중 두 개는 `.borrow()`와 `.borrow_mut()`입니다. 이 메서드들로, 당신은 `&`와 `&mut`으로 하는 것과 같은 것을 할 수 있습니다. 규칙들은 같습니다:

- 많은 대여는 괜찮습니다,
- 하나의 가변 대여는 괜찮습니다,
- 하지만 가변과 불변을 함께 하는 것은 괜찮지 않습니다.

그래서 `RefCell`에서 값을 바꾸는 것은 매우 쉽습니다:

```rust
// 🚧
user_1.active.replace(false);
println!("{:?}", user_1.active);
```

그리고 클로저를 사용하는 `replace_with`와 같은 많은 다른 메서드들이 있습니다:

```rust
// 🚧
let date = 2020;

user_1
    .active
    .replace_with(|_| if date < 2000 { true } else { false });
println!("{:?}", user_1.active);
```

하지만 `RefCell`을 조심해야 합니다, 왜냐하면 그것은 컴파일 시간이 아닌 런타임에 대여를 확인하기 때문입니다. 런타임은 프로그램이 실제로 실행될 때(컴파일 후)를 의미합니다. 그래서 이것은 틀렸음에도 불구하고 컴파일될 것입니다:

```rust
use std::cell::RefCell;

#[derive(Debug)]
struct User {
    id: u32,
    year_registered: u32,
    username: String,
    active: RefCell<bool>,
    // 많은 다른 필드들
}

fn main() {
    let user_1 = User {
        id: 1,
        year_registered: 2020,
        username: "User 1".to_string(),
        active: RefCell::new(true),
    };

    let borrow_one = user_1.active.borrow_mut(); // 첫 번째 가변 대여 - 괜찮습니다
    let borrow_two = user_1.active.borrow_mut(); // 두 번째 가변 대여 - 괜찮지 않습니다
}
```

하지만 그것을 실행하면, 즉시 패닉할 것입니다.

```text
thread 'main' panicked at 'already borrowed: BorrowMutError', C:\Users\mithr\.rustup\toolchains\stable-x86_64-pc-windows-msvc\lib/rustlib/src/rust\src\libcore\cell.rs:877:9
note: run with `RUST_BACKTRACE=1` environment variable to display a backtrace
error: process didn't exit successfully: `target\debug\rust_book.exe` (exit code: 101)
```

`already borrowed: BorrowMutError`가 중요한 부분입니다. 그래서 `RefCell`을 사용할 때, 컴파일**과** 실행 둘 다 해서 확인하는 것이 좋습니다.

### Mutex

`Mutex`는 `mut`을 선언하지 않고 값들을 바꾸는 다른 방법입니다. Mutex는 `mutual exclusion`을 의미하고, 이것은 "한 번에 하나만"을 의미합니다. 이것이 `Mutex`가 안전한 이유입니다, 왜냐하면 그것은 한 번에 하나의 프로세스만 그것을 바꾸게 하기 때문입니다. 이것을 하기 위해, 그것은 `.lock()`을 사용합니다. `Lock`은 안쪽에서 문을 잠그는 것과 같습니다. 당신은 방에 들어가고, 문을 잠그고, 이제 방 안의 것들을 바꿀 수 있습니다. 당신이 문을 잠갔기 때문에 다른 누구도 들어와서 당신을 막을 수 없습니다.

`Mutex`는 예시를 통해 이해하기 더 쉽습니다.

```rust
use std::sync::Mutex;

fn main() {
    let my_mutex = Mutex::new(5); // 새로운 Mutex<i32>. 우리는 mut이라고 말할 필요가 없습니다
    let mut mutex_changer = my_mutex.lock().unwrap(); // mutex_changer는 MutexGuard입니다
                                                     // 우리가 그것을 바꿀 것이기 때문에 mut이어야 합니다
                                                     // 이제 그것은 Mutex에 접근할 수 있습니다
                                                     // my_mutex를 출력해서 보겠습니다:

    println!("{:?}", my_mutex); // 이것은 "Mutex { data: <locked> }"를 출력합니다
                                // 그래서 이제 my_mutex로는 데이터에 접근할 수 없고,
                                // mutex_changer로만 접근할 수 있습니다

    println!("{:?}", mutex_changer); // 이것은 5를 출력합니다. 6으로 바꿔보겠습니다.

    *mutex_changer = 6; // mutex_changer는 MutexGuard<i32>이므로 *를 사용해서 i32를 바꿉니다

    println!("{:?}", mutex_changer); // 이제 6이라고 말합니다
}
```

하지만 `mutex_changer`는 완료된 후에도 여전히 잠금을 가지고 있습니다. 우리가 그것을 어떻게 멈출까요? `Mutex`는 `MutexGuard`가 스코프를 벗어날 때 잠금이 해제됩니다. "스코프를 벗어난다"는 것은 코드 블록이 끝난다는 것을 의미합니다. 예를 들어:

```rust
use std::sync::Mutex;

fn main() {
    let my_mutex = Mutex::new(5);
    {
        let mut mutex_changer = my_mutex.lock().unwrap();
        *mutex_changer = 6;
    } // mutex_changer가 스코프를 벗어납니다 - 이제 사라집니다. 더 이상 잠겨있지 않습니다

    println!("{:?}", my_mutex); // 이제 다음이 나옵니다: Mutex { data: 6 }
}
```

다른 `{}` 코드 블록을 사용하고 싶지 않다면, `std::mem::drop(mutex_changer)`를 사용할 수 있습니다. `std::mem::drop`은 "이것을 스코프 밖으로 보내라"를 의미합니다.

```rust
use std::sync::Mutex;

fn main() {
    let my_mutex = Mutex::new(5);
    let mut mutex_changer = my_mutex.lock().unwrap();
    *mutex_changer = 6;
    std::mem::drop(mutex_changer); // mutex_changer를 드롭합니다 - 이제 사라집니다
                                   // 그리고 my_mutex는 잠금이 해제됩니다

    println!("{:?}", my_mutex); // 이제 다음이 나옵니다: Mutex { data: 6 }
}
```

`Mutex`를 조심해야 합니다 왜냐하면 다른 변수가 그것을 `lock`하려고 하면, 기다릴 것이기 때문입니다:

```rust
use std::sync::Mutex;

fn main() {
    let my_mutex = Mutex::new(5);
    let mut mutex_changer = my_mutex.lock().unwrap(); // mutex_changer가 잠금을 가지고 있습니다
    let mut other_mutex_changer = my_mutex.lock().unwrap(); // other_mutex_changer가 잠금을 원합니다
                                                            // 프로그램이 기다리고 있습니다
                                                            // 그리고 기다리고 있습니다
                                                            // 그리고 영원히 기다릴 것입니다.

    println!("This will never print...");
}
```

또 다른 메서드는 `try_lock()`입니다. 그러면 한 번 시도하고, 잠금을 얻지 못하면 포기할 것입니다. `try_lock().unwrap()`을 하지 마세요, 왜냐하면 작동하지 않으면 패닉할 것이기 때문입니다. `if let`이나 `match`가 더 좋습니다:

```rust
use std::sync::Mutex;

fn main() {
    let my_mutex = Mutex::new(5);
    let mut mutex_changer = my_mutex.lock().unwrap();
    let mut other_mutex_changer = my_mutex.try_lock(); // 잠금을 얻으려고 시도합니다

    if let Ok(value) = other_mutex_changer {
        println!("The MutexGuard has: {}", value)
    } else {
        println!("Didn't get the lock")
    }
}
```

또한, `Mutex`를 바꾸기 위해 변수를 만들 필요가 없습니다. 단지 이렇게 할 수 있습니다:

```rust
use std::sync::Mutex;

fn main() {
    let my_mutex = Mutex::new(5);

    *my_mutex.lock().unwrap() = 6;

    println!("{:?}", my_mutex);
}
```

`*my_mutex.lock().unwrap() = 6;`은 "my_mutex를 잠금 해제하고 6으로 만들어라"를 의미합니다. 그것을 보유하는 변수가 없으므로 `std::mem::drop`을 호출할 필요가 없습니다. 원한다면 100번 할 수 있습니다 - 상관없습니다:

```rust
use std::sync::Mutex;

fn main() {
    let my_mutex = Mutex::new(5);

    for _ in 0..100 {
        *my_mutex.lock().unwrap() += 1; // 100번 잠그고 잠금 해제합니다
    }

    println!("{:?}", my_mutex);
}
```

### RwLock

`RwLock`은 "read write lock"을 의미합니다. 그것은 `Mutex`와 같지만 `RefCell`과도 같습니다. 그것을 바꾸기 위해 `.lock().unwrap()` 대신 `.write().unwrap()`을 사용합니다. 하지만 읽기 접근을 얻기 위해 `.read().unwrap()`도 사용할 수 있습니다. 그것은 규칙들을 따르기 때문에 `RefCell`과 같습니다:

- 많은 `.read()` 변수들은 괜찮습니다,
- 하나의 `.write()` 변수는 괜찮습니다,
- 하지만 하나 이상의 `.write()`나 `.read()`와 `.write()`를 함께 하는 것은 괜찮지 않습니다.

접근을 얻을 수 없을 때 `.write()`를 시도하면 프로그램이 영원히 실행될 것입니다:

```rust
use std::sync::RwLock;

fn main() {
    let my_rwlock = RwLock::new(5);

    let read1 = my_rwlock.read().unwrap(); // 하나의 .read()는 괜찮습니다
    let read2 = my_rwlock.read().unwrap(); // 두 개의 .read()도 괜찮습니다

    println!("{:?}, {:?}", read1, read2);

    let write1 = my_rwlock.write().unwrap(); // 어 오, 이제 프로그램이 영원히 기다릴 것입니다
}
```

그래서 우리는 `Mutex`에서처럼 `std::mem::drop`을 사용합니다.

```rust
use std::sync::RwLock;
use std::mem::drop; // drop()을 많이 사용할 것입니다

fn main() {
    let my_rwlock = RwLock::new(5);

    let read1 = my_rwlock.read().unwrap();
    let read2 = my_rwlock.read().unwrap();

    println!("{:?}, {:?}", read1, read2);

    drop(read1);
    drop(read2); // 둘 다 드롭했으므로, 이제 .write()를 사용할 수 있습니다

    let mut write1 = my_rwlock.write().unwrap();
    *write1 = 6;
    drop(write1);
    println!("{:?}", my_rwlock);
}
```

그리고 `try_read()`와 `try_write()`도 사용할 수 있습니다.

```rust
use std::sync::RwLock;

fn main() {
    let my_rwlock = RwLock::new(5);

    let read1 = my_rwlock.read().unwrap();
    let read2 = my_rwlock.read().unwrap();

    if let Ok(mut number) = my_rwlock.try_write() {
        *number += 10;
        println!("Now the number is {}", number);
    } else {
        println!("Couldn't get write access, sorry!")
    };
}
```

## Cow

Cow는 매우 편리한 열거형입니다. 그것은 "clone on write"를 의미하고 `String`이 필요하지 않다면 `&str`을 반환하고, 필요하다면 `String`을 반환하게 해줍니다. (그것은 배열 대 벡터 등에도 같은 것을 할 수 있습니다.)

그것을 이해하기 위해, 시그니처를 보겠습니다. 그것은 말합니다:

```rust
pub enum Cow<'a, B>
where
    B: 'a + ToOwned + ?Sized,
 {
    Borrowed(&'a B),
    Owned(<B as ToOwned>::Owned),
}

fn main() {}
```

`'a`가 참조와 함께 작동한다는 것을 바로 알 수 있습니다. `ToOwned` 트레이트는 소유된 타입으로 바뀔 수 있는 타입이라는 것을 의미합니다. 예를 들어, `str`은 보통 참조(`&str`)이고 그것을 소유된 `String`으로 바꿀 수 있습니다.

다음은 `?Sized`입니다. 이것은 "아마 Sized이지만, 아닐 수도 있다"를 의미합니다. Rust의 거의 모든 타입은 Sized이지만, `str`과 같은 타입들은 그렇지 않습니다. 그것이 `str`에 `&`가 필요한 이유입니다, 왜냐하면 컴파일러가 크기를 모르기 때문입니다. 그래서 `str`과 같은 것을 사용할 수 있는 트레이트를 원한다면, `?Sized`를 추가합니다.

다음은 `enum` 변형들입니다. 그것들은 `Borrowed`와 `Owned`입니다.

`Cow<'static, str>`을 반환하는 함수가 있다고 상상해보세요. 함수에게 `"My message".into()`를 반환하라고 말하면, 그것은 타입을 볼 것입니다: "My message"는 `str`입니다. 이것은 `Borrowed` 타입이므로, 그것은 `Borrowed(&'a B)`를 선택합니다. 그래서 그것은 `Cow::Borrowed(&'static str)`이 됩니다.

그리고 `format!("{}", "My message").into()`를 준다면 그것은 타입을 볼 것입니다. 이번에는 `String`입니다, 왜냐하면 `format!`이 `String`을 만들기 때문입니다. 그래서 이번에는 "Owned"를 선택할 것입니다.

`Cow`를 테스트하는 예시가 여기 있습니다. 우리는 `Cow<'static, str>`을 반환하는 함수에 숫자를 넣을 것입니다. 숫자에 따라, 그것은 `&str`이나 `String`을 만들 것입니다. 그런 다음 그것은 `.into()`를 사용해서 그것을 `Cow`로 바꿉니다. 그렇게 할 때, 그것은 `Cow::Borrowed`나 `Cow::Owned` 중 하나를 선택할 것입니다. 그런 다음 우리는 어느 것을 선택했는지 보기 위해 매치할 것입니다.

```rust
use std::borrow::Cow;

fn modulo_3(input: u8) -> Cow<'static, str> {
    match input % 3 {
        0 => "Remainder is 0".into(),
        1 => "Remainder is 1".into(),
        remainder => format!("Remainder is {}", remainder).into(),
    }
}

fn main() {
    for number in 1..=6 {
        match modulo_3(number) {
            Cow::Borrowed(message) => println!("{} went in. The Cow is borrowed with this message: {}", number, message),
            Cow::Owned(message) => println!("{} went in. The Cow is owned with this message: {}", number, message),
        }
    }
}
```

이것은 다음을 출력합니다:

```text
1 went in. The Cow is borrowed with this message: Remainder is 1
2 went in. The Cow is owned with this message: Remainder is 2
3 went in. The Cow is borrowed with this message: Remainder is 0
4 went in. The Cow is borrowed with this message: Remainder is 1
5 went in. The Cow is owned with this message: Remainder is 2
6 went in. The Cow is borrowed with this message: Remainder is 0
```

`Cow`는 필요하다면 그것을 바꿀 수 있는 `into_owned`나 `into_borrowed`와 같은 몇 가지 다른 메서드들을 가지고 있습니다.

## 타입 별명(Type aliases)

타입 별명은 "다른 타입에 새로운 이름을 주는 것"을 의미합니다. 타입 별명은 매우 쉽습니다. 보통 매우 긴 타입이 있고 매번 그것을 쓰고 싶지 않을 때 사용합니다. 또한 타입에 기억하기 쉬운 더 좋은 이름을 주고 싶을 때도 좋습니다. 여기 타입 별명의 두 가지 예시가 있습니다.

여기는 어렵지 않지만 다른 사람들(또는 당신)이 코드를 이해하기 쉽게 만들고 싶은 타입입니다:

```rust
type CharacterVec = Vec<char>;

fn main() {}
```

여기는 읽기 매우 어려운 타입입니다:

```rust
// 이 반환 타입은 극도로 깁니다
fn returns<'a>(input: &'a Vec<char>) -> std::iter::Take<std::iter::Skip<std::slice::Iter<'a, char>>> {
    input.iter().skip(4).take(5)
}

fn main() {}
```

그래서 당신은 그것을 이것으로 바꿀 수 있습니다:

```rust
type SkipFourTakeFive<'a> = std::iter::Take<std::iter::Skip<std::slice::Iter<'a, char>>>;

fn returns<'a>(input: &'a Vec<char>) -> SkipFourTakeFive {
    input.iter().skip(4).take(5)
}

fn main() {}
```

물론, 타입을 더 짧게 만들기 위해 아이템들을 가져올 수도 있습니다:

```rust
use std::iter::{Take, Skip};
use std::slice::Iter;

fn returns<'a>(input: &'a Vec<char>) -> Take<Skip<Iter<'a, char>>> {
    input.iter().skip(4).take(5)
}

fn main() {}
```

그래서 당신이 좋아하는 것에 따라 코드에서 무엇이 가장 잘 보이는지 결정할 수 있습니다.

이것이 실제 새로운 타입을 만들지 않는다는 것을 주목하세요. 그것은 단지 기존 타입 대신 사용할 이름일 뿐입니다. 그래서 `type File = String;`이라고 쓰면, 컴파일러는 단지 `String`을 봅니다. 그래서 이것은 `true`를 출력할 것입니다:

```rust
type File = String;

fn main() {
    let my_file = File::from("I am file contents");
    let my_string = String::from("I am file contents");
    println!("{}", my_file == my_string);
}
```

그래서 실제 새로운 타입을 원한다면 어떻게 할까요?

컴파일러가 `File`로 보는 새로운 파일 타입을 원한다면, 그것을 구조체에 넣을 수 있습니다. (이것은 실제로 `newtype` 관용구라고 불립니다)

```rust
struct File(String); // File은 String 주위의 래퍼입니다

fn main() {
    let my_file = File(String::from("I am file contents"));
    let my_string = String::from("I am file contents");
}
```

이제 이것은 작동하지 않을 것입니다, 왜냐하면 그것들은 두 개의 다른 타입이기 때문입니다:

```rust
struct File(String); // File은 String 주위의 래퍼입니다

fn main() {
    let my_file = File(String::from("I am file contents"));
    let my_string = String::from("I am file contents");
    println!("{}", my_file == my_string);  // ⚠️ File을 String과 비교할 수 없습니다
}
```

안의 String을 비교하고 싶다면, my_file.0을 사용할 수 있습니다:

```rust
struct File(String);

fn main() {
    let my_file = File(String::from("I am file contents"));
    let my_string = String::from("I am file contents");
    println!("{}", my_file.0 == my_string); // my_file.0은 String이므로, 이것은 true를 출력합니다
}
```

그리고 이제 이 타입은 어떤 트레이트도 가지지 않으므로, 당신이 직접 구현할 수 있습니다. 이것은 놀라운 일이 아닙니다:

```rust
#[derive(Clone, Debug)]
struct File(String);
```

그래서 여기서 `File` 타입을 사용할 때 그것을 복제하고 디버그 출력할 수 있지만, `.0`을 사용하여 안의 String을 가져오지 않는 한 String의 트레이트를 가지지 않습니다. 하지만 다른 사람들의 코드에서는 `pub`로 공개로 표시된 경우에만 `.0`을 사용할 수 있습니다. 그리고 이것이 이런 종류의 타입들이 `Deref` 트레이트를 많이 사용하는 이유입니다. `pub`과 `Deref` 모두에 대해 나중에 배울 것입니다.

### 함수 내에서 import와 이름 변경

보통 프로그램 맨 위에 `use`를 쓰는데, 다음과 같습니다:

```rust
use std::cell::{Cell, RefCell};

fn main() {}
```

하지만 어디에서나 이것을 할 수 있다는 것을 봤습니다, 특히 긴 이름을 가진 enum이 있는 함수에서 말이죠. 여기 예시가 있습니다.

```rust
enum MapDirection {
    North,
    NorthEast,
    East,
    SouthEast,
    South,
    SouthWest,
    West,
    NorthWest,
}

fn give_direction(direction: &MapDirection) {
    use MapDirection::*; // 이제 North, NorthEast 등을 직접 사용할 수 있습니다.
    let m = "You are going ";
    match direction {
        North => println!("{}{}", m, "north"),
        NorthEast => println!("{}{}", m, "northeast"),
        // 등등
        _ => println!("Not sure where you are going."),
    }
}

fn main() {
    let direction = MapDirection::North;
    give_direction(&direction);
}
```

그래서 함수 안에서 `use MapDirection::*`를 사용했고, 그래서 `MapDirection::North`를 쓰는 대신 `North`만 쓸 수 있습니다.

또한 `as`를 사용하여 이름을 바꿀 수도 있습니다. 예를 들어, 어쩌면 다른 함수에서 `println!`을 많이 사용하고 있어서 더 짧게 만들고 싶을 수도 있습니다:

```rust
fn main() {
    use std::fmt::Display as D; // 이제 Display를 D라고 부를 수 있습니다

    let my_string = "Hello there";
    let my_number = 9;
    print_it(my_string);
    print_it(my_number);
}

fn print_it<T: D>(data: T) {
    println!("{}", data)
}
```

## todo! 매크로

가끔 새로운 Rust 프로젝트를 시작하고 함수들의 구조를 써내려가고 싶지만 실제로 함수 본체를 쓰고 싶지 않을 때가 있습니다. 예를 들어, 다음과 같은 프로젝트를 상상해보세요:

```rust
struct Book {} // OK, 먼저 이 세 가지 구조체를 만들 것입니다
struct User {}
struct Library {}
impl Book {
    fn check_out(&self) {} // 사용자는 책을 빌릴 수 있어야 합니다
}

impl User {
    fn check_book(&self, book: &Book) {} // 사용자는 책을 확인할 수 있어야 합니다
}

impl Library {
    fn add_book(&self) {} // 우리는 도서관에 책을 추가할 수 있어야 합니다
    fn add_user(&self) {} // 우리는 도서관에 사용자를 추가할 수 있어야 합니다
}

fn main() {}
```

하지만 함수 안에 아무것도 없으면 컴파일러가 불만을 토로할 것입니다. 그것은 함수 안에 적어도 `()`를 줘야 한다고 말할 것입니다. 그래서 당신은 이렇게 쓸 수 있습니다:

```rust
fn check_out(&self) {}
fn check_book(&self, book: &Book) {}
fn add_book(&self) {}
fn add_user(&self) {}
```

하지만 `todo!`가 더 좋습니다. 왜냐하면 나중에 함수를 완성하는 것을 기억하게 해주기 때문입니다. 이 함수들을 실행하려고 하면, 프로그램이 패닉을 일으키고 "아직 구현되지 않음"이라고 말할 것입니다.

```rust
struct Book {}
struct User {}
struct Library {}
impl Book {
    fn check_out(&self) {
        todo!() // todo는 매크로이므로 ! 가 필요합니다
    }
}

impl User {
    fn check_book(&self, book: &Book) {
        todo!()
    }
}

impl Library {
    fn add_book(&self) {
        todo!()
    }
    fn add_user(&self) {
        todo!()
    }
}

fn main() {}
```

따라서 이것은 컴파일되지만 만약 함수 중 하나를 호출하려고 하면 크래시가 날 것입니다.

또한 `todo!` 안에 메시지를 넣을 수도 있습니다:

```rust
fn check_book(&self, book: &Book) {
    todo!("Here I need to check the book ID")
}
```

`todo!`는 실제로 `unimplemented!`와 같지만, 더 짧게 쓸 수 있습니다.

또한 `unreachable!()` 매크로도 있습니다. 이 매크로는 절대로 호출되어서는 안 되는 코드에 사용됩니다:

```rust
fn main() {
    let true_or_false = true;

    match true_or_false {
        true => println!("It's true"),
        false => println!("It's false"),
        _ => unreachable!(),
    }
}
```

이것은 `It's true`를 출력할 것입니다. `unreachable!()`는 절대로 호출되지 않을 것인데, 이미 `true`와 `false`를 다루었고 `_`에 대해서는 다른 가능성이 없기 때문입니다. 하지만 컴파일러는 여전히 모든 경우를 다루라고 하므로 `unreachable!()`를 써야 합니다.

이 매크로는 `todo!()`와 비슷하지만 절대로 하지 않을 코드에 사용됩니다. 어쩌면 enum에서 절대로 선택되지 않을 분기가 있는 `match`가 있을 수도 있습니다. 그래서 그 코드에 절대로 도달할 수 없습니다. 그런 경우, `unreachable!()`을 써서 컴파일러가 그 부분을 무시할 수 있다는 것을 알려줄 수 있습니다.

예를 들어, 당신이 살 곳을 선택할 때 뭔가를 쓰는 프로그램이 있다고 해봅시다. 그것들은 우크라이나에 있고, 모두 체르노빌을 제외하고는 좋습니다. 당신의 프로그램은 아무도 체르노빌을 선택할 수 없게 하는데, 지금 당장 살기에 좋은 곳이 아니기 때문입니다. 하지만 enum은 다른 누군가의 코드에서 오래 전에 만들어졌고, 당신은 그것을 바꿀 수 없습니다. 그래서 `match` 분기에서 여기서 매크로를 사용할 수 있습니다. 다음과 같이 보입니다:

```rust
enum UkrainePlaces {
    Kiev,
    Kharkiv,
    Chernobyl, // enum을 바꿀 수 없다고 가정합니다 - 체르노빌은 항상 여기 있을 것입니다
    Odesa,
    Dnipro,
}

fn choose_city(place: &UkrainePlaces) {
    use UkrainePlaces::*;
    match place {
        Kiev => println!("You will live in Kiev"),
        Kharkiv => println!("You will live in Kharkiv"),
        Chernobyl => unreachable!(),
        Odesa => println!("You will live in Odesa"),
        Dnipro => println!("You will live in Dnipro"),
    }
}

fn main() {
    let user_input = UkrainePlaces::Kiev; // 사용자 입력이 다른 함수에서 만들어진다고 가정합니다. 사용자는 무엇을 하든 체르노빌을 선택할 수 없습니다
    choose_city(&user_input);
}
```

이것은 `You will live in Kiev`를 출력할 것입니다.

`unreachable!()`는 또한 읽기에도 좋은데, 코드의 일부 부분이 도달할 수 없다는 것을 상기시켜주기 때문입니다. 코드가 실제로 도달할 수 없다는 것을 확신해야 합니다. 컴파일러가 `unreachable!()`를 호출하면, 프로그램이 패닉을 일으킬 것입니다.

또한, 컴파일러가 알고 있는 도달할 수 없는 코드가 있다면, 그것을 알려줄 것입니다. 다음은 빠른 예시입니다:

```rust
fn main() {
    let true_or_false = true;

    match true_or_false {
        true => println!("It's true"),
        false => println!("It's false"),
        true => println!("It's true"), // 앗, true를 다시 썼습니다
    }
}
```

다음과 같이 말할 것입니다:

```text
warning: unreachable pattern
 --> src/main.rs:7:9
  |
7 |         true => println!("It's true"),
  |         ^^^^
  |
```

하지만 `unreachable!()`는 컴파일러가 알 수 없을 때를 위한 것입니다, 우리의 다른 예시처럼 말이죠.

## `column!`, `line!`, `file!`, `module_path!`

이 네 가지 매크로는 `dbg!()`와 비슷한데, 디버그 정보를 제공하기 위해 그냥 넣기 때문입니다. 하지만 그것들은 어떤 변수도 받지 않습니다 - 그냥 괄호와 함께 사용하고 다른 것은 없습니다. 함께 배우기 쉽습니다:

- `column!()`은 당신이 그것을 쓴 열을 제공합니다,
- `file!()`은 당신이 그것을 쓴 파일의 이름을 제공합니다,
- `line!()`은 당신이 그것을 쓴 줄을 제공합니다, 그리고
- `module_path!()`는 그것이 있는 모듈을 제공합니다.

다음 코드는 간단한 예시에서 모든 세 가지를 보여줍니다. 훨씬 더 많은 코드가 있다고 가정할 것입니다 (모듈 안의 모듈들), 이것이 우리가 이 매크로들을 사용하고 싶은 이유이기 때문입니다. 많은 모듈과 파일에 걸친 큰 Rust 프로그램을 상상할 수 있습니다.

```rust
pub mod something {
    pub mod third_mod {
        pub fn print_a_country(input: &mut Vec<&str>) {
            println!(
                "The last country is {} inside the module {}",
                input.pop().unwrap(),
                module_path!()
            );
        }
    }
}

fn main() {
    use something::third_mod::*;
    let mut country_vec = vec!["Portugal", "Czechia", "Finland"];

    // 이것들을 출력해봅시다
    println!("Now I am in file {}, column {}, line {}.", file!(), column!(), line!());

    print_a_country(&mut country_vec);
}
```

이것은 다음을 출력합니다:

```text
Now I am in file src/main.rs, column 58, line 13.
The last country is Finland inside the module rust_book::something::third_mod
```

## `cfg!`

이제 우리는 `cfg!` 매크로를 봅니다. 이것은 "설정"을 의미하고 컴파일러에게 당신의 코드 설정에 따라 다른 것을 컴파일하라고 말합니다. 보통 OS가 다르거나 대상이 다를 때 사용됩니다. 하지만 `cfg!()`는 `true`나 `false`만 반환하므로, 당신은 그것을 체크하기 위해 `if`와 함께 사용합니다.

```rust
fn main() {
    let helpful_message = if cfg!(target_os = "windows") {
        "backslash를 사용해보세요! Windows를 사용하고 있는 것 같습니다"
    } else {
        "슬래시를 사용해보세요! Windows를 사용하지 않는 것 같습니다"
    };

    println!("{}", helpful_message);
}
```

이것은 설정에 따라 다르게 출력할 것입니다. 하지만 `cfg!()`는 `cfg`와 다릅니다. `cfg!` 매크로는 모든 것을 체크하고 `true`나 `false`를 주고, `cfg`는 컴파일할 것과 무시할 것을 컴파일러에게 말합니다.

여기 `cfg`의 예시가 있습니다. 이것은 당신이 아마 많은 Rust 코드에서 볼 것입니다:

```rust
#[cfg(target_os = "windows")]
fn print_windows_message() {
    println!("This only gets compiled on Windows.");
}

#[cfg(target_os = "macos")]
fn print_mac_message() {
    println!("This only gets compiled on MacOS.");
}

#[cfg(target_os = "linux")]
fn print_linux_message() {
    println!("This only gets compiled on Linux.");
}

fn main() {
    print_windows_message(); // Windows에서만 작동할 것입니다
    print_mac_message(); // MacOS에서만 작동할 것입니다
    print_linux_message(); // Linux에서만 작동할 것입니다
}
```

하지만 이것은 작동하지 않을 것인데, 함수가 다른 OS에서는 존재하지 않을 것이기 때문입니다. 그래서 당신은 이렇게 해야 합니다:

```rust
#[cfg(target_os = "windows")]
fn print_windows_message() {
    println!("This only gets compiled on Windows.");
}

#[cfg(target_os = "macos")]
fn print_mac_message() {
    println!("This only gets compiled on MacOS.");
}

#[cfg(target_os = "linux")]
fn print_linux_message() {
    println!("This only gets compiled on Linux.");
}

fn main() {
    #[cfg(target_os = "windows")]
    print_windows_message();

    #[cfg(target_os = "macos")]
    print_mac_message();

    #[cfg(target_os = "linux")]
    print_linux_message();
}
```

이제 각 OS에서 정확히 하나의 함수만 컴파일됩니다.

`cfg!()`를 사용하여 무언가를 체크할 수도 있습니다. 하지만 `cfg!`를 `if`와 함께 써야 합니다, `cfg`는 `if`와 함께 쓸 수 없기 때문입니다.

# Part 2 - 컴퓨터에서의 Rust

우리가 Playground만 사용해서 Rust의 거의 모든 것을 배울 수 있다는 것을 봤습니다. 하지만 여기까지 모든 것을 배웠다면, 아마 이제 컴퓨터에 Rust를 원할 것입니다. 파일을 사용하거나 하나 이상의 파일에서 코드를 사용하는 것과 같이 Playground로는 할 수 없는 일들이 항상 있습니다. 컴퓨터에 Rust가 필요한 다른 것들은 입력과 플래그입니다. 하지만 가장 중요한 것은 컴퓨터에 Rust가 있으면 크레이트를 사용할 수 있다는 것입니다. 우리는 이미 크레이트에 대해 배웠지만, Playground에서는 가장 인기 있는 것들만 사용할 수 있었습니다. 하지만 컴퓨터에 Rust가 있으면 프로그램에서 어떤 크레이트든 사용할 수 있습니다.

## cargo

`rustc`는 Rust 컴파일러를 의미하고, 실제 컴파일을 하는 것입니다. rust 파일은 `.rs`로 끝납니다. 하지만 대부분의 사람들은 컴파일하기 위해 `rustc main.rs`와 같은 것을 쓰지 않습니다. 그들은 `cargo`라고 불리는 것을 사용하는데, 이것은 Rust의 메인 패키지 매니저입니다.

이름에 대한 한 가지 주의사항: 크레이트들을 합치면 cargo가 되기 때문에 `cargo`라고 불립니다. 크레이트는 배나 트럭에서 보는 나무 상자이지만, 모든 Rust 프로젝트도 크레이트라고 불린다는 것을 기억하세요. 그러면 그것들을 합치면 전체 cargo를 얻습니다.

cargo를 사용해서 프로젝트를 실행할 때 이것을 볼 수 있습니다. `rand`로 간단한 것을 해봅시다: 8개의 글자 중에서 무작위로 선택할 것입니다.

```rust
use rand::seq::SliceRandom; // 슬라이스에 대해 .choose를 사용하기 위해 이것을 사용합니다

fn main() {

    let my_letters = vec!['a', 'b', 'c', 'd', 'e', 'f', 'g', 'h'];

    let mut rng = rand::thread_rng();
    for _ in 0..6 {
        print!("{} ", my_letters.choose(&mut rng).unwrap());
    }
}
```

이것은 `b c g h e a`와 같은 것을 출력할 것입니다. 하지만 Playground에서 이것을 하려고 하면, `rand`를 사용할 수 있는데, 그것이 탑 크레이트이기 때문입니다. 하지만 다른 크레이트를 사용하려고 하면 사용할 수 없습니다.

Playground는 `rand`와 같은 탑 크레이트들을 가지고 있지만, 모든 것을 가지고 있지는 않습니다. 하지만 `cargo`와 함께라면, Rust 커뮤니티의 모든 크레이트를 사용할 수 있습니다.

## 테스트

테스트는 당신의 코드가 작동하는지 확인하는 좋은 방법입니다. Rust에서는 `#[test]`와 `assert!` 및 `assert_eq!`와 같은 **assert 매크로들**을 사용하여 테스트를 작성할 수 있습니다. 여기 간단한 예시가 있습니다:

```rust
#[cfg(test)]
mod tests {
    use super::*;

    #[test]
    fn two_is_two() {
        assert_eq!(2, 2);
    }
}
```

하지만 지금 가장 쉬운 테스트는 `println!`을 사용하고 볼 수 있는 것입니다. 또한 Rust에서 디버그 출력을 위해 `dbg!` 매크로를 사용할 수 있습니다 - 이것은 변수 이름과 그 값을 출력합니다.

```rust
fn main() {
    let my_number = 8;
    dbg!(my_number);
}
```

이것은 `[src/main.rs:4] my_number = 8`을 출력할 것입니다.

더 복잡한 테스트와 벤치마크에 대해서는 나중에 배울 것이지만, 먼저 더 많은 Rust를 배워야 합니다.

## 외부 크레이트

크레이트는 다른 누군가가 쓴 Rust 코드입니다. [crates.io](https://crates.io)에서 그것들을 찾을 수 있습니다. 그것은 Rust 커뮤니티의 공식 레지스트리입니다. 크레이트를 사용하기 위해, `Cargo.toml` 파일에 그것을 추가합니다.

### rand

`rand` 크레이트는 난수를 생성하는 데 사용됩니다. Playground에서 자주 사용하는 것을 봤습니다:

```rust
use rand::Rng; // 트레이트

fn main() {
    let mut rng = rand::thread_rng();
    let random_number = rng.gen_range(1..=100);
    println!("임의의 숫자는: {}", random_number);
}
```

### serde

`serde`는 직렬화와 역직렬화를 위한 것입니다. 직렬화는 Rust 구조체를 JSON이나 다른 형식으로 변환하는 것을 의미하고, 역직렬화는 반대입니다.

```rust
use serde::{Serialize, Deserialize};

#[derive(Serialize, Deserialize)]
struct Person {
    name: String,
    age: u32,
}

fn main() {
    let person = Person {
        name: "김철수".to_string(),
        age: 30,
    };

    let json = serde_json::to_string(&person).unwrap();
    println!("JSON: {}", json);

    let person_again: Person = serde_json::from_str(&json).unwrap();
    println!("다시 만든 사람: {} ({}세)", person_again.name, person_again.age);
}
```

### regex

`regex` 크레이트는 정규 표현식을 사용하기 위한 것입니다:

```rust
use regex::Regex;

fn main() {
    let text = "제 이메일은 user@example.com입니다";
    let email_regex = Regex::new(r"[a-zA-Z0-9._%+-]+@[a-zA-Z0-9.-]+\.[a-zA-Z]{2,}").unwrap();

    if let Some(email) = email_regex.find(text) {
        println!("이메일을 찾았습니다: {}", email.as_str());
    }
}
```

## 모듈

이제 우리가 하나 이상의 파일로 작업하고 있으므로, 모듈에 대해 이야기해야 합니다. `mod`를 사용하여 모듈을 만들 수 있습니다.

### 파일 내 모듈

```rust
mod my_module {
    pub fn public_function() {
        println!("이것은 공개 함수입니다");
    }

    fn private_function() {
        println!("이것은 개인 함수입니다");
    }
}

fn main() {
    my_module::public_function(); // 작동합니다
    // my_module::private_function(); // 오류! 개인 함수입니다
}
```

### 별도 파일의 모듈

다른 파일에 모듈을 둘 수도 있습니다. 예를 들어, `helpers.rs`라는 파일이 있다면:

```rust
// helpers.rs 파일에서
pub fn useful_function() {
    println!("이것은 유용한 함수입니다");
}
```

그러면 `main.rs`에서:

```rust
// main.rs 파일에서
mod helpers;

fn main() {
    helpers::useful_function();
}
```

`pub` 키워드는 다른 모듈에서 함수를 사용할 수 있게 해줍니다. `pub` 없이는, 함수는 개인적이고 그 모듈 내에서만 사용할 수 있습니다.

## 파일 작업

이제 처음으로 파일과 작업해봅시다. `std::fs`는 파일과 작업하기 위한 메서드들이 있는 곳이고, `std::io::Write`로 파일에 쓸 수 있습니다. 그것으로 `.write_all()`을 사용하여 파일에 쓸 수 있습니다.

```rust
use std::fs;
use std::io::Write;

fn main() -> std::io::Result<()> {
    let mut file = fs::File::create("myfilename.txt")?; // 이 이름으로 파일을 만듭니다.
                                                        // 주의! 이 이름의 파일이 이미 있다면,
                                                        // 그 안의 모든 내용을 삭제할 것입니다.
    file.write_all(b"Let's put this in the file")?;     // " 앞의 b를 잊지 마세요. 파일은 바이트를 받기 때문입니다.
    Ok(())
}
```

그러면 새 파일 `myfilename.txt`를 클릭하면, `Let's put this in the file`이라고 말할 것입니다.

하지만 우리에게는 `?` 연산자가 있으므로 이것을 두 줄에 할 필요가 없습니다. 그것은 작동한다면 우리가 원하는 결과를 전달할 것인데, 이터레이터에서 많은 메서드를 사용할 때와 비슷합니다. 이때 `?`가 매우 편리해집니다.

```rust
use std::fs;
use std::io::Write;

fn main() -> std::io::Result<()> {
    fs::File::create("myfilename.txt")?.write_all(b"Let's put this in the file")?;
    Ok(())
}
```

그래서 이것은 "파일을 만들려고 시도하고 작동했는지 확인해주세요. 만약 작동했다면, `.write_all()`을 사용하고 그것도 작동했는지 확인해주세요"라고 말하는 것입니다.

그리고 실제로, 이 두 가지를 함께 하는 함수도 있습니다. 그것은 `std::fs::write`라고 불립니다. 그 안에 원하는 파일 이름과 안에 넣고 싶은 내용을 제공합니다. 다시, 주의하세요! 파일이 이미 존재한다면 그 안의 모든 내용을 삭제할 것입니다. 또한, 이것 때문에 앞에 `b` 없이 `&str`를 쓸 수 있게 해줍니다:

```rust
pub fn write<P: AsRef<Path>, C: AsRef<[u8]>>(path: P, contents: C) -> Result<()>
```

`AsRef<[u8]>`가 둘 중 하나를 줄 수 있는 이유입니다.

매우 간단합니다:

```rust
use std::fs;

fn main() -> std::io::Result<()> {
    fs::write("calvin_with_dad.txt",
"Calvin: Dad, how come old photographs are always black and white? Didn't they have color film back then?
Dad: Sure they did. In fact, those photographs *are* in color. It's just the *world* was black and white then.
Calvin: Really?
Dad: Yep. The world didn't turn color until sometimes in the 1930s...")?;

    Ok(())
}
```

그래서 이것이 우리가 사용할 파일입니다. 이것은 Calvin이라는 만화책 캐릭터와 그의 아버지와의 대화인데, 아버지는 그의 질문에 대해 진지하지 않습니다. 이것으로 매번 사용할 파일을 만들 수 있습니다.

파일을 여는 것은 만드는 것만큼 쉽습니다. `create()` 대신 `open()`만 사용하면 됩니다. 그 후에 (파일을 찾으면), `read_to_string()`과 같은 것을 할 수 있습니다. 그것을 하기 위해 가변 `String`을 만들고 파일을 거기에 읽어들일 수 있습니다. 다음과 같이 보입니다:

```rust
use std::fs;
use std::fs::File;
use std::io::Read; // 이것은 .read_to_string() 함수를 사용하기 위한 것입니다

fn main() -> std::io::Result<()> {
     fs::write("calvin_with_dad.txt",
"Calvin: Dad, how come old photographs are always black and white? Didn't they have color film back then?
Dad: Sure they did. In fact, those photographs *are* in color. It's just the *world* was black and white then.
Calvin: Really?
Dad: Yep. The world didn't turn color until sometimes in the 1930s...")?;


    let mut calvin_file = File::open("calvin_with_dad.txt")?; // 방금 만든 파일을 엽니다
    let mut calvin_string = String::new(); // 이 String이 그것을 담을 것입니다
    calvin_file.read_to_string(&mut calvin_string)?; // 파일을 그것에 읽어들입니다

    calvin_string.split_whitespace().for_each(|word| print!("{} ", word.to_uppercase())); // 이제 String으로 작업을 합니다

    Ok(())
}
```

이것은 다음을 출력합니다:

```text
CALVIN: DAD, HOW COME OLD PHOTOGRAPHS ARE ALWAYS BLACK AND WHITE? DIDN'T THEY HAVE COLOR FILM BACK THEN? DAD: SURE THEY DID. IN FACT, THOSE PHOTOGRAPHS *ARE* IN COLOR. IT'S JUST THE *WORLD* WAS BLACK AND WHITE THEN. CALVIN: REALLY? DAD: YEP. THE WORLD DIDN'T TURN COLOR UNTIL SOMETIMES IN THE 1930S...
```

좋네요! 그리고 파일을 읽는 더 간단한 방법도 있습니다, `std::fs::read_to_string`입니다. 이것은 파일을 만들고 그것에 내용을 읽어들이는 것을 한 번에 합니다. 그런 다음 `String`을 반환합니다. 더 간단해 보입니다:

```rust
use std::fs;

fn main() -> std::io::Result<()> {
     fs::write("calvin_with_dad.txt",
"Calvin: Dad, how come old photographs are always black and white? Didn't they have color film back then?
Dad: Sure they did. In fact, those photographs *are* in color. It's just the *world* was black and white then.
Calvin: Really?
Dad: Yep. The world didn't turn color until sometimes in the 1930s...")?;

    let calvin_string = fs::read_to_string("calvin_with_dad.txt")?; // 파일을 읽고 String에 넣습니다

    calvin_string.split_whitespace().for_each(|word| print!("{} ", word.to_uppercase()));

    Ok(())
}
```

파일을 여는 가장 간단한 방법은 `File::open()`이고, 파일을 만드는 가장 간단한 방법은 `File::create()`입니다. 하지만 때로는 더 많은 옵션이 필요합니다. 그것이 `OpenOptions`가 있는 이유입니다. 실제로 `File::open()`을 봐도 이것을 사용합니다:

```rust
pub fn open<P: AsRef<Path>>(path: P) -> io::Result<File> {
    OpenOptions::new().read(true).open(path.as_ref())
}
```

그리고 `File::create()`에 대해서도:

```rust
pub fn create<P: AsRef<Path>>(path: P) -> io::Result<File> {
    OpenOptions::new().write(true).create(true).truncate(true).open(path.as_ref())
}
```

두 번째 것에 대해 생각해보면, `create()`는:

- write가 `true`로 설정되어 있으므로 쓸 수 있습니다,
- create가 `true`로 설정되어 있으므로 파일을 만들 수 있습니다...
- 하지만 truncate도 `true`로 설정되어 있으므로 파일이 이미 있다면 그 내용을 자를 것입니다 (삭제합니다).

그래서 파일을 만들고 싶지만 이미 존재한다면 실수하고 싶지 않다면, `OpenOptions`를 사용할 수 있습니다. 예시에서 우리는 새 파일을 만들려고 하지만 이미 파일이 있습니다. `create_new()`를 사용하면, 파일이 이미 존재한다면 실패할 것입니다.

```rust
use std::fs;
use std::fs::OpenOptions;

fn main() -> std::io::Result<()> {
     fs::write("calvin_with_dad.txt",
"Calvin: Dad, how come old photographs are always black and white? Didn't they have color film back then?
Dad: Sure they did. In fact, those photographs *are* in color. It's just the *world* was black and white then.
Calvin: Really?
Dad: Yep. The world didn't turn color until sometimes in the 1930s...")?;

    let calvin_file = OpenOptions::new().write(true).create_new(true).open("calvin_with_dad.txt")?;

    Ok(())
}
```

먼저 우리는 `new`로 `OpenOptions`를 만들었습니다 (항상 `new`로 시작합니다). 그런 다음 그것에게 `write`할 수 있는 능력을 주었습니다. 그 후에 `create_new()`를 `true`로 설정하고, 우리가 만든 파일을 열려고 시도했습니다. 작동하지 않을 것이고, 그것이 우리가 원하는 것입니다:

```text
Error: Os { code: 80, kind: AlreadyExists, message: "The file exists." }
```

이제 우리가 원하는 것을 얻었습니다! 파일이 이미 존재한다면 실수하지 않습니다. 파일이 없다면, `create_new(true)`가 그것을 만들 것입니다.

아니면 어쩌면 당신은 파일을 열고 싶지만 삭제하고 싶지 않을 수도 있습니다. 어쩌면 당신은 파일에 추가만 하고 싶을 수도 있습니다 (끝에 쓰고 싶습니다). 그러면 `.append()`를 사용할 수 있습니다:

```rust
use std::fs;
use std::fs::OpenOptions;
use std::io::Write;

fn main() -> std::io::Result<()> {
    fs::write("calvin_with_dad.txt",
"Calvin: Dad, how come old photographs are always black and white? Didn't they have color film back then?
Dad: Sure they did. In fact, those photographs *are* in color. It's just the *world* was black and white then.
Calvin: Really?
Dad: Yep. The world didn't turn color until sometimes in the 1930s...")?;

    let mut calvin_file = OpenOptions::new()
        .append(true) // 이제 삭제하지 않고 쓸 수 있습니다
        .read(true)
        .open("calvin_with_dad.txt")?;
    calvin_file.write_all(b"And it was a pretty grainy color for a while too.\n")?;
    write!(&mut calvin_file, "That's really weird.\n")?;
    write!(&mut calvin_file, "Well, truth is stranger than fiction.")?;

    println!("{}", fs::read_to_string("calvin_with_dad.txt")?);

    Ok(())
}
```

이것은 다음을 출력합니다:

```text
Calvin: Dad, how come old photographs are always black and white? Didn't they have color film back then?
Dad: Sure they did. In fact, those photographs *are* in color. It's just the *world* was black and white then.
Calvin: Really?
Dad: Yep. The world didn't turn color until sometimes in the 1930s...And it was a pretty grainy color for a while too.
That's really weird.
Well, truth is stranger than fiction.
```

이제 우리는 원래 텍스트와 우리가 추가한 새 텍스트를 봅니다.

## Result 타입

Result는 Option과 비슷하지만, 차이점이 있습니다:

- Option은 `Some` 또는 `None`에 관한 것입니다 (값 또는 값 없음),
- Result는 `Ok` 또는 `Err`에 관한 것입니다 (정상 결과, 또는 에러 결과).

그래서 `Option`은 "어쩌면 뭔가가 있을 것이고, 어쩌면 없을 것이다"라고 생각할 때입니다. 하지만 `Result`는 "어쩌면 실패할 것이다"라고 생각할 때입니다.

비교하기 위해, 여기 Option과 Result의 시그니처가 있습니다.

```rust
enum Option<T> {
    None,
    Some(T),
}

enum Result<T, E> {
    Ok(T),
    Err(E),
}

fn main() {}
```

그래서 Result는 `Ok` 안에 값이 있고, `Err` 안에도 값이 있습니다. 왜냐하면 에러는 보통 에러를 설명하는 정보를 포함하기 때문입니다.

`Result<T, E>`는 `Ok`에 대해 무엇을 반환할지, `Err`에 대해 무엇을 반환할지 생각해야 한다는 것을 의미합니다. 실제로, 무엇이든 결정할 수 있습니다. 이것도 괜찮습니다:

```rust
fn check_error() -> Result<(), ()> {
    Ok(())
}

fn main() {
    check_error();
}
```

`check_error`는 "`Ok`를 얻으면 `()`를 반환하고, `Err`를 얻으면 `()`를 반환한다"고 말합니다. 그런 다음 우리는 `()`와 함께 `Ok`를 반환합니다.

컴파일러는 우리에게 흥미로운 경고를 줍니다:

```text
warning: unused `std::result::Result` that must be used
 --> src\main.rs:6:5
  |
6 |     check_error();
  |     ^^^^^^^^^^^^^^
  |
  = note: `#[warn(unused_must_use)]` on by default
  = note: this `Result` may be an `Err` variant, which should be handled
```

이것은 맞습니다: 우리는 `Result`만 반환했지만 그것은 `Err`일 수도 있었습니다. 그래서 여전히 실제로 뭔가를 하지는 않지만, 에러를 조금 처리해봅시다.

```rust
fn give_result(input: i32) -> Result<(), ()> {
    if input % 2 == 0 {
        return Ok(())
    } else {
        return Err(())
    }
}

fn main() {
    if give_result(5).is_ok() {
        println!("It's okay, guys")
    } else {
        println!("It's an error, guys")
    }
}
```

이것은 `It's an error, guys`를 출력합니다. 그래서 우리는 첫 번째 에러를 처리했습니다.

기억하세요, 쉽게 확인하는 네 가지 메서드는 `.is_some()`, `is_none()`, `is_ok()`, 그리고 `is_err()`입니다.

때로는 Result를 가진 함수가 `Err` 값에 대해 `String`을 사용할 것입니다. 이것은 사용하기에 최선의 방법은 아니지만, 지금까지 우리가 한 것보다는 조금 낫습니다.

```rust
fn check_if_five(number: i32) -> Result<i32, String> {
    match number {
        5 => Ok(number),
        _ => Err("Sorry, the number wasn't five.".to_string()), // 이것이 우리의 에러 메시지입니다
    }
}

fn main() {
    let mut result_vec = Vec::new(); // 결과들을 위한 새 vec을 만듭니다

    for number in 2..7 {
        result_vec.push(check_if_five(number)); // 각 결과를 vec에 push합니다
    }

    println!("{:?}", result_vec);
}
```

우리의 vec은 다음을 출력합니다:

```text
[Err("Sorry, the number wasn\'t five."), Err("Sorry, the number wasn\'t five."), Err("Sorry, the number wasn\'t five."), Ok(5),
Err("Sorry, the number wasn\'t five.")]
```

Option과 마찬가지로, `Err`에서 `.unwrap()`은 패닉을 일으킬 것입니다.

```rust
    // ⚠️
fn main() {
    let error_value: Result<i32, &str> = Err("There was an error"); // 이미 Err인 Result를 만듭니다
    println!("{}", error_value.unwrap()); // 그것을 unwrap합니다
}
```

프로그램이 패닉을 일으키고, 다음을 출력합니다:

```text
thread 'main' panicked at 'called `Result::unwrap()` on an `Err` value: "There was an error"', src\main.rs:30:20
```

이 정보는 당신의 코드를 고치는 데 도움이 됩니다. `src\main.rs:30:20`은 "src 디렉토리의 main.rs 안에서, 30번째 줄과 20번째 열에서"를 의미합니다. 그래서 당신은 거기로 가서 코드를 보고 문제를 고칠 수 있습니다.

자신만의 에러 타입도 만들 수 있습니다. 표준 라이브러리와 다른 사람들의 코드에서 Result 함수들은 보통 이것을 합니다. 예를 들어, 표준 라이브러리의 이 함수:

```rust
pub fn from_utf8(vec: Vec<u8>) -> Result<String, FromUtf8Error>
```

이 함수는 바이트들의 벡터(Vec `<u8>`)를 가져와서 String으로 만들려고 합니다. 그래서 Result 안에서:

- Ok는 성공하면 String을 가집니다
- Err는 실패하면 FromUtf8Error를 가집니다. 당신은 이 에러를 사용하여 뭐가 잘못되었는지 알아낼 수 있습니다.

이제 좋은 예시를 만들어봅시다. 실제로는 절대로 하지 않을 일을 시도해봅시다: `String`을 `i32`로 파싱하기 위해 `.parse()`를 사용하되 모든 글자를 확인하는 것입니다.

먼저 에러 타입을 만들어야 합니다. `enum`으로 에러를 만들 수 있습니다. 좋은 에러 타입은 사용자에게 무엇이 잘못되었는지 알려줍니다. 우리는 `ParseError`라고 부를 것이고 두 가지 종류의 에러를 가질 것입니다:

```rust
use std::num::ParseIntError;

#[derive(Debug)]
enum ParseError {
    Empty,
    TooBig,
}
```

그런 다음 우리는 함수를 만들어야 합니다. 우리는 `&str`를 가져와서 `Result<i32, ParseError>`를 반환할 것입니다:

```rust
use std::num::ParseIntError;

#[derive(Debug)]
enum ParseError {
    Empty,
    TooBig,
}

fn parse_str(input: &str) -> Result<i32, ParseError> {
    let parsed_number = input.parse::<i32>(); // 이것은 Result<i32, ParseIntError>를 줍니다
    match parsed_number {
        Ok(number) => {
            if number > 1000 {   // 우리는 1000보다 큰 숫자를 좋아하지 않습니다
                Err(ParseError::TooBig)
            } else {
                Ok(number)
            }
        },
        Err(_) => {
            if input.is_empty() {
                Err(ParseError::Empty)
            } else {
                Err(ParseError::TooBig) // 만약 .parse()가 실패했다면, 아마 너무 클 것입니다
            }
        }
    }
}

fn main() {}
```

이제 테스트해봅시다:

```rust
fn main() {
    // 다음 라인을 하나씩 테스트해보세요
    println!("{:?}", parse_str("7")); // Ok(7)
    println!("{:?}", parse_str("9001")); // Err(TooBig)
    println!("{:?}", parse_str("")); // Err(Empty)
    println!("{:?}", parse_str("completely wrong")); // Err(TooBig)
}
```

좋네요! 그래서 당신은 당신만의 에러 타입을 만들 수 있습니다.

## ? 연산자

하지만 에러를 다루는 더 짧은 방법이 있습니다: `?` 연산자입니다. 함수가 `Result`를 반환할 때, 당신은 `?`를 추가할 수 있습니다. 이것은 컴파일러에게 "만약 에러라면, 에러를 반환하고, 만약 Ok라면, 안의 값을 주세요"라고 말합니다.

이 함수를 봅시다:

```rust
fn parse_str(input: &str) -> Result<i32, std::num::ParseIntError> {
    let parsed_number = input.parse::<i32>()?; // 여기서 ?를 사용했습니다
    Ok(parsed_number)
}
```

이 함수는:

- 만약 input.parse::`<i32>`()가 Ok라면, parsed_number에 i32를 넣습니다. 그런 다음 Ok(parsed_number)를 반환합니다.
- 만약 input.parse::`<i32>`()가 Err라면, ParseIntError를 반환합니다 (그리고 함수를 종료합니다).

`?` 연산자는 매우 편합니다. 하지만 함수가 `Result`를 반환해야만 `Result`에서 그것을 사용할 수 있습니다 (그리고 같은 에러 타입이어야 합니다). 예를 들어, 이것은 작동하지 않습니다:

```rust
    // ⚠️
fn main() {
    let parsed = "7".parse::<i32>()?;
    println!("{}", parsed);
}
```

왜냐하면 `main()`은 `Result`를 반환하지 않기 때문입니다. `main()`은 아무것도 반환하지 않거나, `()`를 반환하거나, `Result`를 반환할 수 있습니다.

```rust
fn main() -> Result<(), std::num::ParseIntError> {
    let parsed = "7".parse::<i32>()?;
    println!("{}", parsed);
    Ok(())
}
```

이제 작동합니다. 하지만 실제로는 `main()`에서 이런 것을 많이 하지 않습니다. `?`는 보통 다른 함수들에서 Result를 반환할 때 사용됩니다.

## 클로저 (Closures)

클로저는 이름이 필요하지 않은 빠른 함수와 같습니다. 때로는 람다라고도 불립니다. 클로저는 `()` 대신 `||`를 사용하기 때문에 찾기 쉽습니다. 그것들은 Rust에서 매우 흔하고, 한번 사용하는 법을 배우면 그것들 없이 어떻게 살았는지 궁금할 것입니다.

클로저를 변수에 바인딩할 수 있고, 그러면 사용할 때 함수와 정확히 같아 보입니다:

```rust
fn main() {
    let my_closure = || println!("This is a closure");
    my_closure();
}
```

그래서 이 클로저는 아무것도 받지 않습니다: `||` 그리고 메시지를 출력합니다: `This is a closure`.

`||` 사이에 함수의 `()` 안에서처럼 입력 변수와 타입을 추가할 수 있습니다:

```rust
fn main() {
    let my_closure = |x: i32| println!("{}", x);

    my_closure(5);
    my_closure(5+5);
}
```

이것은 다음을 출력합니다:

```text
5
10
```

클로저가 더 복잡할 때는, `{}`를 사용할 수 있습니다:

```rust
fn main() {
    let my_closure = || {
        let number = 7;
        let other_number = 10;
        println!("The two numbers are {} and {}.", number, other_number);
          // 이 클로저는 아무것도 반환하지 않습니다
    };

    my_closure();
}
```

하지만 클로저는 **외부 변수를 캡처**할 수 있기 때문에 특별합니다. 즉, 클로저가 만들어진 범위에서 변수를 사용할 수 있다는 의미입니다.

```rust
fn main() {
    let number_outside = 10;

    let my_closure = || println!("{}", number_outside);

    my_closure();
}
```

그래서 `my_closure`가 `number_outside`를 "캡처"했고, 이제 `number_outside`를 사용할 수 있습니다. 그리고 `number_outside`를 안에서 변경하려고 하면 어떻게 될까요?

```rust
fn main() {
    let mut number_outside = 10;

    let mut my_closure = || {
        number_outside += 1; // 외부 변수를 변경합니다
        println!("{}", number_outside);
    };

    my_closure();
}
```

이것은 `11`을 출력합니다. 왜냐하면 `number_outside`가 변경되었기 때문입니다.

클로저의 좋은 점은 `|`와 `|` 사이에 타입을 쓸 필요가 없다는 것입니다. 왜냐하면 컴파일러가 추측할 수 있기 때문입니다:

```rust
fn main() {
    let number = 10;
    let closure_1 = |x| x + number; // 숫자들, 그래서 x는 정수여야 합니다
    let closure_2 = |x| println!("{}", x); // 무엇이든 출력할 수 있습니다

    closure_1(5);
    closure_2("Can print a &str");
    closure_2(closure_1(1));
}
```

이것은 다음을 출력합니다:

```text
Can print a &str
11
```

## 함수에서의 클로저

클로저는 훌륭합니다. 그래서 우리 자신의 함수에 그것들을 어떻게 넣을까요?

클로저를 받는 자신만의 함수를 만들 수 있지만, 함수 안에서는 덜 자유롭고 타입을 결정해야 합니다. 함수 밖에서는 클로저가 `Fn`, `FnMut`, `FnOnce` 중에서 스스로 결정할 수 있지만, 함수 안에서는 하나를 선택해야 합니다. 이해하는 가장 좋은 방법은 몇 가지 함수 시그니처를 보는 것입니다. 여기 `.all()`에 대한 것이 있습니다. 우리는 그것이 이터레이터를 확인해서 모든 것이 `true`인지 보는 것을 기억합니다 (당신이 무엇을 `true`나 `false`로 결정하는지에 따라). 시그니처의 일부는 다음과 같이 말합니다:

```rust
    fn all<F>(&mut self, f: F) -> bool    // 🚧
    where
        F: FnMut(Self::Item) -> bool,
```

`fn all<F>`: 이것은 제네릭 타입 `F`가 있다는 것을 알려줍니다. 클로저는 매번 다른 타입이기 때문에 항상 제네릭입니다.

`(&mut self, f: F)`: `&mut self`는 그것이 메서드라는 것을 알려줍니다. `f: F`는 보통 클로저에 대해 보는 것입니다: 이것은 변수 이름과 타입입니다. 물론, `f`와 `F`에 대해 특별한 것은 없고 다른 이름일 수도 있습니다. 원한다면 `my_closure: Closure`라고 쓸 수도 있습니다 - 상관없습니다. 하지만 시그니처에서는 거의 항상 `f: F`를 봅니다.

다음은 클로저에 대한 부분입니다: `F: FnMut(Self::Item) -> bool`. 여기서 그것은 클로저가 `FnMut`라고 결정하므로, 값들을 변경할 수 있습니다. 그것은 `Self::Item`의 값들을 변경하는데, 이것은 그것이 받는 이터레이터입니다. 그리고 `true` 또는 `false`를 반환해야 합니다.

여기 클로저와 함께하는 훨씬 더 간단한 시그니처가 있습니다:

```rust
fn do_something<F>(f: F)    // 🚧
where
    F: FnOnce(),
{
    f();
}
```

이것은 단지 클로저를 받고, 값을 가져가고 (`FnOnce` = 값을 가져갑니다), 아무것도 반환하지 않는다고 말합니다. 그래서 이제 우리는 아무것도 받지 않는 이 클로저를 호출하고 우리가 좋아하는 무엇이든 할 수 있습니다. 우리는 `Vec`를 만들고 그것을 이터레이트해서 지금 우리가 할 수 있는 것을 보여줄 것입니다.

```rust
fn do_something<F>(f: F)
where
    F: FnOnce(),
{
    f();
}

fn main() {
    let some_vec = vec![9, 8, 10];
    do_something(|| {
        some_vec
            .iter()
            .for_each(|x| print!("{} ", x));
    })
}
```

이것은 `9 8 10 `을 출력합니다.

만약 클로저가 변수들을 사용한다면, 당신은 `Fn`이나 `FnMut`를 사용할 수 있습니다. `Fn`은 참조를 받고, `FnMut`는 가변 참조를 받습니다. 이 예시에서는 `FnMut`를 사용할 것입니다.

```rust
fn do_something<F>(mut f: F) // f는 이제 가변입니다
where
    F: FnMut(),
{
    f(); // f()를 몇 번 호출할 수 있습니다
    f();
}

fn main() {
    let mut x = 10;
    do_something(|| {
        x += 1; // x를 변경하므로 이제 FnMut입니다
        println!("{}", x);
    })
}
```

이것은 다음을 출력합니다:

```text
11
12
```

그리고 만약 우리가 값을 반환하고 싶다면, 우리는 이것을 할 수 있습니다:

```rust
fn do_something<F>(f: F) -> i32
where
    F: Fn() -> i32,
{
    f()
}

fn main() {
    let x = 10;
    let number = do_something(|| x + 1);
    println!("{}", number);
}
```

이것은 `11`을 출력합니다.
