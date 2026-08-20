#  Estudo de Caso: Sistema de Gestão e Monitoramento de Portaria (SGMP)

Projeto acadêmico focado na análise, modelagem e desenvolvimento de um sistema de controle de acesso e segurança condominial em Python.

---

##  Visão Geral do Projeto
O SGMP é uma solução integrada de controle de acesso para portarias e aplicativos móveis para moradores, unindo autenticação biométrica, comunicação em tempo real e resposta rápida a emergências.

---

##  Pilha de Tecnologias & Metodologia

* **Linguagem Principal:** Python (Backend e lógica de alertas)
* **Metodologia de Gestão:** Scrum (Entregas ágeis em Sprints)
* **Ciclo de Vida de Software:** Modelo Espiral (Gestão de riscos e prototipagem)

---

##  Funcionalidades & Arquitetura

###  Aplicativo do Morador
* **Atendimento Remoto:** Chamada de áudio/vídeo para autorização de visitantes.
* **Módulo SOS / Emergência (1 Clique):** Botão de acionamento imediato para solicitar ajuda (Segurança do Condomínio, Polícia ou Ambulância) com envio automático de dados de localização e alerta prioritário na central.

### Totem da Portaria
* **Autenticação Biométrica Dupla:** Reconhecimento facial principal e leitor digital de contingência.
* **Câmera IR (Infravermelho):** Resolução otimizada para leitura noturna e sob luz forte.
* **Módulo de IA (Escopo Futuro):** Análise comportamental e detecção de vivacidade.

---

## Requisitos Não Funcionais de Segurança (Blue Team)
* **Prioridade de Tráfego:** Os alertas do Botão SOS possuem prioridade máxima na fila de rede (baixa latência).
* **Registro em Log de Auditoria:** Cada acionamento do SOS gera um registro imutável com data, hora, morador e tempo de resposta da portaria.
