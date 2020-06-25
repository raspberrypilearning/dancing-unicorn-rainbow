## Control your rainbow circuit

जब आपका पूरा इंद्रधनुष सेट हो जाता है, तो आप नियंत्रित कर सकते हैं कि इंद्रधनुष कैसे प्रकाशित हो। एक LED को नियंत्रित करने का थोड़ा अभ्यास करने के लिए Scratch में निमनलिखित का उपयोग करें:

\--- task \--- जब आप कीबोर्ड पर <kbd>P</kbd> दबाते हैं तब दो सेकंड के लिए LED चालू करें और फिर बंद करें। \--- /task \---

\--- hint \--- \--- hint \--- `Control`{:class="block3control"} ब्लॉक सेक्शन में देखिए। \--- /hint \--- \--- hint \--- निम्नलखित का उपयोग करें

```blocks3
  wait (2) secs
```

\--- /hint \--- \--- hint \---

```blocks3
when [p v] key pressed
turn LED (17 v) [on v] ::extension
wait (2) secs
turn LED (17 v) [off v] ::extension
```

\--- /hint \--- \--- /hints \---

\--- task \--- जब आपका Scratch प्रोग्राम शुरू होता है, तो अपना LED 2 सेकंड के लिए प्रकाशित करें और फिर 2 सेकंड के लिए बंद करें। \--- /task \---

\--- hints \--- \--- hint \---

```blocks3
when flag clicked
turn LED (17 v) [on v] ::extension
wait (2) secs
turn LED (17 v) [off v] ::extension
wait (2) secs
```

\--- /hint \--- \--- /hints \---

\--- task \--- जब तक आपका प्रोग्राम चलता है, तब तक अपना LED चालू और बंद करें। \--- /task \---

\--- hints \--- \--- hint \--- निम्नलखित का उपयोग करें

```blocks3
forever
```

\--- /hint \--- \--- hint \---

```blocks3
when flag clicked
forever
turn LED (17 v) [on v] ::extension
wait (2) secs
turn LED (17 v) [off v] ::extension
wait (2) secs
```

\--- /hint \--- \--- /hints \---

+ अपना LED जल्दी बंद चालू करें।

\--- hints \--- \--- hint \--- कुछ सेकंड के लिए `wait x secs`{:class="block3control"} का उपयोग करें \--- /hint \--- \--- hint \---

```blocks3
when flag clicked
forever
turn LED (17 v) [on v] ::extension
wait (0.5) secs
turn LED (17 v) [off v] ::extension
wait (0.5) secs
```

\--- /hint \--- \--- /hints \---

शाबाश - अब आप एक बहुत बढ़िया इंद्रधनुष बनाने और नियंत्रित करने के लिए तैयार हैं!