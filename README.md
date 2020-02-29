# s4-vuejs-in-taefik-docker
environnement de dev.
Il est crée à partir du blog de "thecodingmachine";
LE FICHIER DOCKER_COMPOSE.YML permettra de lancer docker-compose up -d, 

puis à partir d'une consomle ssh obtenue par 
docker-compose exec app bash:
-Pour symfony le composer install,
-les migrations de la base 
-et les fixtures.

Enfin les outils de débogage pour PHP comme CodeSniffer puis csfix et csCheck, phpStan
et ses plugins: thecodingmachine/phpStan-standard-rules, ou Safe et phpStan-safe-rules

Avec composer on installe le webpack-encore-bundle, puis yarn install.

on ajoute Vue , puis vue-loader, vue-template-compiler, @babel/plugin-transform-runtime et @babel/runtime pour les op asynchrone

Puis les outils de débogage JS:
-eslint, eslint-loader, eslint-plugin-vue, babel-eslint.
-un fichier .eslintrc.JSON 

la branche master comprendra la solution de dev, 
pour tester une spa sur un backend S4 API consommé par axios
