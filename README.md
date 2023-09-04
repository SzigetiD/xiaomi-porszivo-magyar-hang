# xiaomi-porszivo-magyar-hang
Magyar hang, xiaomi/dreame/mijia robotporszívókhoz.

Mindenek előtt felhívnám a figyelmet, hogy mindenki saját felelősségre használja a az alább leírtakat. Semmilyen felelősséget nem tudok vállalni egy esetleges meghibásodásért.
Mivel ezzel a módszerrel a gyári firmware nem kerül átírásra, jelenlegi tudomásom szerint a gyári garanciát nem érinti.

Szükséges elszközök: 
  - Home Assistant
  - Dreame vacuum integráció: https://community.home-assistant.io/t/custom-component-dreame-vacuum/473026
  - Token extraktor: https://github.com/PiotrMachowski/Xiaomi-cloud-tokens-extractor

Mivel én ezeken keresztül állítottam be egyenlőre csak ezt tudom leírni, ha lesz időm visszafejteni a dreame integrációt hogy működik akkor esetleg lesz egy tool ami műküdik.

Lépések:
  - Dreame integráció telepítése és beállítása a leírás alapján: https://github.com/Tasshack/dreame-vacuum/blob/master/README.md
  - dreame_vacuum.vacuum_install_voice_pack service használata:

    - Pareméterek:
      - pack url:  https://github.com/SzigetiD/xiaomi-porszivo-magyar-hang/blob/main/voices/packages/default/6b3bc915549b5fdefa224d44631c3179
      - hash: 6b3bc915549b5fdefa224d44631c3179
      - size: 3784815
      - id: EN
