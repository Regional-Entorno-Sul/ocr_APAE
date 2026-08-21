# **ocr_APAE**  
**Processamento em OCR de arquivos de dados da APAE para uso em regional de saúde.**

Esse projeto tem como objetivo facilitar o processamento de arquivo no formato PDF com dados de sorologia de pacientes atendidos pela APAE de Goiânia.  
Os dados contidos neste arquivo são imagens, o que dificulta a manipulação das informações contidas neste documento.  
Com a finalidade de tornar o processamento das informações contidas neste arquivo mais fácil, rápido e eficiente, o projeto OCR_APAE converte os dados do documento PDF de imagens para um documento PDF com texto editável. Em seguida este último arquivo criado é transformado em um arquivo de texto, que pode ser trabalhado em qualquer ferramenta de processamento de texto, como o bloco de notas do Windows, por exemplo.

## Como usar?
Faça o download do arquivo da última versão do programa. O arquivo sempre estará no formato zip;  
Descompacte o arquivo usando algum utilitário para extração de arquivos zipados. Ao final do processo de descompactação, haverá uma pasta com o nome "ocr_APAE";  
Copie esta pasta para o disco local C ou unidade C da unidade de armazenamento do PC que você está usando;  
Dentro da pasta "ocr_APAE", procure a subpasta "original_PDF" e coloque o arquivo PDF original criado pela APAE;  
Renomeie esse arquivo para o nome "sifilis.pdf";  
Dentro da pasta "ocr_APAE", procure a subpasta "bat" e rode o arquivo "run_apae.bat";  
Quando o processo terminar, procure na pasta "ocr_APAE" a subpasta "txt_out", haverá um arquivo com o nome "apae_sifilis.txt". Este é o arquivo de texto resultado do processsamento do programa;  








