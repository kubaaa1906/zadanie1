# Zadanie 1
Część dodatkowa:
1. Do stworzenia własnego buildera użyłem polecenia: docker buildx create --name zadanie1builder --driver docker-container -bootstrap
2. Aby ustawić stworzony builder jako domyślny użyłem polecenia: docker buildx use zadanie1builder
3. Do wykonania zadania 2 z części dodatkowej użyłem polecenia: docker buildx build -f Dockerfile -t docker.io/kubaa1906/zadanie1final:zadanie1 --platform linux/amd64,linux/arm64 --push .
   Polecenie działa w następujący sposób: -f Dockerfile = tu podajemy nazwe swojego Dockerfile, z którego ma się zbudować kontener, -t docker.io/kubaa1906/zadanie1final:zadanie1 = podajemy link do repozytorium na DockerHubie,    po znaku : podajemy tag, --platform linux/amd,linux/arm64 --push . = wskazujemy na jakich architekturach będzie działał kontener i pushujemy to na DockerHub.

Link do DockerHub: https://hub.docker.com/repositories/kubaa1906
