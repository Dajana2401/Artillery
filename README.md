Zadanie 5 interpretacja wyników:
Wykonuję test obciążeniowy dla API "https://postman-echo.com/", dodając w czasie 3 sekund 2 wirtualnych użytkowników na sekundę,
sprawdzam jak serwer poradzi sobie z takim obciążeniem poprzez sprawdzanie czasu odpowiedzi, ilości otrzymanych statusów 200 (ok), ilości poprawnie utworzonych użytkowników. 
Wykonuję żądanie POST dla API, ponieważ jest to API otwarte to powinnam dostać w odpowiedzi to co wysyłam. Sprawdzam to poprzez wylogowanie 
odpowiedzi z żądania POST- zgadza się. Dodatkowo sprawdzam żądanie POST dla danych z pliku zewnętrznego poprzez dodanie sekcji payload. Serwer poprawnie zwraca przesłane żądanie. 
Wykonuję sprawdzenie 3 metryk z raportu, chcę aby http.request_rate był mniejszy bądź równy 2 i http.response_time.max mniejszy niż 600 milisekund- w sekcji check dostaję odpowiedź OK, czyli warunek spełniony.
Dodatkowo chcę, aby vusers.failed był równy 0- w sekcji check dostaję odpowiedź OK, czyli warunek spełniony.
Ponadto chcę, aby http.response_time.p95 (czas odpowiedzi dla 95 procent użytkownków) był mniejszy niż 500 milisekund- w sekcji check dostaję odpowiedź OK, czyli warunek spełniony.
