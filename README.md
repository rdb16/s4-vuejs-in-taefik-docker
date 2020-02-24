# s4-vuejs-in-taefik-docker
environnement de dev.
Il est crée à partir du blog de "thecodingmachine";
LE FICHIER DOCKER_COMPOSER.YML permettra de lancer docker-composer up -d, 

puis à partir d'une consomle ssh obtenue par 
docker-composer exec app bash:
-Pour symfony le composer install,
-les migrations de la base 
-et les fixtures.

Enfin les outils de débogage pour PHP comme CodeSniffer puis csfix et csCheck, phpStan
et ses plugins: thecodingmachine/phpStan-standard-rules, ou Safe et phpStan-safe-rules
Avec composer on installe le webpack-encore-bundle, puis yarn install.

on ajoute Vue , puis vue-loader, vue-template-compiler, @babel/plugin-transform-runtime et @babel/runtime pour les op asynchrone

Puis les outils de débogage JS:
-eslint, eslint-loader, eslint-plugin-vue, babael-eslint.
-un fichier .eslintrc.JSON 

la branche master comprendra la solution de dev, puis une branche postMessages
pour tester une spa sur un backend S4 API consommé par axios
