### FRANCISCO JAIME DA SILVA


# Digital Innovation One

Código criado para utilização junto a plataforma da Digital Innovation One

<p align="center"><img src="./DIO.png" width="500"></p>

## Desafio AWS EMR


__*Foi Criando um projeto de processamento utilizando pyspark no EMR da AWS*__

O desafio consistia em efetuar um processamento de dados utilizando o produto EMR da AWS. Esse processamento deveira efetuar a contagem das palavras de um livro e informar quantas vezes cada palavra aparecia no mesmo.

---

### Etapas do Desafio
# DIO-LiveCoding-AWS-BigData
Repositório de cógido do Dio Live Coding com AWS EMR e Python
Neste repositório há os arquivos de configuração e execução de análise de dados.

## Instruções

* Acessamos S3: https://s3.console.aws.amazon.com/s3/ 
  * Criar estrutura de data lake : _dio-live-datalake_
  * Criar estrutura de pastas:
    * _data_
    * _output_
    * _temp_
* Acessamos EMR: https://console.aws.amazon.com/elasticmapreduce/
    * O cluster foi criado pelo MrJob e não pelo console
    * Infraestrutura como código 
* foi criada uma chave SSH
    * Acessar  Console do EC2: https://console.aws.amazon.com/ec2/ -> Key Pairs -> Create Key Pair	
    * Download .pem file
* foi utilizada um Id e chave secreta AWS para configurar MrJob
   * Profile
   * My Security Credentials: https://console.aws.amazon.com/iam/home?region={region}#/security_credentials
   * Access Keys - Create new access key
   * Fazer download - única chance de visualizar
* Ambiente linux
   * foi criado um ambiente virtual python: _virtualenv --python=python3.6 venv_diolive_
   * Acessar com o vs code
* Foi utiliado o Notepad++ para editar os códigos
   *  code .
* foi utilizado 0s algoritimos abaixo:
   * dio-live-wordcount-test.py
   * map-reduce-count : contar
   * Instalar boto3: _pip install boto3_
   * Instalar mrjob: _pip install mrjob_
* Foi acesso o S3 i feito uploda dos arquivos
   
* Foi ativado o o ambiente virtual python: source venv_diolive/bin/activate
  * _nano ~/.mrjob.conf_
  * _python3 dio-live-wordcount-test.py -r emr s3://diobkt/data/SherlockHolmes.txt --output-dir=s3://diobkt/output/logs1 --cloud-tmp-dir=s3://diobkt/temp/_



