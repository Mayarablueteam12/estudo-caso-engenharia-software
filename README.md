# 🛡️ Estudo de Caso: Sistema de Gestão e Monitoramento de Portaria (SGMP)

Projeto acadêmico focado na análise, escolha e justificativa do ciclo de vida de desenvolvimento de software para um sistema de controle de acesso predial com reconhecimento facial e Inteligência Artificial.

---

## 📌 Visão Geral do Projeto
O objetivo do sistema é controlar o acesso de moradores e visitantes em um condomínio por meio de leitura biométrica e monitoramento inteligente, garantindo alta precisão, rapidez e mitigação de riscos de segurança física e digital.

---

## 🎯 Modelo de Desenvolvimento Escolhido: Modelo Espiral

### Justificativa da Escolha:
Devido à alta taxa de incerteza inicial, necessidade de ajustes constantes e riscos técnicos de integração hardware/software, o **Modelo Espiral** foi escolhido por priorizar a **análise de riscos e a prototipagem contínua** a cada ciclo.

---

## 📐 Arquitetura da Interface da Portaria & Hardware

O totem de acesso na portaria integra componentes de leitura biométrica e comunicação direta com o usuário:

* **Autenticação Dupla (Face + Digital):** Suporte a reconhecimento facial principal e leitor de impressão digital como contingência/redundância.
* **Câmera IR (Infravermelho) de Alta Resolução:** Garantia de leitura precisa em qualquer condição de iluminação (sol forte ou ambiente noturno).
* **Módulo de Chamada ao Morador:** Comunicação em tempo real integrada via aplicativo para autorização remota de visitantes pelo morador.

---

## 🤖 Inteligência Artificial & Análise de Riscos (Blue Team)

A IA embarcada atua na prevenção de incidentes na entrada do condomínio:

1. **Anti-Spoofing (Detecção de Vivacidade):**
   - Valida se a imagem é de uma pessoa física presente no local, impedindo fraudes com fotos, vídeos ou máscaras.

2. **Detecção Comportamental e Alerta de Coação:**
   - Monitoramento de anomalias na tentativa de acesso para evitar invasões ou tentativas de furto, emitindo alertas silenciosos ao centro de monitoramento caso detectada situação de risco.

3. **Performance e Baixa Latência:**
   - Processamento biométrico otimizado (*Edge Computing*) para garantir resposta rápida sem criar filas de acesso.

---

## 💡 Aprendizados e Conclusão
A abordagem Espiral permite que falhas identificadas nos protótipos de hardware e software (como ajustes de iluminação na câmera ou latência da IA) sejam corrigidas no ciclo seguinte antes da implantação final, garantindo a eficiência do sistema.

---
*Projeto desenvolvido para a disciplina de Engenharia de Software.*
