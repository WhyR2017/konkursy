# Dane z formularza rejestracyjnego

Repozytorium zawiera dane z formularza rejestracyjnego na

> Ogólnopolską Konferencję Użytkowników R - [Why R? 2017](http://whyr.pl/)

Dane zostały pozbawione informacji o imionach, nazwiskach, adresach e-mail oraz afiliacjach uczestników.
Formularz wypełniali zarówno uczestnicy, jak i prelegenci, prowadzący warsztaty, zaproszeni goście oraz organizatorzy konferencji. Formularza nie wypełniały osoby z biletów oferowanych sponsorom, fotografowie (również osoby z branży analizy danych) ani przedstawiciele władz Wydziałów MiNI PW czy MIMUW.

Dane zawierają 183 rekordy osób, które poprzez wpłatę bądź status (organizator, prowadzący warsztaty) potwierdziły swój udział na konferencji oraz 63 rekordy osób, które zrezygnowały poprzez niewniesienie opłaty konferencyjnej.

> Poza konkursem mogę przekazać, że na konferencji będzie równo 200 uczestników.

Dane zawierają informacje o zainteresowaniach, obszarach działań uczestników oraz ich doświadczeniu (w latach) związanym z analizą danych oraz programowaniem w R. Dane zawierają również datę urodzin, kraj pochodzenia oraz miasto. Dodatkowo można sprawdzić stopień naukowy uczestników oraz wybrane przez nich warsztaty.

# Jak wczytać?

Dane do R można wczytać poleceniem

```{r}
library(RCurl)
formularz <- getURL("https://raw.githubusercontent.com/whyRconf/konkursy/master/dane_z_formularza_rejestracyjnego.csv")
dane <- read.csv(text = formularz)
```

# Wizualizacje wykonane przez Ewę Baranowską

Ewa Baranowska z [Koła Naukowego Data Science PW](http://datascience.mini.pw.edu.pl/) przygotowała wcześniej pewne wizualizacje tego zbioru, które można zobaczyć pod adresem [whyr.pl/wizualizacje/](http://whyr.pl/wizualizacje/).

# Pytania

W razie pytan zachęcam do korzystania z panelu dyskusyjnego pod opisem konkursu na wizualizację danych [tutaj](http://whyr.pl/blog/info/2017/09/10/konkurs-PwC.html).