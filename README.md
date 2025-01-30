# Laboratorio-BGP101
📂 Este repositório contém as configurações do Laboratório Final do Curso BGP 101 da Leonardo Furtado Academy. 🌍 O projeto simula uma rede com múltiplos ASs, implementando BGP avançado 🔄, segurança 🔒, MPLS 🚀 e MP-BGP para VPNv4/VPNv6.


📖 Introdução
Concluí o laboratório final do curso BGP 101: O Curso Mais Completo sobre Border Gateway Protocol (BGP) na Leonardo Furtado Academy. Este foi um desafio prático que consolidou meus conhecimentos sobre BGP, abordando filtros de anúncio, segurança, engenharia de tráfego e VPNs.
________________________________________
🌐 Descrição da Topologia
O ambiente simula uma rede complexa com múltiplos Sistemas Autônomos (ASs) interconectados, refletindo um cenário realista de operação BGP.
•	AS11: Cliente do AS1, contrata trânsito IP para fornecer internet aos assinantes.
•	AS1: Conectado ao AS2, estabelecendo uma relação de trânsito IP.
•	AS2: 
o	Core da rede com Route Reflectors (R2 e R3).
o	Cliente do AS4 e AS5 para trânsito global.
o	Fornece backbone para o AS65000, que tem dois sites interligados via VPNv4/VPNv6 e também acessa a internet.
•	AS3: Cliente do AS2, com um cliente direto AS31.
________________________________________
⚙️ Etapas de Configuração
1.	🔧 Configuração Inicial
o	Definição de hostnames, senhas, interfaces e loopbacks para IPv4 e IPv6.
2.	📡 OSPFv3 no AS2
o	Transporte do IBGP e recursividade do NEXT_HOP, otimizando a topologia.
3.	🔁 IBGP no AS2
o	Configuração de Route Reflectors, communities e NEXT_HOP self.
4.	🌍 EBGP entre ASs
o	Estabelecimento de peering e propagação de communities entre ASs.
5.	📢 Anúncio de Rotas
o	Redistribuição de prefixos com route-maps e prefix-lists.
6.	🚦 Filtros de Anúncio
o	Prevenção de route leaks, filtragem de prefixos bogon e definição de LOCAL_PREF.
7.	🚀 Engenharia de Tráfego
o	Configuração de políticas BGP, incluindo RTBH para mitigação de DDoS.
8.	🔒 Segurança
o	Implementação de MD5, GTSM, uRPF strict mode e CoPP.
9.	🏆 BGP VPNv4/VPNv6
o	Configuração de MPLS e MP-BGP para interligar os sites do AS65000.
________________________________________
🙌 Agradecimento
Agradeço ao Leonardo Furtado pela excelente metodologia e pelo conteúdo aprofundado deste curso. A experiência proporcionada foi essencial para consolidar meus conhecimentos sobre BGP e redes escaláveis. 🚀

________________________________________
✅ Conclusão
O laboratório foi concluído com sucesso, implementando todas as configurações necessárias para garantir funcionalidade, segurança e eficiência da rede. A topologia complexa permitiu testar cenários reais de roteamento, engenharia de tráfego e VPNs. 💪
