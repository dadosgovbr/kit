O Código está sendo editado no master, criado localmente e enviado ao branch gh-pages

Para fazer o deploy do jekyll, fazer ele servir localmente com o parametro baseURL.
Esse parãmetro é importante pois no github a página está em /kit/:

bundle exec jekyll serve --baseurl "/kit/"
