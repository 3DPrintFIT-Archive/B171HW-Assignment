# Tablet Bar Mount

Své repo vytvoříte na https://classroom.github.com/a/my7o3Upb

Deadline je **7.1.2018** 23:59 CET. Vypracovaný úkol **nahrajte do repozitáře vytvořeného na odkaze výše**. Nikam jinam jej neposílejte, jako odevzdání se počítá to, co bude ve vašem repozitáři (ve výchozí větvi (většinou `master`)) v momentu deadlinu.

**Pokud máte jakékoliv dotazy, či naleznete chyby, napište je prosím do Issues k tomuto repozitáři.**

## Motivace

Nic podobného neexistuje, i přes poptávku motorkářů, čili po splnění úkolu ho můžete opensourcovat a publikovat například na Thingiverse nebo podobných webech a býti slavní... :)

## Zadání

Vaším úkolem je namodelovat držák na tablet na řídítka motocyklu, za účelem použití tabletu k navigaci.
Držák tabletu je potřeba namontovat na představce řídítek, protože to je nejbezpečnější a zároveň nejpevnější místo, které je jezdci snadno na očích.

## Model

Vámi namodelovaný model se bude skládat ze dvou objektů.

  - Horní část modelu s výřezem pro display tabletu
  - Spodní část modelu, který se dá přídělat na přestavce řídítek
  - Je nezbytné aby vámi naprogramovaný model byl správně umístěn do souřadnic
    - Spodní část objímek musí ležet na `z = 0`
    - Střed rozteče objímek musí ležet na `x = 0` a `y = 0`
    - Řídítka motocyklu jsou rovnoběžné s osou x
    - Jezdec se na tablet dívá ze záporného směru po ose y (tedy dívá se kladným směrem)
    - Samostatně použitý `top_part` leží na podložce (`z = 0`), vystředěn podle os x a y
        - 
