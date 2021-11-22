# Zadanie 1
Program serwera napisany jest na Pythonie. W repozytorium jest plik z komentarzami.

# Zadanie 2
W repozytorium jest plik z komentarzami.

# Zadanie 3


a. zbudowanie opracowanego obrazu kontenera
`docker build -t http .`

b. uruchomienia kontenera na podstawie zbudowanego obrazu
`docker run --name httpserver -p -d 80:7000 http`

c. sposób uzyskania informacji, które wygenerował serwer w trakcie uruchamiania kontenera
`docker logs server`

d. sprawdzenia, ile warstw posiada zbudowany obraz (tu trzeba wcześniej zainstalować jq)
`docker image inspect  http | jq '.[].RootFS.Layers'`
 *Obraz posiada 7 warstw.*

![](https://github.com/dmkard/pco_zad1/blob/main/Resources/screenshot.png)
![](https://github.com/HvVladyslav/Sprawozdanie-1/blob/main/Screen/Screen.png)

# Zadanie 4

Obraz można umieścić na Docker Hub przy pomocy  CI git Hub(workflow). 

