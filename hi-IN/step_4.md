## Scratch में अपने सर्किट का परीक्षण करें

अब आप अपने सर्किट और इंद्रधनुष के पहले रंग को Scratch से जोड़ेंगे, ताकि आप LED को नियंत्रित करने के लिए Scratch प्रोग्राम को कोड कर सकें।

--- task --- अपने Raspberry Pi पर Scratch 3 खोलें।

![open-scratch](images/open-scratch.png) --- /task ---

--- task --- फिर Raspberry Pi Simple Electronics Extension जोड़ें

![add-extension](images/add-extension.png)

![simple-electronics](images/simple-electronics.png) --- /task ---

--- task --- पिछले चरण में, आपने अपने LED को पिन **3V3** से जोड़ा। यदि आप अपने LED का परीक्षण कर रहे हैं तो इसी पिन से कनेक्ट करें। अब आपको अपने LED को एक पिन से कनेक्ट करना होगा जिसे आप Scratch से नियंत्रित कर सकते हैं। पिन **3V3** से वायर को निकले और दूसरे नए पिन में जोड़ें, उदाहरण के लिए **GPIO 17**। --- /task ---

![Move Pin](images/movepin.png)

--- task --- अब परीक्षण करें कि LED को निम्न सरल स्क्रिप्ट का उपयोग करके नियंत्रित किया जा सकता है

```blocks3
when flag clicked
turn LED (17 v) [on v] ::extension
wait (1) secs
turn LED (17 v) [off v] ::extension
```

--- /task ---

--- task --- अपने कोड का परीक्षण करने के लिए हरे झंडे पर क्लिक करें। LED 1 सेकंड के लिए चालू होनी चाहिए। --- /task ---