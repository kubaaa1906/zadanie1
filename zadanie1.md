# Zadanie 1 - potrzebne polecenia oraz link do DockerHub
Część podstawowa:
1. Polecenie do budowy kontenera: docker build -t zadanie1final .
2. Polecenie do uruchomienia kontenera: docker run -d -p 3000:8081 --name zadanie1final -t zadanie1final
3. Polecenie do uzyskania informacji, które wygenerował serwer w trakcie uruchamiania kontenera: docker logs -f zadanie1final
4. Do sprawdzenia ile warstw posiada obraz, można skorzystać z polecenia: 'docker image inspect zadanie1final' i w listingu szukamy pozycji Layers. Zbudowany obraz posiada 10 warstw.

Część dodatkowa:
1. Do stworzenia własnego buildera użyłem polecenia: docker buildx create --name zadanie1builder --driver docker-container -bootstrap
2. Aby ustawić stworzony builder jako domyślny użyłem polecenia: docker buildx use zadanie1builder
3. Do wykonania zadania 2 z części dodatkowej użyłem polecenia: docker buildx build -f Dockerfile -t docker.io/kubaa1906/zadanie1final:zadanie1 --platform linux/amd64,linux/arm64 --push .

Link do DockerHub: https://hub.docker.com/repositories/kubaa1906
