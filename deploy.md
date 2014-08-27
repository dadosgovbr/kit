O Código está sendo editado no master, criado localmente e enviado ao branch gh-pages

Para fazer o deploy do jekyll, fazer ele servir localmente com o parametro baseURL.
Esse parãmetro é importante para manter a integridade de links:

bundle exec jekyll serve --baseurl "/"
