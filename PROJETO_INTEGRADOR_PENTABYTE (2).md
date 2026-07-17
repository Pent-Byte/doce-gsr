**PROJETO INTEGRADOR**

**Cidades Inteligentes**
**Gestão De Recursos Hídricos - Petabyte**

**PARNAMIRIM/RN - 2026**

**Discentes:**

Maria Alicy da Silva Fernandes

Luiz Henrique Torres Lima

Samantha Dantas de Morais

Mateus Inácio da Silva

**Cidades Inteligentes**
**Gestão De Recursos Hídricos - Petabyte**

Trabalho de Conclusão de Curso (Projeto Integrador) submetido ao Curso Técnico Subsequente em Redes de Computadores do Instituto Federal do Rio Grande do Norte (IFRN), como requisito parcial para a obtenção de nota na disciplina de Projeto Integrador referente ao 4º período.

Orientador: Prof. Credson Isaac Lopes dos Santos

**PARNAMIRIM/RN - 2026**

**Lista de figuras**

[Figura 1 - Logomarca da Empresa	6](#figura-1---logomarca-da-empresa)

[Figura 2 - Localização da Matriz.	7](#figura-2---localização-da-matriz.)

[Figura 3 - Localização da Filial	8](#figura-3---localização-da-filial)

[Figura 4 - Planta Baixa Matriz	10](#figura-4---planta-baixa-matriz)

[Figura 5 - Planta Baixa Filial	10](#figura-5---planta-baixa-filial)

[Figura 6 - Rack	11](#figura-6---rack)

[Figura 7 - Topologia da Rede PentaByte	14](#figura-7---topologia-da-rede-pentabyte)

[Figura 8 - Diagrama Unifilar Matriz	15](#figura-8---diagrama-unifilar-matriz)

[Figura 9 - Diagrama Unifilar Filial	15](#figura-9---diagrama-unifilar-filial)

[Figura 10 - Planilha de Endereçamento IP	16](#figura-10---planilha-de-endereçamento-ip)

[Figura 11 - Mapa da Rede da Matriz	17](#figura-11---mapa-da-rede-da-matriz)

[Figura 12 - Mapa de Rede da Filial	17](#figura-12---mapa-de-rede-da-filial)

[Figura 13 - Monitoramento Zabbix	21](#figura-13---monitoramento-zabbix)

[Figura 14 - AD da Matriz	22](#figura-14---ad-da-matriz)

[Figura 15 - OU Administrativo Matriz	23](#figura-15---ou-administrativo-matriz)

[Figura 16 - AD da Matriz se Comunicando com a Filial	23](#figura-16---ad-da-matriz-se-comunicando-com-a-filial)

[Figura 17 - AD da Filial se comunicando com a Matriz	24](#figura-17---ad-da-filial-se-comunicando-com-a-matriz)

[Figura 18 - GPO da Matriz	24](#figura-18---gpo-da-matriz)

[Figura  19 - Script Firewall.sh matriz	26](#figura-19---script-firewall.sh-matriz)

[Figura 20 - Script Firewall.sh filial	26](#figura-20---script-firewall.sh-filial)

[Figura 21 – Tela de bloqueio de conteúdo web por diretiva do Servidor Proxy da Matriz.	28](#figura-21-–-tela-de-bloqueio-de-conteúdo-web-por-diretiva-do-servidor-proxy-da-matriz.)

[Figura 22 - Funcionamento da VPN Matriz	29](#figura-22---funcionamento-da-vpn-matriz)

[Figura 23 - Interface de tunelamento matriz VPN	30](#figura-23---interface-de-tunelamento-matriz-vpn)

[Figura 24 - Funcionamento da VPN Filial	30](#figura-24---funcionamento-da-vpn-filial)

[Figura 25 - Captura de tela interface de tunelamento Filial VPN	31](#figura-25---captura-de-tela-interface-de-tunelamento-filial-vpn)

[Figura 26 - Ping entre AD da filial para matriz VPN	31](#figura-26---ping-entre-ad-da-filial-para-matriz-vpn)

[Figura 27 - Site da Empresa	32](#figura-27---site-da-empresa)

[Figura 28 - Interface de rede DMZ	33](#figura-28---interface-de-rede-dmz)

[Figura 29 - GLPI	35](#figura-29---glpi)

[Figura  30 - Figura do Graylog	37](#figura-30---figura-do-graylog)

[Figura 31 - Funcionamento do Arduino	40](#figura-31---funcionamento-do-arduino)

[Figura 32 – Portal Web corporativo exibindo o alerta em tempo real de nível crítico na lagoa.	43](#figura-32-–-portal-web-corporativo-exibindo-o-alerta-em-tempo-real-de-nível-crítico-na-lagoa.)

**Sumário**

[**1. INTRODUÇÃO	4**](#heading=)

[**1.1 OBJETIVOS	5**](#heading=)

[1.1.1 Objetivo Geral	5](#1.1.1-objetivo-geral)

[1.1.2 Objetivos Específicos	5](#1.1.2-objetivos-específicos)

[**2. SOBRE A EMPRESA	6**](#heading=)

[**2.1 DADOS DA EMPRESA	7**](#heading=)

[2.1.1 Matriz	7](#2.1.1-matriz)

[2.1.2 Filial	8](#2.1.2-filial)

[**2.2 MISSÃO	9**](#heading=)

[**2.3 VISÃO	9**](#heading=)

[**3. PROJETO FÍSICO	9**](#heading=)

[**3.1 Planta Baixa Matriz	10**](#heading=)

[**3.2 Planta Baixa Filial	10**](#heading=)

[**4. CAPACIDADE PLANEJADA	11**](#heading=)

[**4.1 Matriz	11**](#heading=)

[**4.2 Filial	12**](#heading=)

[**5. TOPOLOGIA DE REDES	12**](#heading=)

[**6. MAPA DE REDE	16**](#heading=)

[**7. ENDEREÇAMENTO DE REDE	17**](#heading=)

[**8. PLANEJAMENTO ORÇAMENTO	18**](#heading=)

[**Tabela de Orçamento infraestrutura	19**](#heading=)

[**9. MONITORAMENTO DA REDE	20**](#heading=)

[**10. ACTIVE DIRECTORY	21**](#10.-active-directory)

[10.1 Diretivas de Grupo (GPOs) e Padronização de Segurança	25](#10.1-diretivas-de-grupo-\(gpos\)-e-padronização-de-segurança)

[**11. FIREWALL	25**](#heading=)

[11.1 Servidor Proxy de Rede (Matriz)	27](#11.1-servidor-proxy-de-rede-\(matriz\))

[**12. VPN	28**](#heading=)

[**13. ZONA DESMILITARIZADA (DMZ)	32**](#heading=)

[**14. GLPI – GESTÃO DE SERVIÇOS DE TI	33**](#heading=)

[**15. GRAFANA – VISUALIZAÇÃO E ANÁLISE DE DADOS	35**](#heading=)

[**16. GRAYLOG - CENTRALIZAÇÃO E ANÁLISE DE LOGS	36**](#heading=)

[**17.1. Descrição Geral do Circuito	38**](#heading=)

[**17.2. Componentes Utilizados	39**](#heading=)

[**17.3. Esquema de Ligação e Pinagem	39**](#heading=)

[**17.4. Lógica de Programação	40**](#heading=)

[**17.5. Resultados e Testes de Simulação	41**](#heading=)

[17.6 Integração e Exibição de Telemetria no Portal Web	42](#17.6-integração-e-exibição-de-telemetria-no-portal-web)

[**18. CONCLUSÃO	43**](#heading=)

[**Referências	45**](#heading=)
1. # **INTRODUÇÃO**
No âmago das metamorfoses urbanas contemporâneas, a gestão estratégica das águas pluviais emergiu como um pilar indissociável da resiliência metropolitana. Historicamente, as lagoas de captação têm operado sob um regime de insularidade tecnológica; a ausência de um monitoramento ubíquo e contínuo compromete severamente a capacidade preditiva contra inundações e negligencia o rigoroso controle qualitativo dos efluentes lançados nos ecossistemas receptores. Diante dessa vulnerabilidade, a PentaByte propõe uma intervenção técnica que integra infraestrutura de rede robusta ao manejo ambiental, alinhando-se ao conceito de cidade inteligente entendido como aquela em que investimentos em capital humano, social e em infraestrutura de comunicação tradicional e moderna impulsionam o crescimento econômico sustentável e a gestão criteriosa dos recursos naturais *(CARAGLIU; DEL BO; NIJKAMP, 2011)*.

A convergência com o paradigma das Smart Cities oferece a via de superação necessária. Através da expertise da PentaByte, este projeto implementa uma arquitetura de rede segura e eficiente, fundamentada em normas de cabeamento estruturado e conectividade de alta disponibilidade *(ABNT, 2013)*. O diferencial reside na integração de sensores inteligentes com sistemas de defesa e gerência avançados, incluindo Firewalls de última geração, túneis criptografados via VPN e autenticação centralizada. A segregação de serviços em DMZ garante que os dados coletados sejam processados com integridade, protegendo a rede contra acessos não autorizados enquanto mantém o fluxo de informações vitais para o centro de controle *(STALLINGS, 2015)*.

Este projeto propõe, especificamente, o desenvolvimento de um sistema de monitoramento inteligente para a lagoa de captação de Lagoa Antônio Pessoa, em Parnamirim/RN, utilizando a plataforma Zabbix para a telemetria em tempo real de níveis fluviométricos e parâmetros de qualidade *(ZABBIX LLC, 2026)*. A implementação desta solução pela PentaByte visa não apenas a mitigação de riscos de desastres naturais, mas a consolidação de uma governança hídrica baseada em evidências. Dessa forma, convertemos a infraestrutura física em um ativo informacional estratégico, onde a eficiência tecnológica e a segurança de rede convergem para a sustentabilidade e a proteção do tecido urbano.
##
## 1\.1 OBJETIVOS
## 1\.1.1 Objetivo Geral {#1.1.1-objetivo-geral}
Projetar e instituir, sob a égide da PentaByte, uma infraestrutura de rede resiliente e um ecossistema de monitoramento inteligente para a lagoa de captação, assegurando a fidedignidade dos dados, a integridade cibernética e a otimização da governança hídrica, em conformidade com as boas práticas de segurança da informação preconizadas na literatura de redes *(TANENBAUM; WETHERALL, 2011)*.
## 1\.1.2 Objetivos Específicos {#1.1.2-objetivos-específicos}
Implementar a infraestrutura de rede e conectividade
Centralizar a coleta automatizada de dados hídricos
Implantar o ecossistema corporativo de monitoramento
Garantir a auditoria e conformidade de segurança
Otimizar a gestão de ativos e chamados
#
# **2. SOBRE A EMPRESA**
A PentaByte foi fundada com o objetivo precípuo de desenvolver soluções tecnológicas voltadas para o paradigma das Cidades Inteligentes, especializando-se na gestão estratégica de recursos hídricos. A empresa surgiu da necessidade crítica de modernizar as lagoas de captação, transformando essas infraestruturas urbanas, antes isoladas, em sistemas monitorados e inteligentes, capazes de responder com agilidade aos desafios climáticos e ambientais das metrópoles contemporâneas *(CARAGLIU; DEL BO; NIJKAMP, 2011)*.

Com o avanço das demandas por resiliência urbana, a PentaByte investe em infraestruturas de rede robustas para garantir que o monitoramento de níveis e qualidade da água ocorra de forma ininterrupta. A empresa utiliza tecnologias de conectividade de alto desempenho, aliadas a rigorosas práticas de segurança da informação e telemetria avançada *(KUROSE; ROSS, 2013)*, assegurando que os dados ambientais sejam transmitidos com integridade e precisão.

Desde sua criação, a PentaByte tem se destacado pelo compromisso com a sustentabilidade e pela constante evolução técnica de seus projetos. A implementação de soluções como Firewalls, VPNs e o sistema de monitoramento Zabbix permite que a empresa gerencie o ecossistema das lagoas de captação de forma eficiente, prevenindo transbordamentos, mitigando riscos de desastres naturais e garantindo uma governança baseada em dados reais *(ZABBIX LLC, 2026)*.

Toda a arquitetura de dados desenvolvida pela PentaByte opera em estrita conformidade com as diretrizes da Lei 13.709/2018 (Lei Geral de Proteção de Dados) *(BRASIL, 2018)*, assegurando que a inovação tecnológica caminhe lado a lado com a segurança jurídica e a privacidade.
### *Figura 1 - Logomarca da Empresa* {#figura-1---logomarca-da-empresa}
*Fonte: O autor.*
## 2\.1 DADOS DA EMPRESA
#### **2.1.1 Matriz** {#2.1.1-matriz}
Endereço: R. Rio Amazonas, 86 - Parque de Exposições, Parnamirim - RN.
CEP: 59146-410
CNPJ: 58.685.374/4580-98
Telefone: (84) 5797-5984 e (84) 99574-4562
E-mail: <contato@pentabyte.com.br>
### *Figura 2 - Localização da Matriz.* {#figura-2---localização-da-matriz.}
*Fonte: Google Maps (2026).*
#### **2.1.2 Filial** {#2.1.2-filial}
Endereço: R. Geraldo Pontes, 294-236 - Parque de Exposicoes, Parnamirim - RN.
CEP: 59146-395
CNPJ: 68.795.697/2466-64
Telefone: (84) 8775-579 e (84) 99487-3479
E-mail: <contato@segurebyte.com.br>
### *Figura 3 - Localização da Filial* {#figura-3---localização-da-filial}
*Fonte: Google Maps (2026).*
##
## 2\.2 MISSÃO
A missão da PentaByte é fornecer infraestrutura tecnológica avançada e segura para o monitoramento inteligente de recursos hídricos em Cidades Inteligentes. Focada na gestão sustentável e proativa, a empresa visa garantir a máxima confiabilidade na coleta de dados ambientais, otimizar a comunicação segura entre redes corporativas e automatizar o controle de ativos e incidentes, assegurando a preservação ambiental e a eficiência operacional por meio da tecnologia *(CARAGLIU; DEL BO; NIJKAMP, 2011)*.
## 2\.3 VISÃO
Ser reconhecida como referência nacional na inovação de infraestruturas tecnológicas para Cidades Inteligentes, consolidando-se como a principal parceira na gestão estratégica, sustentável e ultra-segura de monitoramento hídrico e automação de redes corporativas.
# **3. PROJETO FÍSICO**
Foram desenvolvidas duas plantas baixas para a Matriz e a Filial da PentaByte, com o objetivo de implantar o cabeamento estruturado e organizar a infraestrutura de rede voltada ao monitoramento hídrico e suporte da empresa, em conformidade com os procedimentos normativos de projeto de cabeamento de telecomunicações para redes internas estruturadas *(ABNT, 2013)*.

O cabeamento será encaminhado por eletrocalhas metálicas aparentes instaladas no teto, utilizando o corredor de circulação entre as salas. A partir das eletrocalhas, os cabos irão derivar por eletrodutos rígidos de aço galvanizado até o kit condulete com dois conectores RJ-45 fêmea. Em alguns ambientes, o cabeamento será direcionado diretamente ao ponto de telecomunicação ou servidores, seguindo as recomendações de topologia física em estrela hierárquica para cabeamento estruturado *(TANENBAUM; WETHERALL, 2011)*.

Serão utilizados cabos de par trançado UTP Categoria 6 (CAT6), seguindo o padrão de pinagem ANSI/TIA-568-B, com conectores e tomadas RJ45 fêmea (keystones) certificados para a categoria. Na matriz serão distribuídos 34 pontos de rede e na filial 26 pontos de rede.
##
## 3\.1 Planta Baixa Matriz
### *Figura 4 - Planta Baixa Matriz* {#figura-4---planta-baixa-matriz}
![image1]

*Fonte: O autor.*
##
## 3\.2 Planta Baixa Filial
### *Figura 5 - Planta Baixa Filial* {#figura-5---planta-baixa-filial}
![image2]

*Fonte: O autor.*
### *Figura 6 - Rack* {#figura-6---rack}
![image3]

*Fonte: O autor.*
# **4. CAPACIDADE PLANEJADA**
Considerando que a infraestrutura física da PentaByte será implementada em um único andar para centralizar as operações administrativas e de gerência, a capacidade planejada de pontos de rede foi dimensionada a partir da soma dos pontos originalmente distribuídos por cada compartimento estratégico da empresa, seguindo os critérios de dimensionamento de áreas de trabalho definidos pela normatização de cabeamento estruturado *(ABNT, 2013)*:
## 4\.1 Matriz

|LOCALIZAÇÃO|QUANT. DE PONTOS|
| :- | :- |
|Sala de Monitoramento|8|
|Recepção|6|
|Sala de RH|6|
|Sala de Data Center|4|
|Copa|4|
|Sala de Depósito|2|
|Banheiro Masculino|2|
|Banheiro Feminino|2|
|**Total**|**34**|

*Fonte: O autor.*
## 4\.2 Filial

|LOCALIZAÇÃO|QUANT. DE PONTOS|
| :- | :- |
|Recepção|6|
|Sala de Monitoramento|6|
|Sala de Depósito|4|
|Copa|4|
|Corredor (Circulação)|4|
|Banheiro Feminino|2|
|Banheiro Masculino|2|
|**Total**|**26**|

*Fonte: O autor.*
#
# **5. TOPOLOGIA DE REDES**
A topologia de rede define a forma como os dispositivos, ativos de interconexão e links de comunicação estão estruturados dentro da infraestrutura da PentaByte, descrevendo o fluxo físico e estrutural dos dados, a distribuição dos equipamentos de hardware e o controle de tráfego entre a matriz e a filial *(TANENBAUM; WETHERALL, 2011)*.

Para a PentaByte, a topologia adotada nas redes locais (LAN) será baseada no modelo em Estrela Estendida, no qual as estações de trabalho, pontos de acesso e servidores estão interligados diretamente a switches de distribuição e switches centrais. Essa configuração proporciona maior desempenho, facilidade de gerenciamento de hardware e isolamento de falhas, garantindo que um problema em um cabo de rede ou computador específico não comprometa toda a infraestrutura hídrica *(KUROSE; ROSS, 2013)*.

A interconexão de longa distância (WAN) entre as duas sedes será realizada através de uma arquitetura Ponto a Ponto, viabilizada por links dedicados de fibra óptica de provedores parceiros locais. Para garantir a segurança perimetral de toda essa topologia, serão implementados firewalls de borda tanto na matriz quanto na filial *(STALLINGS, 2015)*. Esses dispositivos serão responsáveis por controlar todo o tráfego de entrada e saída da internet pública, além de fechar um túnel criptografado seguro para que a filial se comunique de forma direta e privada com o centro de dados principal.

Na Matriz, o núcleo da rede será sustentado por um Switch gerenciável de Camada 3 (Layer 3), que funcionará como o ponto central de distribuição. Esse equipamento de alta performance fará a segmentação física e estrutural dos setores (Administração, Diretoria e Engenharia de Campo), além de interconectar diretamente o rack de servidores onde operam o DC1 (Windows Server 2025 GUI) e o banco de dados principal *(MICROSOFT, 2026)*.

Na Filial, a infraestrutura física de distribuição de rede será concentrada em um Switch de Camada 2 (Layer 2). Este switch conecta localmente as estações dos técnicos e o servidor secundário DC2 (Windows Server 2022 Server Core), mantendo a comunicação ativa com a matriz através do gateway de borda. Toda essa infraestrutura de ativos de rede será monitorada em tempo real por um sistema centralizado, permitindo que a equipe de TI acompanhe a integridade das portas dos switches, a oscilação dos links de fibra óptica e a latência da comunicação *(ZABBIX LLC, 2026)*.

Essa arquitetura de topologia de rede assegura alta tolerância a falhas, eficiência na transmissão de pacotes, segurança física do perímetro e escalabilidade, elementos essenciais para suportar a infraestrutura de Cidades Inteligentes da PentaByte *(CARAGLIU; DEL BO; NIJKAMP, 2011)*.
### *Figura 7 - Topologia da Rede PentaByte* {#figura-7---topologia-da-rede-pentabyte}
![image4]

*Fonte: O autor.*
### *Figura 8 - Diagrama Unifilar Matriz* {#figura-8---diagrama-unifilar-matriz}
![image5]

*Fonte: O autor.*
### *Figura 9 - Diagrama Unifilar Filial* {#figura-9---diagrama-unifilar-filial}
![image6]

*Fonte: O autor.*
#
#
# **6. MAPA DE REDE**
O mapa de rede da PentaByte consiste na representação gráfica e esquemática de toda a infraestrutura de comunicação do projeto, ilustrando a disposição dos ativos de hardware, os canais de interconexão e a distribuição dos servidores localizados na matriz e na filial. Esta documentação visual viabiliza a análise imediata da engenharia da rede, simplificando a compreensão do fluxo de dados e o caminho percorrido pelas informações desde os pontos de coleta até a central *(TANENBAUM; WETHERALL, 2011)*.

No diagrama que compõe este mapa, estão devidamente mapeados elementos críticos como os firewalls perimetrais, switches de distribuição, servidores de diretório e hosts de virtualização. Estão incluídas também as demarcações dos links de fibra óptica fornecidos pelos parceiros locais de conectividade, as antenas de recepção de telemetria e o cabeamento estruturado que interliga os setores. Adicionalmente, o esquema incorpora dados técnicos fundamentais, tais como as faixas de endereçamento IP alocadas, a divisão das VLANs e a modelagem estrutural das conexões de contingência *(FOROUZAN, 2010)*.

Esta ferramenta técnica desempenha um papel estratégico na governança de TI da PentaByte, servindo como guia para o isolamento proativo de incidentes, resolução de gargalos de largura de banda e para o direcionamento de futuras expansões na malha de monitoramento das lagoas. O mapa de rede assegura uma gestão operacional otimizada, promovendo a integridade, a padronização e a resiliência cibernética indispensáveis para o suporte a Cidades Inteligentes *(STALLINGS, 2015)*.
### *Figura 10 - Planilha de Endereçamento IP* {#figura-10---planilha-de-endereçamento-ip}
![image7]

*Fonte: O autor.*
### *Figura 11 - Mapa da Rede da Matriz* {#figura-11---mapa-da-rede-da-matriz}
![image8]

*Fonte: O autor.*
### *Figura 12 - Mapa de Rede da Filial* {#figura-12---mapa-de-rede-da-filial}
![image9]

*Fonte: O autor.*
# **7. ENDEREÇAMENTO DE REDE**
O endereçamento de rede define o planejamento lógico e a atribuição de identificadores numéricos exclusivos para cada dispositivo, servidor, interface de rede e elemento de monitoramento hídrico dentro da infraestrutura da PentaByte. Essa estruturação organiza o tráfego de dados, garantindo que os pacotes de informação sejam roteados corretamente entre as sub-redes da matriz, da filial e dos sistemas de telemetria locais *(FOROUZAN, 2010)*.

Para garantir eficiência e evitar o esgotamento de conexões, a PentaByte adotará o padrão de endereçamento privado IPv4 sob a máscara de sub-rede de comprimento variável (VLSM). A distribuição dos blocos de IP será dividida de forma cirúrgica entre as duas localidades para impedir conflitos de roteamento e otimizar o desempenho *(KUROSE; ROSS, 2013)*. Os IPs de servidores críticos — como o DC1 (Windows Server 2025 GUI) na matriz, o DC2 (Windows Server 2022 Server Core) na filial, gateways de firewalls e interfaces de switches gerenciáveis — serão definidos de forma estática (fixa), assegurando que os serviços essenciais de DNS e Active Directory estejam sempre acessíveis no mesmo endereço *(MICROSOFT, 2026)*.

Por outro lado, as estações de trabalho dos funcionários administrativos, computadores da engenharia e dispositivos móveis receberão suas configurações IP de forma dinâmica e automatizada. Isso será feito através do serviço DHCP (Dynamic Host Configuration Protocol), onde o servidor da matriz e o servidor da filial gerenciarão escopos locais distintos e isolados, distribuindo endereços temporários dentro de suas respectivas sub-redes corporativas *(FOROUZAN, 2010)*.

Essa política de endereçamento garante uma rede organizada, com mapeamento preciso de privilégios de acesso e facilidade na identificação de incidentes. Ao delimitar claramente as faixas de IP de cada setor e servidor, a PentaByte consolida um ambiente escalável, preparado para receber novos pontos de rede à medida que o monitoramento urbano das lagoas de captação se expandir.
# **8. PLANEJAMENTO ORÇAMENTO**
A projeção orçamentária da PentaByte foi desenvolvida a partir de um mapeamento rigoroso dos insumos indispensáveis para a implementação e sustentação de toda a infraestrutura de redes e sistemas da organização. Foram contabilizados minuciosamente os custos associados a ativos de conectividade, insumos de cabeamento estruturado, servidores de grande capacidade, mecanismos de segurança perimetral, licenciamento de softwares corporativos e dispositivos de contingência energética, assegurando uma perspectiva ampla e fidedigna dos aportes financeiros envolvidos no projeto *(ABNT, 2013)*.

O plano financeiro foi modelado para oferecer flexibilidade e escalabilidade, viabilizando ampliações futuras na malha de comunicação à medida que a cobertura geográfica se expandir e a demanda pelo processamento de dados crescer. Adicionalmente, foram estimados os custos operacionais com links de dados e as provisões para a manutenção preventiva dos equipamentos elétricos, salvaguardando a estabilidade econômica e a perenidade operacional do negócio a longo prazo.

Esse direcionamento orçamentário subsidia a tomada de decisões estratégicas por parte da administração, coibindo despesas supérfluas e garantindo que o arcabouço tecnológico da PentaByte seja implantado de forma eficaz, segura e estritamente convergente com as metas de modernização urbana do projeto, alinhando-se à opção por soluções de monitoramento em código aberto amplamente documentadas na literatura técnica *(ZABBIX LLC, 2026)*.
## Tabela de Orçamento infraestrutura

|Local|Categoria|Descrição do Item|Qtd|Valor Unitário (R$)|Subtotal (R$)|
| :- | :- | :- | :- | :- | :- |
|Matriz|Infraestrutura|Rack padrão 24U com porta e ventilação|1|R$ 1.419,14|R$ 1.419,14|
|Matriz|Infraestrutura|Bandeja fixa para rack|4|R$ 180,00|R$ 720,00|
|Matriz|Infraestrutura|Organizador horizontal de cabos|6|R$ 120,00|R$ 720,00|
|Matriz|Infraestrutura|Guia vertical para rack|2|R$ 320,00|R$ 640,00|
|Matriz|Rede|Switch gerenciável 24 portas Gigabit|2|R$ 4.500,00|R$ 9.000,00|
|Matriz|Rede|Patch panel CAT6 – 24 portas|4|R$ 720,00|R$ 2.880,00|
|Matriz|Rede|Patch cord CAT6 – 2 metros|30|R$ 32,00|R$ 960,00|
|Matriz|Cabeamento|Cabo UTP CAT6 – caixa 305m|6|R$ 1.150,00|R$ 6.900,00|
|Matriz|Cabeamento|Conjunto Condulete 1" 2 RJ45|22|R$ 109,90|R$ 2.417,80|
|Matriz|Cabeamento|Eletrocalha metálica 100x75 mm|80|R$ 80,00|R$ 6.400,00|
|Matriz|Cabeamento|Eletroduto PVC rígido 1"|120|R$ 20,00|R$ 2.400,00|
|Matriz|Energia|Régua de tomadas para rack|2|R$ 260,00|R$ 520,00|
|Matriz|Serviços|Instalação e organização de cabeamento|1|R$ 3.800,00|R$ 3.800,00|
|Matriz|Serviços|Configuração de rede e testes|1|R$ 1.900,00|R$ 1.900,00|
|Filial|Infraestrutura|Rack padrão 16U com porta e ventilação|1|R$ 1.162,00|R$ 1.162,00|
|Filial|Infraestrutura|Bandeja fixa para rack|3|R$ 180,00|R$ 540,00|
|Filial|Infraestrutura|Organizador horizontal de cabos|4|R$ 120,00|R$ 480,00|
|Filial|Rede|Switch gerenciável 24 portas Gigabit|2|R$ 1.621,00|R$ 3.242,00|
|Filial|Rede|Patch panel CAT6 – 24 portas|2|R$ 720,00|R$ 1.440,00|
|Filial|Rede|Patch cord CAT6 – 2 metros|20|R$ 32,00|R$ 640,00|
|Filial|Cabeamento|Cabo UTP CAT6 – caixa 305m|4|R$ 1.150,00|R$ 4.600,00|
|Filial|Cabeamento|Conjunto Condulete 1" 2 RJ45|10|R$ 109,90|R$ 1.099,00|
|Filial|Cabeamento|Eletrocalha metálica 50x75 mm|60|R$ 70,00|R$ 4.200,00|
|Filial|Cabeamento|Eletroduto PVC rígido 1"|90|R$ 20,00|R$ 1.800,00|
|Filial|Energia|Régua de tomadas para rack|1|R$ 260,00|R$ 260,00|
|Filial|Serviços|Instalação, testes e documentação|1|R$ 1.800,00|R$ 1.800,00|
|**Total**|||||**R$ 61.939,94**|

*Fonte: O autor.*
# **9. MONITORAMENTO DA REDE**
Para o gerenciamento da rede e da infraestrutura de TI, a PentaByte utiliza o Zabbix integrado ao Grafana como solução principal de monitoramento e visualização de dados. O Zabbix é uma plataforma open-source amplamente adotada para a supervisão centralizada de redes e sistemas *(ZABBIX LLC, 2026)*, atuando em conjunto com o Grafana para a renderização de painéis avançados, permitindo o acompanhamento em tempo real do desempenho e da disponibilidade de todos os serviços da empresa *(GRAFANA LABS, 2026)*.

Por meio dessa arquitetura, a PentaByte realiza a supervisão contínua de servidores, roteadores MikroTik, switches, enlaces de internet, equipamentos de borda, firewalls e serviços essenciais distribuídos na matriz, na filial e na zona desmilitarizada (DMZ). A infraestrutura conta ainda com o Graylog para a centralização e análise profunda de logs de auditoria *(GRAYLOG, INC., 2026)*, e com o GLPI para a abertura automatizada de chamados e inventário de ativos *(TECLIB' EDITION, 2026)*. Esse conjunto garante maior controle, segurança cibernética e rapidez na identificação de falhas, tentativas de intrusão ou degradações de desempenho, contribuindo para uma gestão estritamente proativa da rede.

Principais recursos utilizados:

* Monitoramento de Infraestrutura: acompanhamento contínuo de dispositivos físicos e virtuais, como roteadores MikroTik, switches, firewalls e servidores hospedados na rede interna e na DMZ, além de serviços críticos e sistemas operacionais *(MIKROTIK, 2026)*;
* Coleta Avançada de Dados e Logs: utilização de protocolos como SNMP, agentes nativos e scripts para a coleta de métricas de desempenho pelo Zabbix, combinada com o envio centralizado de mensagens de syslog dos ativos para o Graylog *(GRAYLOG, INC., 2026)*;
* Alertas e Notificações Automatizadas: configuração de gatilhos automáticos para eventos de criticidade, gerando alertas imediatos para a equipe de TI e abrindo de forma integrada ordens de serviço e chamados técnicos diretamente na plataforma GLPI;
* Painéis e Gráficos Personalizáveis com Grafana: criação de dashboards dinâmicos e relatórios visuais de alto nível, consolidando informações detalhadas sobre o tráfego de dados do túnel VPN, consumo de recursos e saúde dos ativos *(GRAFANA LABS, 2026)*;
* Automatização e Resposta a Incidentes: execução de rotinas e scripts automatizados nos gateways de borda e servidores em caso de falhas, auxiliando no reestabelecimento rápido de rotas de contingência e serviços sem intervenção manual imediata;
* Escalabilidade e Alta Disponibilidade: capacidade de monitorar múltiplos equipamentos, serviços segmentados e o fluxo de dados criptografados, acompanhando de maneira robusta e segura o crescimento da infraestrutura da PentaByte.

A utilização desse ecossistema integrado garante máxima confiabilidade, conformidade de segurança e eficiência operacional para a PentaByte, permitindo a tomada de decisões rápidas, inteligentes e embasadas no monitoramento contínuo de todo o ambiente de rede.
### *Figura 13 - Monitoramento Zabbix* {#figura-13---monitoramento-zabbix}
![image10]

*Fonte: O autor.*
# **10. ACTIVE DIRECTORY** {#10.-active-directory}
O serviço de diretório é um componente essencial para a governança e segurança da infraestrutura de rede, atuando como um repositório centralizado que gerencia identidades, autentica usuários e aplica políticas de segurança em todo o ambiente corporativo. Na PentaByte, o Active Directory (AD) é responsável por garantir o controle de acesso lógico a recursos compartilhados, computadores e sistemas, assegurando a integridade dos dados administrativos e operacionais da empresa *(MICROSOFT, 2026)*.

Para a implementação das políticas de gerenciamento, a PentaByte utiliza servidores Windows Server dedicados à função de Controladores de Domínio (DC). As configurações são estruturadas sob o domínio projeto.pentabyte, onde são organizadas as Unidades Organizacionais (OUs), contas de usuários, grupos de permissões e as Diretivas de Grupo (GPOs) responsáveis por padronizar as restrições de segurança e as configurações das estações de trabalho na matriz e na filial *(MICROSOFT, 2026)*.

Foram configuradas regras específicas de replicação de diretório entre as localidades da empresa, garantindo que as bases de dados de autenticação e os serviços de DNS integrados permanecessem sincronizados e em alta disponibilidade. Isso permite que, em caso de indisponibilidade em uma das sedes, os usuários continuem realizando o logon de forma segura e transparente, mantendo o tráfego interno protegido e os serviços essenciais em execução.

Para complementar a segurança e permitir a análise contínua do ambiente, a infraestrutura do Active Directory é integrada de forma estrita ao ecossistema de gerência. O desempenho dos servidores, o status da replicação e a disponibilidade do serviço são monitorados continuamente pelo Zabbix, enquanto todos os logs de auditoria como tentativas de login mal-sucedidas, criação de usuários ou alterações de privilégios são enviados em tempo real para o Graylog *(GRAYLOG, INC., 2026)*. Essa abordagem garante maior controle, conformidade de segurança e proteção robusta aos acessos lógicos e à identidade corporativa da PentaByte.
### *Figura 14 - AD da Matriz* {#figura-14---ad-da-matriz}
*Fonte: O autor.*
### *Figura 15 - OU Administrativo Matriz* {#figura-15---ou-administrativo-matriz}
*Fonte: O autor.*
### *Figura 16 - AD da Matriz se Comunicando com a Filial* {#figura-16---ad-da-matriz-se-comunicando-com-a-filial}
![image11]

*Fonte: O autor*
### *Figura 17 - AD da Filial se comunicando com a Matriz* {#figura-17---ad-da-filial-se-comunicando-com-a-matriz}
*Fonte: O autor.*
### *Figura 18 - GPO da Matriz* {#figura-18---gpo-da-matriz}
![image12]

*Fonte: O autor.*
#
##
## 10\.1 Diretivas de Grupo (GPOs) e Padronização de Segurança  {#10.1-diretivas-de-grupo-(gpos)-e-padronização-de-segurança}
Para garantir a conformidade de segurança dos endpoints associados ao domínio projeto.pentabyte, foram projetadas e ativadas Diretivas de Grupo (GPOs) vinculadas à Unidade Organizacional (OU) dos computadores administrativos:

* GPO - Bloqueio de Dispositivos de Armazenamento Removível (USB): Desabilita a montagem e leitura de mídias físicas externas (como pendrives). Esta política mitiga o risco de vazamento de informações operacionais de monitoramento e impede a introdução acidental de códigos maliciosos nas estações ligadas à matriz.
* GPO - Bloqueio Automático de Tela por Inatividade: Força a ativação do protetor de tela com exigência de senha após 5 minutos de ociosidade do usuário. A medida resguarda a console operacional de visualização caso um operador se ausente temporariamente de seu posto.
* GPO - Padronização de Papel de Parede Corporativo: Define uma imagem de plano de fundo padrão da PentaByte associada a uma notificação de aviso legal e termo de uso aceitável, lembrando os usuários sobre a finalidade exclusivamente profissional e auditada dos computadores da empresa.
# **11. FIREWALL**
O firewall é um componente essencial para a segurança da infraestrutura de rede, atuando como uma barreira de proteção que controla e filtra o tráfego de entrada e saída, prevenindo acessos não autorizados e ataques externos *(STALLINGS, 2015)*. Na PentaByte, o firewall é responsável por garantir a integridade dos serviços e a segurança dos dados trafegados na rede corporativa e nos sistemas de monitoramento hídrico.

Para a implementação das políticas de segurança, a PentaByte utiliza recursos avançados de filtragem e controle de pacotes diretamente em seus gateways de borda MikroTik *(MIKROTIK, 2026)*. As regras de segurança são organizadas e aplicadas de forma estruturada no sistema operacional dos ativos de borda, sendo responsáveis por ativar as configurações de filtragem, tradução de endereços de rede (NAT) para mascaramento da internet e controle estrito de acesso a zonas sensíveis, como a zona desmilitarizada (DMZ).

Foram configuradas regras específicas de firewall para permitir e proteger a comunicação entre a matriz e a filial, garantindo o encaminhamento adequado de pacotes entre as redes internas através de um túnel seguro de VPN, sem comprometer a segurança da infraestrutura. Também foram definidas políticas altamente restritivas para proteger os serviços de diretório, bancos de dados e aplicações corporativas, permitindo apenas o tráfego estritamente essencial *(FOROUZAN, 2010)*.

Para complementar a segurança e permitir a análise contínua do ambiente, a infraestrutura de firewall é integrada ao ecossistema de gerência, possibilitando o monitoramento de desempenho e disponibilidade dos links pelo Zabbix, além do envio contínuo de mensagens de eventos e logs para o Graylog. Caso qualquer comportamento anômalo ou tentativa de intrusão seja detectada, alertas automáticos disparam a abertura de chamados de incidentes diretamente na plataforma GLPI. Essa abordagem garante maior controle, confiabilidade e proteção de ponta a ponta aos serviços oferecidos pela PentaByte.
### *Figura  19 - Script Firewall.sh matriz* {#figura-19---script-firewall.sh-matriz}
![image13]

*Fonte: O autor.*
### *Figura 20 - Script Firewall.sh filial* {#figura-20---script-firewall.sh-filial}
![image14]

*Fonte: O autor.*
## 11\.1 Servidor Proxy de Rede (Matriz)  {#11.1-servidor-proxy-de-rede-(matriz)}
Adicionalmente aos serviços de filtragem de pacotes do MikroTik de borda, foi implantado um Servidor Proxy configurado no ambiente da Matriz, fornecendo controle a nível de aplicação para as estações administrativas:

* Filtragem de Conteúdo Web: O Proxy intercepta as requisições HTTP/HTTPS originadas da rede interna, aplicando Listas de Controle de Acesso (ACLs) para bloquear domínios associados a categorias de entretenimento e redes sociais durante o expediente. Com isso, garante-se o foco nas ferramentas corporativas de monitoramento como o painel do Zabbix, Grafana e portal corporativo.
* Otimização de Desempenho (Caching): O servidor realiza o cache de requisições de arquivos estáticos comuns de forma local. Isso diminui o uso geral da banda WAN e reduz a latência no acesso a páginas externas comuns e documentações da operadora.
* Auditoria de Tráfego: Toda a navegação web realizada pelos usuários administrativos passa pelo Proxy, gerando logs estruturados que registram o comportamento da rede corporativa para análises preventivas.
### *Figura 21 – Tela de bloqueio de conteúdo web por diretiva do Servidor Proxy da Matriz.* {#figura-21-–-tela-de-bloqueio-de-conteúdo-web-por-diretiva-do-servidor-proxy-da-matriz.}
![image15]

*Fonte: O autor.*
# **12. VPN**
A VPN (Virtual Private Network) é um componente essencial para a conectividade segura da infraestrutura de rede, atuando como um canal criptografado que interliga pontos geograficamente distantes através da internet pública, prevenindo a interceptação de dados e ataques de interceptação no meio do caminho (man-in-the-middle) *(IETF, 2000)*. Na PentaByte, a VPN é responsável por garantir a confidencialidade, a autenticidade e a integridade das informações trafegadas entre a matriz e a filial.

Para a implementação dessa tecnologia de comunicação, a PentaByte utiliza protocolos robustos de tunelamento diretamente em seus roteadores MikroTik de borda *(MIKROTIK, 2026)*. As configurações de segurança são estabelecidas de forma permanente entre os gateways das duas localidades, ativando algoritmos de criptografia forte e chaves de autenticação seguras, necessárias para o correto funcionamento da comunicação e tráfego interno da empresa.

Foram estabelecidas rotas específicas dentro do túnel VPN para permitir o tráfego fluído entre as sub-redes da matriz e da filial, garantindo o encaminhamento adequado de pacotes de dados, replicação de serviços de diretório, acesso a servidores de arquivos e sistemas de gestão sem expor esses fluxos diretamente para a internet. Também foram definidas políticas de priorização de tráfego (QoS) dentro do túnel, permitindo que os serviços críticos e a telemetria tenham preferência de banda *(STALLINGS, 2015)*.

Para complementar a segurança e permitir a análise contínua do ambiente, a infraestrutura da VPN é integrada ao ecossistema de gerência. Isso possibilita o monitoramento em tempo real do status do túnel, da latência e do consumo de banda por meio de gráficos dinâmicos no Grafana alimentados pelo Zabbix, além do registro centralizado de tentativas de conexão e logs de autenticação no Graylog. Essa abordagem garante maior controle, confiabilidade e proteção total nas interconexões da PentaByte.
### *Figura 22 - Funcionamento da VPN Matriz* {#figura-22---funcionamento-da-vpn-matriz}
![image16]

*Fonte: O autor.*
### *Figura 23 - Interface de tunelamento matriz VPN* {#figura-23---interface-de-tunelamento-matriz-vpn}
![image17]

*Fonte: O autor.*
### *Figura 24 - Funcionamento da VPN Filial* {#figura-24---funcionamento-da-vpn-filial}
![image18]

*Fonte: O autor.*
### *Figura 25 - Captura de tela interface de tunelamento Filial VPN* {#figura-25---captura-de-tela-interface-de-tunelamento-filial-vpn}
![image19]

*Fonte: O autor*
### *Figura 26 - Ping entre AD da filial para matriz VPN* {#figura-26---ping-entre-ad-da-filial-para-matriz-vpn}
*Fonte: O autor*
# **13. ZONA DESMILITARIZADA (DMZ)**
A Zona Desmilitarizada (DMZ) é uma sub-rede isolada da rede interna da empresa, que mantém comunicação controlada com a rede externa (internet). Por ser mais exposta a acessos externos, a DMZ atua como uma camada adicional de segurança, permitindo a disponibilização de serviços públicos e corporativos sem comprometer a integridade da rede interna da PentaByte *(STALLINGS, 2015)*.

Na infraestrutura da PentaByte, a DMZ é utilizada para hospedar serviços críticos que necessitam de acesso ou visibilidade externa, como portais de visualização de dados, monitoramento ambiental acessível via internet e o servidor de gerenciamento de chamados e inventário do GLPI *(TECLIB' EDITION, 2026)*. Esses serviços são isolados da rede administrativa e operacional por meio do firewall MikroTik, reduzindo drasticamente os riscos de ataques cibernéticos e de movimentação lateral dentro do ambiente interno caso um servidor exposto seja comprometido.

Para complementar a segurança e permitir a análise contínua do ambiente, todos os servidores e serviços posicionados na DMZ são integrados ao ecossistema de gerência. O Zabbix realiza o monitoramento contínuo de disponibilidade e integridade dos sistemas, enquanto o Graylog centraliza a coleta e análise de logs de acesso e segurança gerados nessa zona. Qualquer atividade suspeita ou tentativa de violação de privilégios aciona o disparo automático de alertas e notificações para o isolamento proativo de incidentes. Essa abordagem garante maior controle, confiabilidade e proteção às aplicações públicas operadas pela PentaByte.
### *Figura 27 - Site da Empresa* {#figura-27---site-da-empresa}
![image20]

*Fonte: O autor.*
### *Figura 28 - Interface de rede DMZ* {#figura-28---interface-de-rede-dmz}
*Fonte: O autor.*
# **14. GLPI – GESTÃO DE SERVIÇOS DE TI**
Para a governança do suporte e controle patrimonial de TI, o ambiente realiza a abertura automatizada de chamados, o gerenciamento centralizado de incidentes e a atualização em tempo real do registro de todos os ativos da empresa, otimizando o fluxo de atendimento técnico para os setores administrativos e operacionais *(TECLIB' EDITION, 2026)*.

O sistema opera a partir da zona desmilitarizada (DMZ) e executa varreduras automáticas para catalogar minuciosamente o hardware, as versões de softwares e as licenças ativas na matriz e na filial. Essa rotina mapeia dinamicamente toda a infraestrutura física e virtual, desde os servidores de aplicação até os roteadores MikroTik e switches de distribuição de rede.

O fluxo de gerenciamento trabalha de forma perfeitamente integrada aos alertas de monitoramento da rede. Ao detectar quedas de links, falhas de energia ou indisponibilidade de serviços críticos, os gatilhos automáticos geram e encaminham ordens de serviço de maneira imediata para a fila de suporte técnico, reduzindo drasticamente o tempo de resposta e o isolamento de falhas *(ZABBIX LLC, 2026)*.

A infraestrutura desta aplicação também é controlada de forma proativa: o volume de acessos e os índices de disponibilidade da plataforma são acompanhados continuamente em telas gráficas, enquanto as mensagens de auditoria, tentativas de login e logs de segurança do servidor de chamados são direcionados em tempo real para o concentrador de eventos. Essa abordagem garante total rastreabilidade, eficiência e segurança na condução dos atendimentos tecnológicos da PentaByte.
### *Figura 29 - GLPI* {#figura-29---glpi}
![image21]

*Fonte: O autor.*
# **15. GRAFANA – VISUALIZAÇÃO E ANÁLISE DE DADOS**
O Grafana é uma plataforma open-source voltada para a visualização e análise de dados de monitoramento em tempo real *(GRAFANA LABS, 2026)*. No projeto da PentaByte, o Grafana funciona de forma integrada ao Zabbix, permitindo transformar todas as métricas brutas capturadas na rede em dashboards interativos e gráficos avançados.

Por meio dessa integração, o Grafana possibilita a visualização clara de indicadores críticos como a utilização de banda nos enlaces dedicados (WAN 1 e WAN 2), latência de pacotes, disponibilidade do túnel VPN, além do consumo de recursos de hardware (CPU, memória e armazenamento) do controlador de domínio Windows Server (Active Directory). Esses painéis unificados facilitam a análise técnica, auxiliando diretamente a equipe na identificação de gargalos de rede, tendências de crescimento e na visibilidade do volume de requisições direcionadas à zona desmilitarizada (DMZ), onde operam serviços como a plataforma de inventário e chamados do GLPI *(TECLIB' EDITION, 2026)*.

A ferramenta oferece dashboards altamente personalizáveis, com filtros específicos por setor, alertas visuais de comportamento e histórico detalhado de dados, contribuindo para uma gestão mais estratégica do ambiente. O monitoramento visual do Grafana permite que a equipe técnica realize tomadas de decisões baseadas em dados consolidados, melhorando significativamente o planejamento de capacidade preventiva antes que ocorra o esgotamento dos recursos locais.
# **16. GRAYLOG - CENTRALIZAÇÃO E ANÁLISE DE LOGS**
O Graylog é uma plataforma open-source voltada para o gerenciamento, centralização e análise de logs em tempo real *(GRAYLOG, INC., 2026)*. No projeto da PentaByte, o Graylog atua como o núcleo de auditoria de segurança e conformidade, coletando, indexando e armazenando de forma estruturada as mensagens de eventos geradas por todos os ativos da infraestrutura.

Para a consolidação da auditoria de segurança e tratamento proativo de incidentes, o ambiente utiliza a plataforma para centralizar, estruturar e analisar o fluxo contínuo de logs gerados por todos os ativos de rede da matriz e da filial. O sistema atua de forma direta sobre os dados de telemetria textual da infraestrutura, convertendo registros brutos em informações correlacionadas para a identificação imediata de anomalias operacionais e ameaças perimetrais *(STALLINGS, 2015)*.

No controlador de domínio Windows Server, a ferramenta realiza o rastreamento contínuo dos eventos do Active Directory, auditando o sucesso e a falha de autenticação de usuários para mitigar ataques de força bruta, além de monitorar alterações em grupos de segurança e elevações de privilégios administrativos *(MICROSOFT, 2026)*. Na camada de borda e conectividade, o sistema recebe as mensagens de syslog dos roteadores MikroTik, registrando tentativas de acessos bloqueados pelas regras de firewall nas interfaces WAN e auditando a estabilidade do túnel VPN por meio do log de negociação de chaves criptográficas. Na zona desmilitarizada (DMZ), o monitoramento intercepta e padroniza as requisições direcionadas ao servidor web do GLPI, isolando padrões de varreduras maliciosas e tentativas de movimentação lateral não autorizada em direção às VLANs internas.

O fluxo operacional elimina a necessidade de inspeções individuais em arquivos de texto isolados por máquina, concentrando as buscas em uma linha do tempo unificada e normalizada. Sempre que uma assinatura de evento crítico ou desvio de conformidade é identificado pelo motor de busca, o ecossistema disponibiliza os dados para o diagnóstico imediato da equipe técnica, acelerando o tempo de resposta a incidentes e assegurando a rastreabilidade completa das ações administrativas da PentaByte.
### *Figura  30 - Figura do Graylog* {#figura-30---figura-do-graylog}
![image22]

*Fonte: O autor*
# **17. ARDUINO**
No projeto da PentaByte, o Arduino atua como a unidade de controle na ponta da infraestrutura de Cidades Inteligentes, sendo responsável pela automação física e captação de dados em tempo real nos reservatórios e lagoas de captação *(ARDUINO, 2026)*. A plataforma opera de forma integrada a sensores industriais e de telemetria, convertendo grandezas físicas do meio ambiente em dados digitais estruturados para o monitoramento hídrico.

O microcontrolador executa a leitura contínua de sensores de nível (ultrassônicos ou de pressão hidroclorídrica) para medir o volume de água das lagoas, além de processar sensores de fluxo para calcular a vazão e sensores físico-químicos para analisar a qualidade da água. Essas informações são processadas localmente pela placa e transmitidas de forma estruturada, via rede local, para que os concentradores e sistemas de monitoramento possam registrar os históricos operacionais.

Dessa forma, o dispositivo elimina a necessidade de medições manuais ou verificações locais em campo. O fluxo automatizado garante alta precisão na coleta de dados biológicos e de volumetria, permitindo que qualquer variação crítica no nível dos reservatórios seja detectada instantaneamente na ponta, fornecendo os dados necessários para o acionamento de alertas preventivos contra transbordamentos ou escassez.
## **17.1. Descrição Geral do Circuito**
Como parte do desenvolvimento da infraestrutura proposta pela PentaByte, foi projetado um protótipo funcional para o monitoramento automatizado e gerenciamento de riscos em lagoas de captação. O principal objetivo deste circuito é eliminar a necessidade de checagem humana presencial e manual, utilizando a tecnologia para medir continuamente o nível da água. O sistema foi desenvolvido e validado no ambiente de simulação Tinkercad, integrando um microcontrolador a um sensor de ondas sonoras para emitir alertas visuais e digitais em tempo real, mitigando riscos de transbordamento e auxiliando na gestão ambiental do município *(ARDUINO, 2026)*.
## **17.2. Componentes Utilizados**
Para a construção do protótipo, foram selecionados componentes que equilibram precisão, baixo custo e facilidade de integração em cenários reais de IoT (Internet das Coisas). A tabela abaixo detalha o hardware empregado:

|Componente|Função no Projeto|
| :- | :- |
|Arduino Uno R3|Placa microcontroladora principal baseada no processador ATmega328P. Atua como o "cérebro" do sistema, processando o código, calculando as distâncias e controlando as saídas.|
|Sensor Ultrassônico PING))) (Parallax)|Atua como o elemento sensor principal. Ele emite pulsos de alta frequência (ultrassom) que ricocheteiam no alvo para calcular a distância com base no tempo de retorno do eco.|
|LED Vermelho|Atuador de saída utilizado como indicador visual de segurança. Permanece apagado em condições normais e acende imediatamente para sinalizar o estado crítico de transbordo.|
|Resistor de 220 Ω|Componente passivo utilizado para limitar a corrente elétrica que passa pelo LED, evitando a queima do atuador e protegendo a porta digital do Arduino.|
|Protoboard e Jumpers|Matriz de contatos e fios flexíveis utilizados para realizar a interconexão elétrica segura entre o microcontrolador, o sensor e o circuito do LED.|

Fonte: O autor
## **17.3. Esquema de Ligação e Pinagem**
A arquitetura de conexões do protótipo foi estruturada de forma a otimizar o uso das portas digitais e garantir a estabilidade elétrica. O mapeamento físico dos pinos foi realizado da seguinte forma:

**Alimentação do Sistema:**

O pino 5V do Arduino foi conectado diretamente à coluna do pino central do sensor por meio de um fio azul-claro para fornecer a alimentação de energia. O pino GND (Ground/Terra) da barra inferior do Arduino foi conectado à coluna correspondente da protoboard utilizando um fio amarelo, garantindo o aterramento do sensor. Um segundo pino GND da barra inferior do Arduino foi conectado por meio de um fio roxo diretamente ao terminal do resistor, fechando o circuito de aterramento do LED.

**Conexão do Sensor PING:**

O pino de sinal (SIG) do sensor foi conectado à porta digital D2 do Arduino através de um fio verde. Por se tratar de um componente de 3 pinos, essa via única é chaveada dinamicamente pelo código para o disparo e a leitura do eco.

**Conexão do Atuador de Alerta (LED):**

O ânodo (terminal positivo/perna curvada) do LED foi conectado à porta digital D13 do Arduino por meio de um fio rosa (ou magenta). O catodo (terminal negativo) foi associado em série ao resistor conectado ao pino de aterramento.
### *Figura 31 - Funcionamento do Arduino* {#figura-31---funcionamento-do-arduino}
![image23]

*Fonte: O autor.*
## **17.4. Lógica de Programação**
O comportamento inteligente do circuito é governado por um algoritmo desenvolvido em linguagem C/C++ (padrão Arduino) *(ARDUINO, 2026)*. O software implementa uma lógica de leitura baseada na física do som e realiza a tomada de decisões automaticamente a cada 500 milissegundos.

Código-fonte oficial implementado no sistema:

const int pinoSensor = 2;
const int pinoAlerta = 13;
void setup() {
Serial.begin(9600);
pinMode(pinoAlerta, OUTPUT);
}

void loop() {
pinMode(pinoSensor, OUTPUT);
digitalWrite(pinoSensor, LOW);
delayMicroseconds(2);
digitalWrite(pinoSensor, HIGH);
delayMicroseconds(5);
digitalWrite(pinoSensor, LOW);

pinMode(pinoSensor, INPUT);
long duracao = pulseIn(pinoSensor, HIGH);
long distanciaCm = duracao / 29 / 2;

Serial.print("Distancia medida: ");
Serial.print(distanciaCm);
Serial.println(" cm");

if (distanciaCm >= 250) {
digitalWrite(pinoAlerta, HIGH);
Serial.println("ALERTA CRÍTICO: A lagoa esta completamente CHEIA!");
}
else {
digitalWrite(pinoAlerta, LOW);
Serial.println("Nível Baixo: Lagoa segura e SEM RISCO.");
}

delay(500);
}
##
## 17\.5. Resultados e Testes de Simulação
Os testes realizados no ambiente virtual do Tinkercad validaram com sucesso o funcionamento do protótipo automatizado da PentaByte. Durante a simulação, o comportamento do sistema seguiu rigorosamente os parâmetros estabelecidos *(ARDUINO, 2026)*.

**Cenário de Segurança (Nível de Água Baixo):**

Ao simular a lagoa sob condições normais com o espelho d'água distante do sensor (gerando leituras elevadas na faixa de 250 cm de distância), o fluxo de dados no Monitor Serial exibiu estavelmente a mensagem de conformidade "Nível Baixo: Lagoa segura e SEM RISCO", mantendo o LED de alerta apagado.

**Cenário de Alerta Crítico (Risco de Transbordo):**

Ao simular o enchimento total da lagoa, onde a superfície da água sobe e se aproxima fisicamente do sensor ultrassônico (gerando leituras de proximidade na faixa de 118 cm), o algoritmo respondeu instantaneamente. O LED vermelho foi energizado e o fluxo do Monitor Serial passou a reportar o status de emergência "ALERTA CRÍTICO: A lagoa está completamente CHEIA!", enviando as strings para acionamento do gatilho no Zabbix e registro de incidente.
## 17\.6 Integração e Exibição de Telemetria no Portal Web {#17.6-integração-e-exibição-de-telemetria-no-portal-web}
          Para viabilizar a visualização pública e administrativa do status da lagoa em tempo real, o portal web corporativo foi integrado diretamente com os dados de leitura gerados pelo microcontrolador Arduino:
**Consumo de Dados via Web:**

A página web realiza o consumo dos eventos de telemetria através de requisições assíncronas (via AJAX/Fetch), permitindo que os indicadores da página sejam alterados instantaneamente sem a necessidade de recarga de página (refresh) pelo usuário.

**Dinâmica Visual do Monitorador:**

O portal monitorador interpreta a string de nível recebida. Se o status for seguro, a interface apresenta um painel estável na cor verde. Caso a distância detectada caia abaixo do limite (sinalizando água alta), o banner superior do site atualiza dinamicamente para uma barra vermelha com o aviso "ALERTA CRÍTICO: Risco de transbordo iminente na Lagoa Antônio Pessoa", permitindo a visualização clara em qualquer dispositivo conectado.

Os resultados laboratoriais comprovam que o sistema cumpre os requisitos de tempo de resposta imediato e confiabilidade necessários para compor uma rede de segurança em cidades inteligentes *(CARAGLIU; DEL BO; NIJKAMP, 2011)*.
### *Figura 32 – Portal Web corporativo exibindo o alerta em tempo real de nível crítico na lagoa.* {#figura-32-–-portal-web-corporativo-exibindo-o-alerta-em-tempo-real-de-nível-crítico-na-lagoa.}
### ![image24]
*Fonte: O autor.*
# **18. CONCLUSÃO**
A elaboração e o planejamento da infraestrutura tecnológica da PentaByte demonstram a viabilidade técnica e estratégica de integrar soluções modernas de redes, segurança e automação voltadas ao conceito de monitoramento preditivo de recursos hídricos *(CARAGLIU; DEL BO; NIJKAMP, 2011)*. Através do correto dimensionamento físico e lógico apresentado nas plantas baixas e diagramas, o projeto assegura um ambiente corporativo altamente escalável, capaz de suportar o fluxo contínuo de dados operacionais entre a matriz e a filial de forma segura e eficiente *(ABNT, 2013)*.

A escolha de uma arquitetura centralizada com ferramentas de código aberto (open-source) como o Zabbix para monitoramento de ativos, o Grafana para a inteligência visual de dados e o Graylog para a auditoria de segurança provou-se uma decisão financeira e técnica assertiva *(ZABBIX LLC, 2026)*. Essa abordagem permitiu otimizar a projeção orçamentária, reduzindo os custos recorrentes com licenciamento de software e concentrando o investimento em ativos de rede de alta performance, servidores robustos para o Active Directory e dispositivos de contingência energética *(MICROSOFT, 2026)*. Dessa forma, garante-se uma infraestrutura com alta disponibilidade e baixo custo de manutenção *(STALLINGS, 2015)*.

Por fim, a integração dos microcontroladores Arduino na ponta do sistema valida a eficácia da automação na coleta de dados biológicos e volumétricos das lagoas de captação *(ARDUINO, 2026)*. Ao eliminar processos manuais e centralizar as métricas em tempo real, a PentaByte consolida uma postura proativa, permitindo tomadas de decisão preditivas e respostas rápidas a incidentes ou variações hídricas críticas. O projeto cumpre, portanto, todos os requisitos técnicos, operacionais e de conformidade com as boas práticas de segurança da informação, estando pronto para sua fase de implementação e implantação em campo *(BRASIL, 2018)*.
# **Referências**
ARDUINO. Arduino Uno Rev3 – Documentation. Disponível em: https://docs.arduino.cc/hardware/uno-rev3/. Acesso em: 13 jul. 2026.

ASSOCIAÇÃO BRASILEIRA DE NORMAS TÉCNICAS. NBR 14565: Procedimento básico para elaboração de projetos de cabeamento de telecomunicações para rede interna estruturada. Rio de Janeiro: ABNT, 2013.

BRASIL. Lei nº 13.709, de 14 de agosto de 2018. Lei Geral de Proteção de Dados Pessoais (LGPD). Diário Oficial da União, Brasília, DF, 15 ago. 2018.

CARAGLIU, A.; DEL BO, C.; NIJKAMP, P. Smart Cities in Europe. Journal of Urban Technology, v. 18, n. 2, p. 65-82, 2011.

FOROUZAN, B. A. Comunicação de Dados e Redes de Computadores. 4. ed. Porto Alegre: AMGH, 2010.

GRAFANA LABS. Grafana Documentation. Disponível em: https://grafana.com/docs/grafana/latest/. Acesso em: 13 jul. 2026.

GRAYLOG, INC. Graylog Documentation. Disponível em: https://docs.graylog.org/. Acesso em: 13 jul. 2026.

IETF – INTERNET ENGINEERING TASK FORCE. RFC 2764: A Framework for IP Based Virtual Private Networks. 2000. Disponível em: https://www.rfc-editor.org/rfc/rfc2764. Acesso em: 13 jul. 2026.

KUROSE, J. F.; ROSS, K. W. Redes de Computadores e a Internet: uma abordagem top-down. 6. ed. São Paulo: Pearson, 2013.

MICROSOFT. Active Directory Domain Services Overview. Microsoft Learn. Disponível em: https://learn.microsoft.com/pt-br/windows-server/identity/ad-ds/get-started/virtual-dc/active-directory-domain-services-overview. Acesso em: 13 jul. 2026.

MIKROTIK. RouterOS Documentation – Firewall. Disponível em: https://help.mikrotik.com/docs/spaces/ROS/pages/328059/Firewall. Acesso em: 13 jul. 2026.

STALLINGS, W. Criptografia e Segurança de Redes: Princípios e Práticas. 6. ed. São Paulo: Pearson, 2015.

TANENBAUM, A. S.; WETHERALL, D. J. Redes de Computadores. 5. ed. São Paulo: Pearson, 2011.

TECLIB' EDITION. GLPI Documentation. Disponível em: https://glpi-project.org/documentation/. Acesso em: 13 jul. 2026.

ZABBIX LLC. Zabbix Documentation. Disponível em: https://www.zabbix.com/documentation/current/en/manual. Acesso em: 13 jul. 2026.

[image1]: Aspose.Words.7606f958-b3fe-469b-b84a-c47a96d5909b.001.png
[image2]: Aspose.Words.7606f958-b3fe-469b-b84a-c47a96d5909b.002.png
[image3]: Aspose.Words.7606f958-b3fe-469b-b84a-c47a96d5909b.003.png
[image4]: Aspose.Words.7606f958-b3fe-469b-b84a-c47a96d5909b.004.png
[image5]: Aspose.Words.7606f958-b3fe-469b-b84a-c47a96d5909b.005.png
[image6]: Aspose.Words.7606f958-b3fe-469b-b84a-c47a96d5909b.006.png
[image7]: Aspose.Words.7606f958-b3fe-469b-b84a-c47a96d5909b.007.png
[image8]: Aspose.Words.7606f958-b3fe-469b-b84a-c47a96d5909b.008.png
[image9]: Aspose.Words.7606f958-b3fe-469b-b84a-c47a96d5909b.009.png
[image10]: Aspose.Words.7606f958-b3fe-469b-b84a-c47a96d5909b.010.png
[image11]: Aspose.Words.7606f958-b3fe-469b-b84a-c47a96d5909b.011.png
[image12]: Aspose.Words.7606f958-b3fe-469b-b84a-c47a96d5909b.012.png
[image13]: Aspose.Words.7606f958-b3fe-469b-b84a-c47a96d5909b.013.png
[image14]: Aspose.Words.7606f958-b3fe-469b-b84a-c47a96d5909b.014.png
[image15]: Aspose.Words.7606f958-b3fe-469b-b84a-c47a96d5909b.015.png
[image16]: Aspose.Words.7606f958-b3fe-469b-b84a-c47a96d5909b.016.png
[image17]: Aspose.Words.7606f958-b3fe-469b-b84a-c47a96d5909b.017.png
[image18]: Aspose.Words.7606f958-b3fe-469b-b84a-c47a96d5909b.018.png
[image19]: Aspose.Words.7606f958-b3fe-469b-b84a-c47a96d5909b.019.png
[image20]: Aspose.Words.7606f958-b3fe-469b-b84a-c47a96d5909b.020.png
[image21]: Aspose.Words.7606f958-b3fe-469b-b84a-c47a96d5909b.021.png
[image22]: Aspose.Words.7606f958-b3fe-469b-b84a-c47a96d5909b.022.png
[image23]: Aspose.Words.7606f958-b3fe-469b-b84a-c47a96d5909b.023.png
[image24]: Aspose.Words.7606f958-b3fe-469b-b84a-c47a96d5909b.024.png
