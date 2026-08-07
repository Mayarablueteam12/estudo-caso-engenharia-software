# 🛡️ Estudo de Caso: Sistema de Gestão e Monitoramento de Portaria (SGMP)

Projeto acadêmico focado na análise, escolha e justificativa do ciclo de vida de desenvolvimento de software para um sistema de controle de acesso predial com reconhecimento facial.

---

## 📌 Visão Geral do Projeto
O objetivo do sistema é controlar o acesso de moradores e visitantes em um condomínio por meio de leitura biométrica facial, garantindo alta precisão, rapidez e segurança.

## 🎯 Modelo de Desenvolvimento Escolhido: Modelo Espiral

### Justificativa da Escolha:
Devido à alta taxa de incerteza inicial e aos riscos técnicos envolvidos, o **Modelo Espiral** foi escolhido por priorizar a **análise de riscos e a prototipagem contínua** a cada ciclo.

---

## 🔍 Mapeamento de Riscos e Testes (1º Ciclo da Espiral)

1. **Iluminação e Captação da Câmera:**
   - *Risco:* Dificuldade de leitura em horários de sol forte (contra-luz) ou à noite.
   - *Ação:* Teste de sensores com iluminação infravermelha e ajuste do posicionamento.

2. **Performance e Latência:**
   - *Risco:* Análise demorada (acima de 2 segundos) gerando filas no portão.
   - *Ação:* Validação do processamento facial em servidor local (*edge*) para evitar atrasos de rede.

3. **Segurança (Bloqueio de Não Autorizados):**
   - *Risco:* Falsos positivos ou tentativas de engano usando fotos de moradores (*anti-spoofing*).
   - *Ação:* Implementação e validação de detecção de vivacidade (*liveness detection*).

---

## 💡 Aprendizados e Conclusão
A principal vantagem da abordagem Espiral é permitir que falhas identificadas nos protótipos (como lentidão de resposta) sejam corrigidas no ciclo seguinte antes do desenvolvimento do produto final, garantindo qualidade e eficiência.

---
*Projeto desenvolvido para a disciplina de Engenharia de Software.*

