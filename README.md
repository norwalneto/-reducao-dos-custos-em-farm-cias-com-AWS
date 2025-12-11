# Relatório de Redução de Custos com AWS  
**Projeto DIO – Operação Farmacêutica**  
**Empresa:** Abstergo Industries  
**Data:** 11/12/2025  
**Responsável:** Norwal  

---

## 1. Introdução

Este documento apresenta a análise, escolha e implementação de três serviços AWS com foco exclusivo na redução imediata de custos operacionais da Abstergo Industries.  
O estudo foi realizado no contexto do projeto prático da DIO, com ênfase em eficiência, governança e otimização financeira no ambiente em nuvem.

A abordagem foi objetiva: identificar gastos excessivos, eliminar desperdícios, adotar serviços gerenciados e aplicar modelos de cobrança sob demanda, especialmente para aplicações da área farmacêutica que exigem disponibilidade, integridade e rastreabilidade.

---

## 2. Descrição do Projeto

A iniciativa foi organizada em três etapas, cada uma resultando em cortes claros de custos sem comprometer resiliência, disponibilidade ou segurança.

---

### **Etapa 1 – Amazon S3 + Lifecycle Policies**

**Foco:** Redução agressiva de custos de armazenamento.  
**Caso de uso:**  
A empresa mantinha arquivos e dados farmacêuticos em EC2 e infraestrutura local, elevando custos de manutenção e capacidade.  
A migração para o Amazon S3, combinada com Lifecycle Policies, permitiu mover dados pouco acessados para classes mais baratas, como S3 Standard-IA e S3 Glacier.

**Impacto direto:**
- Economia de até **70%** no armazenamento.  
- Eliminação de servidores dedicados.  
- Durabilidade elevada para **99,999999999%**.  
- Armazenamento escalável e com custo proporcional ao uso.  

---

### **Etapa 2 – AWS Lambda (Serverless)**

**Foco:** Redução de custos com execução sob demanda.  
**Caso de uso:**  
Rotinas internas (auditoria, organização de dados e processos farmacêuticos) eram executadas em instâncias EC2 superdimensionadas, custando mesmo quando ocioso.  
A migração dessas rotinas para AWS Lambda eliminou custos fixos.

**Impacto direto:**
- Pagamento exclusivamente por execução.  
- Economia entre **80% e 90%** para workloads event-driven.  
- Zero custo em períodos ociosos.  
- Eliminação de instâncias subutilizadas.  

---

### **Etapa 3 – Amazon RDS Serverless + Read Replicas**

**Foco:** Otimização de custos e escalabilidade de banco de dados.  
**Caso de uso:**  
O banco relacional funcionava continuamente, com picos ocasionais e longos períodos ociosos, causando desperdício.  
Com RDS Serverless Auto Pause, o banco passa a pausar sozinho quando não há consulta.  
Read Replicas absorvem cargas de leitura, evitando aumento da instância principal.

**Impacto direto:**
- Economia mensal entre **30% e 55%**.  
- Redução da sobrecarga e maior estabilidade.  
- Escalabilidade automática, sem expansão desnecessária.  

---

## 3. Conclusão

As soluções aplicadas garantem redução imediata de custos estruturais, sustentando um ambiente mais leve, econômico e eficiente.  
A Abstergo Industries passa a operar com práticas de otimização que se alinham às recomendações corporativas de governança e compliance, especialmente importantes no setor farmacêutico.

Recomenda-se manter revisões periódicas de consumo, utilizar o AWS Cost Explorer e ampliar o uso de serviços totalmente gerenciados para sustentar o ciclo contínuo de melhoria.

---

## 4. Anexos

### **Diagrama de Arquitetura (opcional)**
Coloque aqui a imagem do seu diagrama ou o link para ela.

### **Link do Repositório GitHub**
`https://github.com/seuusuario/seurepositorio`

### **Capturas de Tela das Configurações**
Recomendação de estrutura:  
