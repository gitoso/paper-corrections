# Correções no Artigo

## Outros
- Modifiquei as referências bibliográficas para a língua inglesa:
    - Publicado em -> Published on
    - Acessado em -> Accessed on

---
## Revisor 1

- [x] ~~Ainda que o trabalho apresentado faça parte de um contexto maior, o artigo não deixa claro para quem serve a identificação dos binários e para que propósito ela será efetuada. Os fabricantes (supostamente) sabem o que está contido nos seus equipamentos, então não parece que teriam necessidade dessa identificação. Seriam provedores de banda larga que desejam descobrir equipamentos vulneráveis em poder de seus usuários? Equipes corporativas de TI tentando preservar a segurança da rede conhecendo o ambiente dos usuários remotos? Os próprios usuários remotos? Atacantes tentando identificar alvos potenciais? Além disso, para que se pretende usar o resultado?~~

- [x] ~~Em suma, definir claramente o que se pretende resolver com a pesquisa é de grande importância para justificar escolhas de projeto e saber se os objetivos foram ou não atingidos.~~

    - **Linha 59:** _With this work. we aim to prevent future network router attacks by assuming the attacker position in enumerating the most common resources and vulnerabilities found in network devices firmware images. Our intention is to analyse if from the large amount of firmware images available from open sources (vendors' sites), it could be possible to extract enough knowledge so that a large scale attack could be performed. If that is the case, vendors could be warned so they can patch their devices._ 

---
## Revisor 2
- [ ] O trabalho é um trabalho em andamento. Embora isso não seja um problema, já que o workshop aceita trabalhos em andamento, ele devia ter sido submetido na categoria de pôsteres que é a categoria voltada para trabalhos em andamento.
    - **Na verdade esse item acho que não temos mais o que fazer nesse caso...**
- [x] ~~Senti falta de algum resultado mais relacionado diretamente a segurança. Por exemplo, as tabelas 2, 3 e 4 poderiam ser ampliadas com apresentação da quantidade de vulnerabilidades conhecidas para aquelas arquiteturas e kernels.~~
    - Adicionei à tabela 3 o número de CVEs para cada versão de Kernel (extraído do cvedetails.com). Para as tabelas 2 e 4 não consegui achar fontes para os números de vulnerabilidades.

- [x] ~~pg. 2: "maybe" -> "may be"~~

- [x] ~~Sugiro colocar no artigo as datas de último acesso das URLs apresentadas nas notas de rodapé (Se todas foram acessadas na mesma data, para evitar excesso de informação, seria suficiente colocar na primeira nota de rodapé que aquela URL, assim como todas as outras, foi acessada em tal data).~~

- [x] ~~pg. 3: "validation our proposal" -> "validation of our proposal"~~

- [x] ~~pg. 4: "not require the actual hardware" -> "not requiring the actual hardware"~~

- [x] ~~O label das figuras e das tabelas está em português (Figura ao invés de Figure e Tabela ao invés de Table).~~

- [x] ~~Como o foco deste artigo é na parte de re-hosting, eu destacaria esse bloco de alguma forma na Figura 1.~~

- [x] ~~Quando o Firmadyne é apresentado na página 4 não é falado nada sobre o o scraper dele. Na página 5 entretanto está escrito que o scraper do Firmadyne será usado como base. Nesse caso me parece ser algo que deveria ter sido previamente discutido na seção de trabalhos relacionados quando o Firmadyne foi apresentado.~~
    - **Linha 91:** _This approach allows firmware emulation to be done at scale, with the counterpart that the kernel replacement sacrifices emulation fidelity. The authors of {\tt Firmadyne} also implemented a web scraper capable of downloading firmware binary from popular vendors website and then used {\tt Firmadyne} to emulate and perform security analysis on the downloaded firmware images._

- [x] ~~pg. 6: "Finally, The" -> "Finally, the"~~

- [x] ~~Da forma como a Seção 3 é apresentada, subentende-se que estão sendo considerados firmwares baseados em Linux, mas isso não fica claro, nem na Seção 4. Isso deveria ser antecipado/explicado já no início da Seção 3.~~
    - **Linha 102:** _based on Linux kernel_

- [x] ~~pg. 7: "we selected five vendors" -> Qual foi o critério para selecionar esses cinco fabricantes?~~
    - **Adicionado:** _(these five vendors were selected at random, as a mean to start the research, but the final goal is to use all available vendors within the scraper)_

- [x] ~~A Figura 2 não é citada no texto.~~

## Revisor 3

- [x] ~~Não está clara a contribuição do artigo e não é feita uma comparação explícita com a ferramenta usada como base para o desenvolvimento do trabalho.~~

- [x] ~~O texto precisa ser revisado e melhorado. O objetivo do artigo não está claro no texto. No resumo, o objetivo parece ser a análise dos firmwares e uma caracterização estatística. Na introdução, o objetivo parece ser a automatização da análise de segurança. Na proposta, o objetivo parece ser a verificação de quais firmwares são mais comuns nos sites dos fabricantes. Na leitura dos resultados, é possível inferir que a proposta é melhorar a ferramenta Firmadyne, que é usada como base para desenvolver o os blocos de scraper/re-hosting mostrados na arquitetura. Os autores deveriam focar nesse ponto, caso seja essa a contribuição do artigo conforme este revisor entendeu. Assim sendo, poderiam apresentar uma análise comparativa entre a proposta e a ferramenta Firmadyne, por exemplo adicionando à Figura 2 os resultados obtidos para a Firmadyne.~~
    - **Qual é o objetivo do artigo?** R: Reunir informações, de modo a auxiliar o processo de re-hosting (no futuro) com o objetivo de analisar a viabilidade de um ataque cibernético à dispositivos de roteadores de rede;
    - Modificações realizadas:
        - [Resumo](./Resumo.md)
        - [Introdução](./Introduction.md)
        - [Rehosting Process](./RehostingProcess.md)
        - [Resultados](./Resultados.md)
        - [Conclusão](./Conclusao.md)
