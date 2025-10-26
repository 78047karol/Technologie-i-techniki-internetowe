Instrukcja:
Pliki:
- persons.xml  — przykładowy plik XML z danymi rejestrujących się osób
- persons.dtd  — DTD opisujące strukturę XML (w prostym zakresie)
- persons.xsd  — XSD (XML Schema) z typami i ograniczeniami (np. wiek, enumeracja płci)

Jak weryfikować (np. na FreeFormatter XML Validator):
1. Otwórz stronę FreeFormatter (zakładka XML Validator - XSD).
2. Wklej zawartość persons.xml w polu "XML" (upewnij się, że w deklaracji <!DOCTYPE ...> nazwa pliku DTD to "persons.dtd" — jeśli wklejasz, DTD możesz pominąć lub wkleić w pole DTD).
3. Wklej zawartość persons.xsd w polu "XSD" (jeśli validator pyta o "schema location" użyj persons.xsd lub pozostaw pusty jeśli używasz poleu XSD).
4. Kliknij "Validate" — powinno zwrócić, że dokument jest poprawny względem schematu XSD.

Jak dodać pliki na GitHub (szybko przez web UI):
1. Wejdź do repozytorium → Add file → Upload files → wybierz te 3 pliki → Commit changes.

Uwaga:
- DTD nie narzuca zakresu liczbowego (np. minimalny/maksymalny wiek). To robi XSD.
- W XSD używamy enumeracji dla płci: 'M' lub 'K'.
