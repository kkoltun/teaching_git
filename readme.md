# Zasada Pojedynczej Odpowiedzialności

## Ogólnie

* Pierwsza z zasad składających się na S.O.L.I.D. (S to SRP czyli Single Responsibility Principle).
* Mówiąc ogólnie: **każdy moduł (w naszym ujęciu jest to klasa) powinien odpowiadać za jak najmniejszy fragment logiki programu**.
* Robert C. Martin (Uncle Bob): **klasa powinna mieć tylko jeden powód do zmiany**.

## Przykład 

* Obiekt: moduł składający raport z różnych danych i go drukujący.
* Pierwszy powód do zmian: zmiana zawartości raportu lub danych wchodzących w jego skład.
* Drugi powód do zmian: zmiana formatu wydrukowanego raportu.

Powody obu zmian są różne:
* Zmiana zawartości raportu to zmiana raczej fundamentalna.
* Zmiana formatu, *layoutu* raportu to zmiana raczej kosmetyczna.

Wniosek:
* Moduł ma dwie różniące się znacznie odpowiedzialności dotykające różnych sfer raportów.
* Należy rozdzielić te funkcjonalności i nie doprowadzić do sytuacji w której są ze sobą nadmiernie powiązane.
