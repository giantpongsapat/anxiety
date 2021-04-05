# intro

`SceneSetup.intro();`

# intro-play-button

(...51)

[เล่น!](#intro-start) `publish("intro-to-game-1"); Game.OVERRIDE_CHOICE_LINE=true;`

# intro-start

(...500)

`clearText()`

n3: ก่อนที่จะเริ่ม คุณอยากอ่านเรื่องราวแบบไหน

`publish("show_options_bottom")`

# intro-start-2

n3: ทีนี้ มาเริ่มเรื่องกันเถอะ

```
publish("hide_tabs");
clearText();
```

(...1000)

`publish("intro-to-game-2")`

n2: นี่คือมนุษย์

(...600)

`clearText()`

(...300)

`publish("intro-to-game-3")`

# act1

```
SceneSetup.act1();
publish("hide_tabs");
music('battle', {volume:0.5});
```

(...300)

n: และนี่คือความกังวลของมนุษย์

n: _คุณ_ คือความกังวล

(#act1_normal)


# act1_normal

```
hong({body:"putaway"});
sfx("rustle");
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

h: ไม่ ไม่ ไม่ ไม่ฟัง ฉันจะเช็คโทรศัพท์ละ
```
sfx("rustle2");
hong({body:"phone1", mouth:"neutral", eyes:"neutral"})
```

n: งานของคุณคือการปกป้องมนุษย์จาก *อันตราย*

`bb({eyes:"look", mouth:"small_lock", body:"fear"})`

b: ไม่นะ! เธอเสียเวลาไปกับทวิตเตอร์! อีกแล้วหรอ!

```
bb({eyes:"normal", mouth:"normal", body:"normal"});
hong({eyes:"annoyed"});
```

h: นั่นสิ ทำไมฉันถึงไม่ฟังความคิดของตัวเองบ่อยๆ มั่งนะ

`hong({eyes:"neutral"});`

n: เร็วเข้า เตือนเธอเกี่ยวกับ*อันตราย!*

```
bb({eyes:"look"});
```

[โอ้ ไม่, ดูข่าวที่น่ากลัวนั่นสิ!](#act1d_news)

[โอ้ ไม่, ทวีตนั่นมันนินทา *เรา* หรือป่าว?](#act1d_subtweet)

[เฮ้, GIF แมวดื่มนมนี่นา](#act1d_milk)

# act1d_milk

`hong({mouth:"smile", eyes:"surprise"});`

h: เฮ้ นั่นน่ารักดี ฉัน--

```
hong({mouth:"shock", eyes:"shock"});
bb({body:"scream"});
Game.OVERRIDE_TEXT_SPEED = 1.8;
```

b: แมวมันกินนมไม่ได้และเรากำลังดูแมวถูกทรมาน!

(...200)

```
bb({body:"normal", mouth:"normal", eyes:"fear"});
attack("20p", "bad");
publish("hp_show");
```



