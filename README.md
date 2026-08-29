# **ocr_APAE**  
**Processamento em OCR de arquivos de dados da APAE para uso em regional de saúde.**

Esse projeto tem como objetivo facilitar o processamento de arquivo no formato PDF com dados de sorologia de pacientes atendidos pela APAE de Goiânia.  
Os dados contidos neste arquivo são imagens, o que dificulta a manipulação das informações contidas neste documento.  
Com a finalidade de tornar o processamento das informações contidas neste arquivo mais fácil, rápido e eficiente, o projeto OCR_APAE converte os dados do documento PDF de imagens para um documento PDF com texto editável. Em seguida este último arquivo criado é transformado em um arquivo de texto, que pode ser trabalhado em qualquer ferramenta de processamento de texto, como o bloco de notas do Windows, por exemplo.

## Como usar?
1)Faça o download do arquivo da última versão do programa. O arquivo sempre estará no formato zip;  
2)Descompacte o arquivo usando algum utilitário para extração de arquivos zipados. Ao final do processo de descompactação, haverá uma pasta com o nome "ocr_APAE";  
3)Copie esta pasta para o disco local C ou unidade C da unidade de armazenamento do PC que você está usando;  
4)Dentro da pasta "ocr_APAE", procure a subpasta "original_PDF" e coloque o arquivo PDF original criado pela APAE;  
5)Renomeie esse arquivo PDF original da APAE para o nome "sifilis.pdf";  
6)Dentro da pasta "ocr_APAE", procure a subpasta "bat" e rode o arquivo "run_apae.bat";  
7)Quando o processo terminar, procure na pasta "ocr_APAE" a subpasta "txt_out", haverá um arquivo com o nome "apae_sifilis.txt". Este é o arquivo de texto resultado do processamento do programa;  

## Créditos
Para realizar o processamento do arquivo, o "ocr_APAE" utiliza vários programas para tornar possível o resultado final.  

*NAPS2 (https://www.naps2.com)* - NAPS2 é um programa para digitalização de documentos gratuito e de código fonte aberto para Windows, Mac e Linux. Neste projeto, o NAPS2 é utilizado para realizar a transformação das imagens contidas no arquivo PDF em um arquivo PDF com texto editável, para isso o NAPS2 usa o recurso de reconhecimento optico de caracteres (OCR), nativo do produto. 
  
*XpdfReader (https://www.xpdfreader.com)* - XpdfReader é um projeto gratuito e de código aberto que possui uma coleção de ferramentas que rodam em linha de comando que permitem realizar várias funções em arquivos PDF. No projeto "ocr_APAE" é usada uma destas ferramentas, o "pdftotext", que transforma um arquivo PDF editável em um arquivo de texto (formato txt).  

*iconv for Windows (https://github.com/mlocati/gettext-iconv-windows)* - é um projeto de código aberto que compila o iconv usado no Linux e mantido pela Free Software Foundation em um arquivo binário para execução no sistema operacional Windows. No "ocr_APAE", o iconv foi usado para fazer a transliteração do arquivo de texto gerado do XpdfReader, separando a acentuação dos caracteres.  

*Gawk for Windows (https://gnuwin32.sourceforge.net/packages/gawk.htm)* - AWK é uma linguagem de programação interpretada projetada para processar, filtrar e manipular dados em arquivos de texto. No gawk for Windows, a letra "g" junto ao awk, significa GNU, que é um sistema operacional tipo Unix, criado para oferecer um sistema completo e totalmente composto por software livre. Nessa implementação para o Windows, o AWK é usado, no "ocr_APAE", para remover a acentuação aguda no arquivo de texto após a transliteração executada pelo "iconv for Windows";  

*sed for Windows (https://gnuwin32.sourceforge.net/packages/sed.htm) - Assim como o Gawk for Windows, o sed for Windows é outro projeto gratuito e de código aberto, apoiado e mantido pela Free Software Foundation. O sed é um editor de fluxo (stream editor) usado para filtragem e transformação de texto. No "ocr_APAE", o sed é usado para remover caracteres de acentuação soltos no texto, remoção de linhas em branco, remover linhas de texto em que ocorrem determinadas palavras no texto, etc.  
  










