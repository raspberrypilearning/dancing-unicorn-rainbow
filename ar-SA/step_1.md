\--- no-print \--- هذا هو إصدار Scratch 3 من المشروع. يمكنك العثور على النسخة [Scratch 2 هنا.](https://projects.raspberrypi.org/en/projects/dancing-unicorn-rainbow-scratch2) \--- /no-print \---

## المقدمة

إنشاء ضوء قوس قزح (LED) ووحيد القرن يرقص له، وكل ذلك مدعوم من قبل Raspberry Pi.

### ما الذي ستصنعه

سوف تستخدم Scratch لربط قوس قزح من مصابيح LED بكائن وحيد القرن، ومن ثم تجعل وحيد القرن يرقص إلى إيقاع قوس قزح. إليك فيديو يظهر ما قد يبدو عليه وحيد قرن راقص مع قوس القزح:<video width="560" height="315" controls> <source src="resources/Screencast.mp4" type="video/mp4"> Your browser does not support the video tag, try FireFox or Chrome </video> 

بمجرد أن تقوم بتدريب وحيد القرن الخاص بك على الرقص على قوس القزح، بإمكانك أن تتعلم كيفية استخدام قوس قزح لجعل وحيد القرن يفعل الحيل أو لعب اللعبة.

## \--- collapse \---

## title: ما الذي ستحتاجه

### الأجهزة

+ Raspberry Pi
+ لوحة توصيل
+ 3 أو أكثر من مصابيح LED الملونة
+ مقاومات (100 اوم على الاقل)، **1 لكل مصباح LED**
+ 1× زر
+ أسلاك التوصيل من ذكر إلى أنثى، ** 1 لكل LED **
+ 2× أسلاك توصيل إضافية من ذكر إلى انثى
+ 1× سلك موصل من ذكر إلى ذكر

فيما يتعلق بالتحدي النهائي الاختياري:

+ 1× buzzer جرس
+ 2× أسلاك توصيل إضافية من ذكر إلى انثى

### البرامج

ستحتاج إلى أحدث إصدار من نظام التشغيل Raspbian، والذي يتضمن بالفعل حزمة البرامج التالية:

+ سكراتش Scratch3.0

```bash
sudo apt-get update
sudo apt-get install scratch3
```

**ملاحظة:** سيعمل برنامج Scratch 3** فقط ** على Raspberry Pi 4. \--- /collapse \---

## \--- collapse \---

## title: ما الذي ستتعلمه

يتناول هذا المشروع عناصر من [معايير المناهج الرقمية الخاصة بـ Raspberry Pi](http://rpf.io/curriculum) {:target="_blank"}:

+ [دمج المدخلات و/أو المخرجات لإنشاء مشاريع أو حل مشكلة](https://curriculum.raspberrypi.org/physical-computing/builder/){:target="_blank"}

+ [استخدام تراكيب البرمجة الأساسية لإنشاء برامج بسيطة](https://www.raspberrypi.org/curriculum/programming/builder){:target="_blank"} \--- /collapse \---

## \--- collapse \---

## title: معلومات إضافية للمعلمين

إذا كنت بحاجة إلى طباعة هذا المشروع، فالرجاء استخدام [نسخة متوافقة مع الطابعة](https://projects.raspberrypi.org/en/projects/dancing-unicorn-rainbow/print){:target="_blank"}.

يمكنك العثور على الحل الكامل لهذا المشروع في [rpf.io/p/en/dancing-unicorn-rainbow-get](https://rpf.io/p/en/dancing-unicorn-rainbow-get) \--- /collapse \---