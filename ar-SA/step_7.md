## أضيء قوس قزحك

للتأكد من أن قوس القزح يعمل ، سوف تختبره أولاً عن طريق إضاءة قوس القزح بأكمله في وقت واحد. ستقوم بعد ذلك بإنشاء التعليمات البرمجية لجعل قوس قزح يضيء جميع ألوانه الواحد تلو الآخر، ثم في نمط من اختيارك.

--- task --- أضف المزيد من التعليمات البرمجية للتحكم في مصابيح LED الأخرى. تأكد من تضمين منافذ GPIO الصحيحة. --- /task ---

قوس قزحك يجب أن يضيء مثل هذا:

![قوس قزح مضاء](images/rainbowlit.png)

--- hints ---
 --- hint --- أضف المزيد من الكتل البرمجية `تشغيل LED (0 v) [on v]`{:class="block3extensions"} في هذا الجزء من الكود البرمجي:

```blocks3
when flag clicked
turn LED (17 v) [on v] ::extension
```

--- /hint --- --- hint --- استمر في إضافة الكتل البرمجية في أسفل التعليمات البرمجية الخاصة بك حتى يتم تعيين جميع المصابيح LED الخاصة بك إلى `on`{:class="block3extensions"}.

```blocks3
when flag clicked
turn LED (17 v) [on v] ::extension
turn LED (18 v) [on v] ::extension
turn LED (22 v) [on v] ::extension
```

--- /hint --- --- hint ---

إذا لم تكن مصابيح LED مضاءة:

1) تحقق من منفذ GPIO الذي تتصل به المصابيح، وتأكد من ضبطها إلى `on`{:class="block3extensions"} 
2) اختبر ما إذا كانت مصابيح LEDs تعمل - يمكنك توصيل سلك الذي يربط مصباح LED إلى **GPIO 3V3** لاختباره 
3) تأكد من اكتمال الدائرة على لوحة التحكم

--- /hint ------ /hints ---

--- task --- الآن، أضف المزيد من التعليمات البرمجية لجعل قوس قزح يومض في نمط قوس قزح مثل هذا:

<video width="560" height="315" controls> <source src="resources / Scratch-GPIO-Pathways-5.mp4" type="video/mp4"> Your browser does not support the video tag, so try FireFox or Chrome. </video> 

للقيام بذلك، سوف تحتاج إلى تشغيل ضوء واحد لبضع ثوان ثم إيقاف التشغيل في نفس الوقت الذي يشتغل فيه مصباح LED التالي. --- /task ---

--- hints ---
 --- hint ---

تأكد من أن كتلة `الأحداث `{:class="blockevents"} تطابق ما تفعله لاختبار الكود. في المثال هنا علينا النقر على العلم الأخض لجعل قوس قزحنا يعمل:

```blocks3
when flag clicked
```

--- /hint --- --- hint ---

إذا كنت عالقا، تأكد من أنك تستخدم هذه الكتل:

```blocks3
turn LED (0 v) [off v] ::extension
wait () secs
```

--- /hint --- --- hint ---

حاول استخدام هذا النهج:

```blocks3
when flag clicked
turn LED (17 v) [on v] ::extension
wait (0.5) secs
turn LED (17 v) [off v] ::extension
turn LED (18 v) [on v] ::extension
wait (0.5) secs
turn LED (18 v) [off v] ::extension
turn LED (22 v) [on v] ::extension
```

سوف تحتاج إلى إضافة كتل لكل المصابيح الخاصة بك والتأكد من أنك تستخدم أرقام منافذ GPIO الصحيحة في الكود الخاص بك.

--- /hint ------ /hints ---

--- task --- جعل الأضواء تومض مرارا وتكرارا خلال قوس القزح في حلقة تكرارية.

للدوران عبر نمط قوس قزح للأبد، استخدم:

```blocks3
كرر باستمرار
```

--- /task ---

--- challenge ---

+ اجعل قوس القزح يضيء في نمط من اختيارك.

--- collapse ---
---
title: تحديات قوس قزح
---

جرب الأفكار التالية:

1) اجعل مصابيح LED تومض بسرعة كبيرة وبطيئة جدا
2) اجعل قوس قزح يومض بأكمله
3) اجعل أزواج مصابيح LED تضيء في أنماط متبادلة
4) اجعل قوس قزح يومض برمز مورس (Morse code)
5) اجعل قوس قزح يفعل أشياء مختلفة استجابة لأحداث مختلفة

--- /collapse --- --- /challenge ---