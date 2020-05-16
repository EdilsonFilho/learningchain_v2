# learningchain_v2
READ ME

Esse repositório foi criado especialmente para guardar trabalhos relacionados ao meu projeto de pós-graduação.
Logo esse repositório é para fins educacionais. 
Observe que ele possui _v2, pois tive a alegria de ler um artigo em https://devpost.com/software/learningchain sobre esse tema e encontrei em https://github.com/HVYVince/LearningChain um projeto bem interessante.
_v2 pois baixei para fins de estudo, criando modificacoes experimentais, versionando nesse repositorio a evolucao desse estudo. Uma vez obtendo resultado satisfatorios, notificarei o repositorio de HVYVince, onde originalmente elaborou esse projeto. 

LearningChain é inspirado no paper X. Chen, J. Ji, C. Luo, W. Liao and P. Li, "When Machine Learning Meets Blockchain: A Decentralized, Privacy-preserving and Secure Design," 2018 IEEE International Conference on Big Data (Big Data), Seattle, WA, USA, 2018, pp. 1178-1187, doi: 10.1109/BigData.2018.8622598

O LearningChain surge com uma alternativa que combina o blockchain com um sistema de preservação da privacidade e segurança, considerando um modelo de aprendizagem (linear ou não) e sem um servidor central confiável.

PARA RODAR ESSE PROJETO

REQUISITOS
-Python
autopep8==1.4.4
certifi==2019.9.11
chardet==3.0.4
Click==7.0
docker==4.1.0
Flask==1.1.1
idna==2.8
itsdangerous==1.1.0
Jinja2==2.10.3
MarkupSafe==1.1.1
psutil==5.6.6
pycodestyle==2.5.0
requests==2.22.0
six==1.13.0
urllib3==1.25.7
websocket-client==0.56.0
Werkzeug==0.16.0
(em cada pasta tem um arquivo de requisitos)

Então, aqui está exatamente o que acontece quando você deseja usar nosso serviço. (https://devpost.com/software/learningchain)

1-Você faz o download do nosso cliente e o executa. Ele irá gerar um par de chaves ECC que se identificará exclusivamente no gráfico
2- Você configura o cliente para executar apenas os trabalhos nos quais tem interesse : data de validade suficientemente longa, recompensa alta o suficiente e deixá-lo funcionar até que você obtenha créditos suficientes.
3- Você cria um contêiner de docker com tudo o que seu modelo precisa para seu treinamento. Você o hospeda no host de contêineres de sua escolha .
4- Você cria o trabalho com a recompensa que está pronta para pagar pela conclusão. Quanto maior a recompensa , mais o 5- gráfico está interessado em seu trabalho e mais rápido o resultado chega !
5- Seu trabalho é propagado no gráfico e a recompensa é retirada do seu saldo.
6- Assim que um nó encontra uma solução , ele a propaga para a rede, anunciando a perda calculada.
7- Qualquer pessoa ainda pode tentar superar a perda anunciada até a data de vencimento do seu trabalho.
8- Quando seu trabalho expira, o nó que deu a melhor perda ganha a recompensa. As notícias são propagadas no gráfico. Se mais de um nó tiver exatamente a mesma perda, o mais rápido vence .
9- O vencedor propaga o modelo computado no gráfico.
10- Cada nó pode verificar se o vencedor mentiu sobre a perda anunciada, tentando o modelo proposto. Se um nó suficiente considerar o vencedor um trapaceiro, ele será banido do gráfico e seus créditos serão perdidos. Se for esse o caso, sua recompensa será devolvida a você 


Boa sorte!










