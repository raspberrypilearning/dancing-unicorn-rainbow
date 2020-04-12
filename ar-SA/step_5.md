## التحكم في دائرة قوس قزح

عندما يتم إعداد قوس قزح بأكمله، يمكنك التحكم في كيفية إضاءته. استخدم Scratch للقيام بما يلي من أجل التمرس قليلا للتحكم في واحد من مصابيح LED:

--- task --- عندما تضغط على مفتاح <kbd>P</kbd> قم بتشغيل LED لمدة ثانيتين ثم قم بإيقاف تشغيله. --- /task ---

--- hints ---
 --- hint --- انظر في قسم الكتل `التحكم`{:class="block3control"}.
--- /hint ---
 --- hint --- استخدم

```blocks3
  انتظر (2) ثانية
```

--- /hint --- --- hint ---

```blocks3
when [p v] key pressed
turn LED (17 v) [on v] ::extension
wait (2) secs
turn LED (17 v) [off v] ::extension
```

--- /hint ------ /hints ---

--- task --- عندما يبدأ برنامج Scratch الخاص بك، اجعل المصباح LED يشتغل مدة 2 ثانية ثم يتوقف لمدة ثانية. --- /task ---

--- hints ---
 --- hint ---

```blocks3
when flag clicked
turn LED (17 v) [on v] ::extension
wait (2) secs
turn LED (17 v) [off v] ::extension
wait (2) secs
```

--- /hint ------ /hints ---

--- task --- اجعل LED يعمل ويتوقف طالما أن برنامجك يعمل. --- /task ---

--- hints ---
 --- hint --- استخدم

```blocks3
كرر باستمرار
```

--- /hint --- --- hint ---

```blocks3
when flag clicked
forever
turn LED (17 v) [on v] ::extension
wait (2) secs
turn LED (17 v) [off v] ::extension
wait (2) secs
```

--- /hint ------ /hints ---

+ اجعل وميض LED الخاص بك أكثر سرعة.

--- hints ---
 --- hint --- استخدم كتلة `انتظر x ثواني`{:class="block3control"} لمدة ثوان أقل.
--- /hint ---
 --- hint ---

```blocks3
when flag clicked
forever
turn LED (17 v) [on v] ::extension
wait (0.5) secs
turn LED (17 v) [off v] ::extension
wait (0.5) secs
```

--- /hint ------ /hints ---

أحسنت - أنت الآن على استعداد لإنشاء قوس قزح رائع والتحكم به!