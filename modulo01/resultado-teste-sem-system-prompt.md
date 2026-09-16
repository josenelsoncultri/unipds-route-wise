Com base na transcrição da reunião de discovery do projeto **RouteWise**, estruturei as informações em um formato de **Documento de Requisitos e Definição de Escopo**. Este material pode ser usado como base para a criação de Backlog, PRDs (Product Requirement Documents) ou Planos de Projeto.

---

# Relatório de Discovery: Projeto RouteWise

## 1. Visão Geral
O projeto visa substituir um sistema de rastreamento de 2016 por uma solução moderna e automatizada para a gestão de uma frota de 140 veículos. O foco principal é a redução de custos (multas), aumento da segurança (prevenção de acidentes) e automação de processos gerenciais manuais.

## 2. Participantes
*   **Carlos Mendonça:** Diretor de Operações (Stakeholder Principal/Business Owner)
*   **Marcus:** Consultor Externo (Facilitador/PM)
*   **Priya:** TI/Infraestrutura (Responsável Técnica)

## 3. Dores Atuais (Pain Points)
*   **Monitoramento Manual:** Operadores precisam vigiar telas constantemente; falhas humanas durante turnos e intervalos.
*   **Prejuízo Financeiro:** Multas de excesso de velocidade por falta de intervenção imediata.
*   **Segurança:** Risco de acidentes graves sem alertas preventivos.
*   **Falta de Visibilidade de Hardware:** Dispositivos GPS ficam offline ou sem bateria sem que a central saiba, gerando "pontos cegos".
*   **Carga de Trabalho Administrativa:** Carlos gasta ~2 horas semanais gerando relatórios manuais em Excel para a diretoria e RH.

## 4. Requisitos Funcionais (MVP - Release 1)

### 4.1. Rastreamento e Alertas
*   **Alertas de Velocidade em Tempo Real:** Notificação imediata para o supervisor da rota quando o limite for excedido.
*   **Escalação de Alertas:** Se o supervisor não atuar em "X" minutos, o alerta deve ser escalado para a coordenação.
*   **Regras Configuráveis:** O sistema deve permitir configurar limites de velocidade diferentes por:
    *   Tipo de veículo (ex: caminhão pesado vs. van leve).
    *   Tipo de rota (ex: trecho urbano vs. rodovia).
*   **Interface de Mapa:** Visualização em tempo real para o operador de despacho.

### 4.2. Gestão de Dispositivos (Health Check)
*   **Status de Conexão:** Alerta imediato se um dispositivo ficar offline por um período determinado.
*   **Monitoramento de Bateria:** Visualização do nível de carga (para dispositivos compatíveis).
*   **Inventário Digital:** Substituir a planilha de Excel por um dashboard de status dos 140 rastreadores.

### 4.3. Dashboards e Relatórios
*   **Dashboard Gerencial:** Automatização de indicadores (veículos rodados, alertas gerados, ranking de motoristas com mais ocorrências).
*   **Exportação para RH:** Funcionalidade de exportar dados de conduta dos motoristas para o sistema de gestão de pessoas (formato a definir: API ou CSV).

## 5. Requisitos Não-Funcionais e Restrições
*   **Baixa Latência:** O "tempo real" deve ser rápido o suficiente para permitir intervenção antes do término da infração.
*   **Perfis de Acesso:**
    1.  **Operador:** Foco no mapa e alertas.
    2.  **Técnico:** Foco na saúde dos dispositivos.
    3.  **Gestor (Carlos):** Foco em relatórios, dashboards e configuração de regras.
*   **Conformidade (LGPD):** Necessidade de validação jurídica sobre o rastreamento de dados sensíveis de motoristas e termos de consentimento.

## 6. Roadmap e Futuro (Fase 2)
*   **Detecção de Frenagem Brusca:** Utilização dos dados de acelerômetro dos novos rastreadores para análise de perfil de risco.
*   **Manutenção Preditiva:** Cruzamento de histórico de uso com dados de manutenção (atualmente em planilhas orgânicas).
*   **Substituição de Hardware:** Upgrade dos rastreadores antigos para modelos com acelerômetro.

## 7. Próximos Passos e Ações
| Ação | Responsável | Prazo/Status |
| :--- | :--- | :--- |
| Cotação de novos rastreadores (140 unidades) | Carlos | Esta semana |
| Levantamento de custo/prazo de instalação com fornecedor atual | Priya | A definir |
| Verificar existência de API no sistema do RH | Marcus | A definir |
| Consulta ao departamento de Compliance/Jurídico sobre LGPD | Priya/Carlos | Urgente |
| **Apresentação do MVP no Board** | **Time** | **Julho/2026** |

---
*Transcrição processada para fins de documentação de projeto.*