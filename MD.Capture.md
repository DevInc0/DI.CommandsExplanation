## /capture

- ***Разрешение:*** `capture`

- ***Параметры:***

  - **[] - Обязательный параметр. <> - Дополнительный параметр**

  - ```
    set team base [Название команды]
    
    Устанавливает место спавна определённой команды на Вашей позиции
    ```
  - ```
    set zone [Название] [Количество игроков для начала захвата] [Время захвата] [Радиус зоны]
    
    Устанавливает зону с определённым названием с центром на Вашей позиции и соответствующими параметрами
    ```
  - ```
    modify zone [Название зоны] [players/time/radius/position/name] <Новое значение>
    
    players - количество игроков для захвата - /capture modify zone "Falcon Base" players 10
    time - время захвата - /capture modify zone "Falcon Base" time 50
    radius - радиус зоны - /capture modify zone "Falcon Base" radius 100
    position - центр зоны - /capture modify zone "Falcon Base" position
    name - имя зоны - /capture modify zone "Falcon Base" name "City downtown"
    
    Меняет определённый параметр у зоны
    ```
  - ```
    remove zone [Название зоны]
    
    Удаляет зону с определённым названием
    ```
  - ```
    remove soldier [Steam64/Имя игрока] <kick>
    
    kick - кикнуть игрока с сервера после удаления информации
    
    Удаляет информацию о солдате
    ```
  - ```
    change soldier stat [kills/captures/fightoff/reprimands/encouragements] [Steam64/Имя игрока] [Новое значение]
    
    kills - количество убийств - /capture change soldier stat kills Бен 100
    captures - количество захваченных точек - /capture change soldier stat captures Бен 0
    fightoff - отбитые точки - /capture change soldier stat fightoff Бен 0
    reprimands - выговоры - /capture change soldier stat reprimands Бен 10
    encouragements - поощрения - /capture change soldier stat encouragements Бен 273
    
    Изменяет определённую статистику солдата
    ```
