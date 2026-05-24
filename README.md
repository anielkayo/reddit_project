Cel badania: Analiza dynamiki agresji w sieciach społecznościowych na przykładzie interakcji między politycznymi subreddittami (nacechowanymi politycznie)

Temat projektu: Analiza dynamiki agresji i polaryzacji w sieciach społecznościowych na przykładzie interakcji między subreddittami politycznymi a hobbystycznymi.
Pytanie badawcze: Czy społeczności o sprecyzowanych poglądach politycznych wykazują statystycznie wyższy poziom agresji wobec innych grup niż społeczności neutralne tematycznie?
Cel projektu: Identyfikacja wzorców zachowań agresywnych w sieci Reddit oraz stworzenie modelu klasyfikującego stopień wrogości między subreddittami w zależności od ich profilu tematycznego.
1. Hipoteza "Eskalacji Emocjonalnej"

Treść: „Prawdopodobieństwo wystąpienia linku negatywnego między dwoma subredditami wzrasta, jeśli w poprzednich 24 godzinach wystąpiły między nimi interakcje o wysokim natężeniu słownictwa związanego z gniewem (anger)”.   + HuggingFace Transformers wykorzystujemy własne właściwości- samemu wykonać analizę- bardziej zaawansowane (rok 2017r) - nowsze modele i biblioteki pythona


Uzasadnienie: To hipoteza dynamiczna. Pozwala sprawdzić, czy konflikty na Reddicie wybuchają nagle, czy są poprzedzone "fazą zapalną" widoczną w parametrach tekstowych.

BADAMY/ POTRZEBNE INFORMACJE:
1) nazwy subredditów
2) czy dany link był negatywny/ sarkastycznie negatywny -> nacechowanie linka
3) data linka - przedział czasowy
4) natężenie słownictwa związanego z gniewem- niska/wysoka agresja

zmienna lingwistyczno- czasowa- CZY negatywny oraz W JAKIM czasie; CZY W CIĄGU 24H OD OPUBLIKOWANIA POSTA  pojawiła się kolejna interakcja z odpowiedzią na tego subreddita

2. Hipoteza "Złożoności Poznawczej"

Treść: „Teksty towarzyszące negatywnym linkom mają niższą złożoność językową (np. krótsze słowa, mniej spójników logicznych) niż teksty w linkach pozytywnych”.

Uzasadnienie: Często agresja wiąże się z uproszczonym widzeniem świata. Możemy to zweryfikować, korelując sentyment z miarami takimi jak średnia długość słowa lub wskaźnik czytelności, które można wyliczyć z body properties.

3. Hipoteza 3: Multimodalna (Najsilniejsza badawczo)

"Modele uczenia maszynowego (np. Random Forest) potrafią przewidzieć wystąpienie negatywnego odniesienia między dwiema społecznościami ze skutecznością (F1-score) powyżej 75%, łącząc cechy lingwistyczne (czas przyszły, emocje) z cechami strukturalnymi sieci (wspólni sąsiedzi, dotychczasowa historia interakcji).”

