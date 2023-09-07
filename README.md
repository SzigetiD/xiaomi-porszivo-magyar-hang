# xiaomi-porszivo-magyar-hang
Magyar hang, xiaomi/dreame/mijia robotporszívókhoz.

Mindenek előtt felhívnám a figyelmet, hogy mindenki saját felelősségre használja a az alább leírtakat. Semmilyen felelősséget nem tudok vállalni egy esetleges meghibásodásért.
Mivel ezzel a módszerrel a gyári firmware nem kerül átírásra, jelenlegi tudomásom szerint a gyári garanciát nem érinti.

Szükséges elszközök: 
  - Home Assistant
  - Dreame vacuum integráció: https://community.home-assistant.io/t/custom-component-dreame-vacuum/473026
  - Token extraktor: https://github.com/PiotrMachowski/Xiaomi-cloud-tokens-extractor

Mivel én ezeken keresztül állítottam be egyenlőre csak ezt tudom leírni, ha lesz időm visszafejteni a dreame integrációt hogy működik akkor esetleg lesz egy tool ami műküdik.
Egyelőre a saját magam által készített magyar hangokat lehet telepíteni a lenti módszerrel ami lazább/viccesebb hangvételű, a forrásban meg lehet őket előre hallgatni: https://github.com/SzigetiD/xiaomi-porszivo-magyar-hang/tree/main/voices 
Az én gépemben (x10+) sikerült a hangok 95%-át lefedni. Folyamatosan fogom bővíteni.

Lépések:
  - Dreame integráció telepítése és beállítása a leírás alapján: https://github.com/Tasshack/dreame-vacuum/blob/master/README.md
  - dreame_vacuum.vacuum_install_voice_pack service használata:

    - Pareméterek:
      - Language ID: "FR" (vagy bármelyik választható nyelv az appban, érdemes nem az angolt választani)
      - URL:  "https://github.com/SzigetiD/xiaomi-porszivo-magyar-hang/blob/main/voices/packages/default/6b3bc915549b5fdefa224d44631c3179"
      - MD5: 6b3bc915549b5fdefa224d44631c3179
      - Size: 3784815
      
