* Zasada otwarte-zamknięte (ang. Open/Closed principle)

**Elementy systemu takie, jak klasy, moduły, funkcje itd. powinny być otwarte na [rozszerzenie|modyfikacje], ale zamknięte na [rozszerzenie|modyfikacje].**

Oznacza to, że [można zmienić zachowanie modułu elementu bez zmiany jego kodu|zawsze należy wprowadzać zmiany w kodzie modułu].
Jest to szczególnie ważne w środowisku produkcyjnym, gdzie zmiany kodu źródłowego mogą być [wskazane|niewskazane].

Program, który trzyma się tej zasady, [wymaga|nie wymaga] zmian w kodzie.