# s4-vuejs-in-taefik-docker
environnement de dev.
Il est crée à partir du blog de "thecodingmachine";
LE FICHIER DOCKER_COMPOSER.YML permettra de lancer docker-composer up -d, 
puis à partir d'une consomle ssh :
-Pour symfony le composer install,
-les migrations de la base 
-et les fixtures.

Enfin les outils de débogage pour PHP comme CodeSniffer puis csfix et csCheck, phpStan
et ses plugins: thecodingmachine/phpStan-standard-rules, ou Safe et phpStan-safe-rules

Pour Vue.js et les outils de débogage pour JS le yarn install. 

la branche master comprendra la solution de dev, puis une branche postMessages
pour tester une spa sur un backend S4 API consommé par axios
