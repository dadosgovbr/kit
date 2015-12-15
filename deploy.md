O código está sendo editado no master, criado localmente e enviado ao branch
gh-pages.

Para a instalação do Jekyll e outras dependências do Github pages, [veja a
documentação](https://help.github.com/articles/using-jekyll-with-pages/).

Para editar, use o branch master:

    git checkout master

Para fazer o build para uma pasta local, use:

    mkdir /tmp/kit-dados-abertos
    jekyll build --destination /tmp/kit-dados-abertos

Para enviar ao branch gh-pages, use:

    git checkout gh-pages
    cp -R /tmp/kit-dados-abertos/* .

Para atualizar as mudanças no repositório local e enviar ao repositório remoto
(deploy):

    git add .
    git commit -m "[descrição das alterações]"
    git push

Para fazer o deploy local do jekyll, que é útil para visualizar localmente as
akterações, usar o parametro baseURL.
Esse parãmetro é importante para manter a integridade de links:

    bundle exec jekyll serve --baseurl "/"
