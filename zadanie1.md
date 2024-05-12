# Zadanie 1
Część podstawowa:
1. Polecenie do budowy kontenera: docker build -t zadanie1final .
2. Polecenie do uruchomienia kontenera: docker run -d -p 3000:8081 --name zadanie1final -t zadanie1final
3. Polecenie do uzyskania informacji, które wygenerował serwer w trakcie uruchamiania kontenera: docker logs -f zadanie1final
4. Do sprawdzenia ile warstw posiada obraz, można skorzystać z polecenia: 'docker image inspect zadanie1final' i w listingu szukamy pozycji Layers. Zbudowany obraz posiada 10 warstw.

