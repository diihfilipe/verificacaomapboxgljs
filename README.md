##Verificação de compatibilidade Mapbox GL JS

###Porque isso?

A tecnologia de renderização de mapas 3D bem como outras funcionalidades do Mapbox exigem que o navegador suporte a tecnologia WebGL, a maioria dos navegadores modernos oferece esse suporte nativamente, porém podem haver algumas incompatibilidades por exemplo com as configurações do computador e/ou sistema operacional. Abaixo temos uma 'blacklist' de configurações que NÃO suportam o WebGL.

* Em todas as versões do Windows, o WebGL é desativado em todos os drivers gráficos mais antigos do que Janeiro de 2009.
* Adicionalmente, no Windows XP, o WebGL é desativado nos drivers da ATI/AMD mais antigos do que a versão 10.6, nos drivers da NVIDIA mais antigos do que a versão 257.21 e nos drivers da Intel mais antigos do que a versão 14.42.7.5294.
* O WebGL é desativado no driver NVIDIA versão 6.14.11.9621 no Windows XP.
* O WebGL é sempre desativado no driver da ATI FireNV 2400.
* O WebGL é desativado nos drivers da Parallels mais antigos do que a versão 7.
* o WebGL é sempre desativado nos drivers da S3 Trio.

Para vefificar a compatibilidade do seu computador com essa tecnologia acesse http://mapbox.github.io/mapbox-gl-supported/, caso retorne a mensagem de erro 'MAPBOX GL JS NOT SUPPORTED' siga os passos abaixo.

###Como ativar o WebGL no seu navegador(Google Chrome):

* A opção "Usar aceleração de hardware quando disponível" deve estar ativada no Chrome para que o mesmo utilize a tecnologia WebGl. (Basta acessar as configurações do chrome e procurar por "aceleração de hardware").

* Acessar chrome://flags/ no seu navegador e buscar pela opção WebGL 2.0 e alterar para ENABLE.
(imagem)

* E por fim acessar a pagina  http://mapbox.github.io/mapbox-gl-supported/ e verificar se o retorno é "MAPBOX GL JS IS SUPPORTED".

###ALTERNATIVAS:

baixar e instalar o chrome canary (uma versão beta do google chrome que oferece mais compatibilidade com esta tecnologia) https://www.google.com.br/chrome/browser/canary.html.
