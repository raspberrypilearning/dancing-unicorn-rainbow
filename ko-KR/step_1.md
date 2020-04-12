--- no-print --- 
이 프로젝트에 사용된 버전은 스크래치 3 입니다. [Scratch 2 버전은 여기에서 찾을 수 있습니다.](https://projects.raspberrypi.org/ko-KR/projects/dancing-unicorn-rainbow-scratch2) 
--- / no-print ---

## 들어가며

Raspberry Pi로 구동되는 LED 무지개를 만들고 유니콘이 춤을 추게 해보세요.

### 만들 작품

스크래치를 사용하여 LED 무지개를 유니콘 스프라이트에 연결 한 다음, 유니콘이 무지개의 리듬에 맞춰 춤을 추게 할 것입니다. 다음은 춤추는 유니콘과 무지개의 모습을 보여주는 비디오입니다:

<video width="560" height="315" controls> <source src="resources/Screencast.mp4" type="video/mp4"> 브라우저가 비디오 태그를 지원하지 않습니다. FireFox 또는 Chrome을 사용해보십시오. </video> 

유니콘을 무지개에 맞춰 춤을 추도록 한 이후에는, 무지개를 사용하여 유니콘이 재롱을 부리거나 게임을 하게 하는 방법을 배울 수 있습니다.

--- collapse ---
---
title: 준비물
---

### 하드웨어

+ Raspberry Pi
+ 브레드보드
+ 3개 이상의 색상이 다양한 LED
+ 저항 (100 ohm 이상), **LED 한 개당 하나씩**
+ 버튼 1개
+ M-F 점퍼 케이블, **LED 한 개당 하나씩**
+ 추가 M-F 점퍼 케이블 2개
+ F-F 점퍼 케이블 1개

선택적인 도전 과제를 하고 싶다면:

+ 버저 1개
+ 추가 M-F 점퍼 케이블 2개

### 소프트웨어

다음 소프트웨어 패키지가 포함 된 최신 버전의 Raspbian이 필요합니다:

+ 스크래치 3

```bash
sudo apt-get update
sudo apt-get install scratch3
```

**참고:** 스크래치 3는 **Raspberry Pi 4 에서만** 작동합니다. --- /collapse ---

--- collapse ---
---
title: 학습 효과
---

이 프로젝트는 [라즈베리 파이 디지털 메이킹 커리큘럼](http://rpf.io/curriculum){:target="_blank"}: 중 아래의 과정에 있는 요소들을 다룹니다.

+ [프로젝트를 진행하거나 문제를 해결하기 위해 입력과 출력을 결합하기](https://curriculum.raspberrypi.org/physical-computing/builder/){:target="_blank"}

+ [문제를 해결하기 위해 간단한 프로그램 구조 적용하기](https://www.raspberrypi.org/curriculum/programming/builder){:target="_blank"}

--- collapse ---
---
title: 교육자를 위한 추가 정보
---

이 프로젝트를 인쇄한다면 [프린트용 버전](https://projects.raspberrypi.org/ko-KR/projects/dancing-unicorn-rainbow/print){:target="_blank"}을 사용해 주십시오.

이 프로젝트의 전체 솔루션은 [rpf.io/p/ko-KR/dancing-unicorn-rainbow-get](https://rpf.io/p/ko-KR/dancing-unicorn-rainbow-get)에서 찾을 수 있습니다. --- /collapse ---