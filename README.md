**Zadatak**. Ovaj se zadatak nastavlja na prethodni zadatak _Vector_ i treba ga
napraviti u repozitoriju za _Vector_ malom doradom koda.

- Napraviti **univerzalni konstruktor** koji se oslanja na pretpostavke da objekt 
  koji služi za izgradnju novog vektora ima metodu `size()` i iterator (`begin()`
  i `end()` metode). Pomoću `std::enable_if` eliminirati novi konstruktor kao 
  konstruktor kopije i kao konstruktor koji uzima duljinu vektora kako ne bi 
  preuzeo funkciju drugih konstruktora. Koristiti elemente `<type_traits>` zaglavlja.
- Testirati novi konstruktor. Obilježiti sve konstruktore kako bi se moglo provjeriti 
  da se uvijek poziva odgovarajući konstruktor. 
- Napraviti **univerzalni operator pridruživanja** koji se oslanja na pretpostavke da objekt
  na desnoj strani ima metodu `size()` i iterator (`begin()`   i `end()` metode). 
  Eliminirati eventualnu koliziju s običnim operatorom/ima pridruživanja i napisati 
  testove.  
- Implementirati metodu `emplace(index, args..)` koja na mjestu s indeksom `index` 
  konstruira element vektora prenoseći argumente `args` konstruktoru tipa `T` (parametar
  predloška). Implementirati **savršeno prolijeđivanje**. Testirati metodu.
- Preopteretiti operatore indeksiranja po referencijskoj oznaci. Osigurati da se 
  operator pridruživanja ne može pozvati na desnoj vrijednoosti.
 
