# slideshow

## Nesse projeto, a página vai exibir uma sequência de imagens de modo autônomo.

O script inicia capturando as propriedades do elemento identificado com a classe "slideshow", através do comando "document.querySelector". Tem uma variável com um "array" com o caminho das imagens do projeto.

Há uma variável que recebe o tempo que o slide irá demorar para passar as imagens, nesse caso o valor "2000" que representa 2 segundos em milisegundos. E mais uma variável que tem a funçao de contagem no código, com o valor "0".

Na função "moveSlideShow", a variável "slide" que contém as propriedades do elemento "img", recebe o primeiro item da lista de imagens. O array de imagens recebe o valor inicial do contador como posição.

Em seguida a função realiza uma verificação observando se o valor do contador é menor que o total de imagens na lista. Em caso positivo, significa que ainda há imagens para exibir, por isso tem seu valor acrescido de um. Caso contrário o valor do contador é zerado e o slide é reiniciado exibindo novamente a primeira imagem.

Ao final um método javascript "setTimeout" responável por executar um determinado trecho de código a cada periodo de tempo. Para o método passamos como parâmetro a função e o tempo que definimos anteriormente. Assim, a função será executada repetidas vezes, a cada 2 segundos, realizando as alterações das imagens.

Por último a função "window.onload" que é uma propriedade javascript executada quando a página carrega pela primeira vez.