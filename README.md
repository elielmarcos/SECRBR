# Sinais Elétricos de Cargas Residenciais - Brasil (SECRBR) Dataset

Conjunto de dados público com registro de cargas em uma residência do Brasil para pesquisadores NILM.



# Informações do conjunto de dados

- sinais elétricos de um apartamento de 45m² (sala, cozinha, banheiro e 2 quartos) de Criciúma/Santa Catarina - Brasil
- 31 dias de gravação (2022/07/05 até 2022/08/05)
- 5 leituras de aparelhos individuais a 60Hz
- leituras agregadas da rede elétrica do apartamento a 60Hz
- dados armazenados em formato .csv
- leituras de tensão, corrente, potência ativa, reativa e aparente disponíveis com registro de timestamp



## Download

Para baixar os dados acesse o repositório com a senha: *GetSECRBR*

Você pode baixar o conjunto de dados completo (~40 GB) usando o endereço:
```bash
LINK
```



## Eletrodomésticos

| Contagem | Aparelho | Medidor |
|----------|------------------------|------------:|
| - | Lâmpadas com reator | sm01 |
| - | Lâmpadas resistivas | sm01 |
| - | Lâmpadas de LED | sm01 |
| 1 | Refrigerador | pm01 |
| 1 | Chaleira | pm03 |
| 1 | Torradeira | sm01 |
| 1 | Forno | sm01 |
| 1 | Micro-ondas | sm01 |
| 1 | Batedeira | sm01 |
| 1 | Ferro de passar | sm01 |
| 1 | Aspirador de pó | pm04 |
| 1 | Máquina de lavar roupa | sm01 |
| 1 | Secador de cabelo | pm05 |
| 1 | Chuveiro | sm01 |
| 1 | Televisor #1 | pm02 |
| 1 | Televisor #2 | sm01 |
| 1 | Notebook | sm01 |
| 1 | Roteador | sm01 |
| 2 | Carregador de Smartphone | sm01 |



## Extrutura do conjunto de dados

> **SECRBR** ══╗\
>          ║\
>          ╠═> **pm01** ══╦═> 2022_07_05\
>          ║          ░      ...\
>          ║          ╚═> 2022_08_05\
>          ║\
>          ╠═> **pm02** ══╦═> 2022_07_05\
>          ║          ░      ...\
>          ║          ╚═> 2022_08_05\
>          ║\
>          ╠═> **pm03** ══╦═> 2022_07_05\
>          ║          ░      ...\
>          ║          ╚═> 2022_08_05\
>          ║\
>          ╠═> **pm04** ══╦═> 2022_07_05\
>          ║          ░      ...\
>          ║          ╚═> 2022_08_05\
>          ║\
>          ╠═> **pm05** ══╦═> 2022_07_06\
>          ║          ░      ...\
>          ║          ╚═> 2022_08_05\
>          ║\
>          ╚═> **sm01** ══╦═> 2022_07_06\
>                     ░      ...\
>                     ╚═> 2022_08_05
>
>			
> **sm01**: Smartmeter01 Leituras agregadas\
> **pm01**: Powermeter01 Leituras individuais do Refrigerador\
> **pm02**: Powermeter02 Leituras individuais do Televisor #1\
> **pm03**: Powermeter03 Leituras individuais do Chaleira\
> **pm04**: Powermeter04 Leituras individuais do Aspirador de pó\
> **pm04**: Powermeter05 Leituras individuais do Secador de cabelo\



## Header dos arquivos

|TIMESTAMP|TENSÃO (V)|CORRENTE (A)|POTÊNCIA ATIVA (W)|POTÊNCIA REATIVA (VAR)|POTÊNCIA APARENTE (VA)|
|-----------|------------|--------------|--------------------|------------------------|------------------------:|
	

## Problemas conhecidos

Os dados do Smartmeter estão com vários intervalos sem registro 
(achamos que foi ocasionado por falhas de comunicação, pois era o medidor com maior distância entre o roteador)


