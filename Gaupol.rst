
Subtitles (Legendas)
====================

Ideias:

* O método mais eficaz talvez seja teclar de raiz as legendas usando o Gaupol (por exemplo) e a sequência de etapas abaixo mencionadas.
* A transcrição automática de legendas pode ser útil: via youtube ou via reconhecimento com "CMU speech recognition" (sem ainda saber qual a sequência de comandos para o ativar; este projeto parou em 2009!?!?)

Nota:

* legndas = subtítulos (brasil) = subtitles

Leituras:

* https://www.dcmp.org/ciy/converting-youtube-to-srt.html

Extração de legendas existentes
-------------------------------

* Se já existem no youtube talvez se possa ter sucesso com  `http://keepsubs.com/`_
* Ou usar o reconhecimento do youtube e posterior edição (de seguida).

Reconhecimento automático de voz
--------------------------------

Comandos e ideias que podem ser úteis:

* Youtube.com, "O Meu Canal" => "Gestor de Videos" (linha por cima do banner)
* O próprio youtube tem um editor: carrega-se o video na "área pessoal", editar as legendas: teclar as palavras e depois o youtube encaixa os tempos (não tentei ainda).
* Fazer edição de legendas dentro do próprio Youtube.
* Parece que o Youtube faz reconhecimento de fala automatico e produz legendas mas não parece ser imediatamente.

   * Carregar o video no youtube na conta pessoal
   * Esperar que as legendas automáticas surgam (demora um dia?? É automático?)
   * Descarregar o SRT (Gestor de Videos, Legendas, Acções)
   * Editar as legendas 


Sobre o Gaupol
--------------

Permite a edição de legendas (e lê-se que faz transcrição automática na versão 0.19??)

http://home.gna.org/gaupol/

Passos básicos e ideias gerais:

* File -> New
* File -> Save As  (gravar mesmo vazio)
* Video -> Load  (carregar o video)
* até agora não soube associar o "projeto" a um video e suas legendas. 
* Tecla "O" repete a voz apenas da linha corrent (incluindo uma palavra da linha anterior e uma da linha seguinte.)
* Teclas I, J e K são úteis.


Algoritmo bastante eficaz:

0. Posicionar o vido no início ou onde se quer.
1. Abrir uma legenda nova com tecla I (abre uma legenda de duração padrão de 3 segundos).
2. Carregar em O para ouvir a palavra na legenda anterior e ouvir até aos 3 segundos; depois pode ouvir-se mais um pouco carregando em P.
3. Logo após a tecla O, faze-se ENTER que edita a célula e também termina a edição da célula;  
4. Transcreve-se tudo, repetindo as teclas O e P, parando o som no instante que coincide com o texto na legenda criada.
4. Carregar K nesse instante, para acertar o fim do tempo da legenda com o tempo no video.
5. Carregar I para inserir apenas mais 1 legenda.

* Repetir.
* Lembrar de fazer CTRL-S para ir gravando.


Instalar o Gaupol 
-----------------

É melhor, no ubuntu, usar a versão padrão.

Para versões seguintes (não vi vantagem ainda):

https://github.com/otsaloma/gaupol/blob/master/INSTALL.md



**0.26**
--------

For Ubuntu 14.10, Gaupol 0.26 is available via the default repositories, so all you have to do is:

::

   $ sudo apt-get update
   $ sudo apt-get install gaupol

Gaupol 0.26 is not available via any PPA for Ubuntu 14.04, Linux Mint 17, Elementary OS 0.3 and other Ubuntu 14.04 derivative systems, so we have to download the gaupol archive, extract it and execute the python installer:

::

   $ wget http://download.gna.org/gaupol/0.26/gaupol-0.26.tar.xz
   $ tar -xJvf gaupol-0.26.tar.xz
   $ cd gaupol-0.26
   $ sudo python3 setup.py clean install


Speach recognition

::
   sudo apt-get install python-pocketsphinx

https://wiki.gnome.org/Apps/Gaupol/SpeechRecognition#Speech_Recognition_Menu_Item_Is_Unavailable


http://cmusphinx.sourceforge.net/wiki/tutorial








