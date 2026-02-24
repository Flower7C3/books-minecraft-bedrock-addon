# Książki – Modlitwy i Katechizm

Paczka behawioralna do **Minecraft Bedrock Edition** z książkami.

## Zawartość

### Katechizm

- Błogosławieństwa Ewangeliczne  
- Cnoty  
- Grzechy przeciwko Duchowi Świętemu  
- Pięć warunków dobrej spowiedzi  
- Przykazania Boże  
- Przykazania kościelne  
- Przykazania miłości  
- Siedem grzechów głównych  
- Sześć Prawd Wiary  

### Modlitwy

- Akt wiary, nadziei, miłości i żalu  
- Aniele Boży  
- Anioł Pański  
- Modlitwa Pańska  
- Pozdrowienie Anielskie  
- Wyznanie wiary (Skład Apostolski i Credo)  

## Instalacja

1. Pobierz plik `.mcpack` z [releases](../../releases) (lub zbuduj paczkę samodzielnie).
2. Otwórz Minecraft Bedrock Edition.
3. Przejdź do **Ustawienia → Zasoby globalne → Moje pakiety**.
4. Wybierz **Import** i wskaż pobrany plik.
5. Włącz paczkę w wybranym świecie.

## Użycie

Książki są wydawane przez **loot table** – przy każdym wywołaniu gracz otrzymuje **wszystkie książki** z danej grupy.

### Z poziomu gry (cheaty włączone)

- **Katechizm:**  
  `/loot give @s loot katechizm`
- **Modlitwy:**  
  `/loot give @s loot modlitwy`

### Funkcja (np. z przycisku / command block)

W pliku `BP/functions/give_prayer_books.mcfunction` znajduje się przykład – wywołanie funkcji daje graczowi wszystkie książki katechizmowe i wszystkie modlitwy.

## Źródła i autorzy

- Treści: [modlitwa.katolicki.net](http://modlitwa.katolicki.net/)  
- Modlitwa Pańska, Przykazania, Błogosławieństwa: tradycja biblijna / Ewangelia  
- *Aniele Boży* (tekst polski): Karol Antoniewicz  
- Pozostałe modlitwy i katechizm: autorzy anonimowi / tradycja  

## Wymagania

- Minecraft Bedrock 1.20.0 lub nowszy  

## Licencja

**Kod** (struktura paczki, loot table, skrypty): [MIT](LICENSE).

Treści modlitw i katechizmu należą do ich autorów i źródeł (patrz sekcja Źródła i autorzy).
