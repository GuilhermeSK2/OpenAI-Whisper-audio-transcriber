# Transcrição de Áudio com OpenAI Whisper

Este projeto demonstra a utilização do modelo OpenAI Whisper para realizar a transcrição automática de áudio para texto (Speech-to-Text - STT). Além de transcrever o conteúdo falado, o modelo também é capaz de detectar o idioma presente no áudio.

## Visão Geral

O OpenAI Whisper é um modelo de STT (Speech-to-Text) altamente performático e robusto, treinado em uma vasta quantidade de dados de áudio multilíngues. Ele se destaca na transcrição de áudios em diversos idiomas e com diferentes qualidades de som. Este projeto oferece um script simples para:
1.  Carregar um modelo Whisper pré-treinado.
2.  Processar um arquivo de áudio.
3.  Retornar a transcrição do texto e o idioma detectado.
4.  Salvar a transcrição em um arquivo de texto.

## Estrutura do Projeto

* `Whisper.ipynb`: O notebook Jupyter que contém todo o código para instalação das dependências, carregamento do modelo, transcrição do áudio e salvamento do texto.
* `teste.mp3`: Um arquivo de áudio de exemplo (você pode substituí-lo pelo seu próprio arquivo de áudio).

## Tecnologias Utilizadas

* **Python 3**
* **`openai-whisper` library**: A implementação oficial do modelo Whisper.
* **Jupyter Notebook**: Para execução e demonstração interativa do código.

## Pré-requisitos

Para usar este projeto, você precisará de um arquivo de áudio para transcrever. O exemplo usa `teste.mp3`. Certifique-se de que o arquivo de áudio que você deseja transcrever esteja no mesmo diretório do notebook ou forneça o caminho completo para ele.

## Modelos Whisper Disponíveis

O Whisper possui diversos tamanhos de modelo, que variam em precisão e velocidade:
* `tiny`
* `base`
* `small`
* `medium`
* `large`

Você pode alterar `whisper.load_model("base")` para um modelo diferente (ex: `"small"`) dependendo da sua necessidade de precisão versus velocidade. Modelos maiores geralmente são mais precisos, mas exigem mais recursos computacionais e tempo de processamento.

## Saída

O script imprimirá a transcrição do áudio e o idioma detectado no console do Jupyter. Além disso, a transcrição completa será salva em um arquivo chamado `arquivo.txt` no mesmo diretório.
