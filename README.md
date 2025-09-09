<h1 align="center">Olá 👋, eu sou o Otávio Ribeiro</h1>
<h3 align="center">Data Engineering Manager @ Educbank — Databricks • Spark • Delta Lake • Orquestração</h3>

<p align="center">
  <a href="https://github.com/Donotavio">
    <img src="https://visitor-badge.laobi.icu/badge?page_id=Donotavio" alt="visits"/>
  </a>
  <a href="https://wakatime.com/@ee59639e-06da-4c79-af0f-2be09bc8780a">
    <img src="https://wakatime.com/badge/user/ee59639e-06da-4c79-af0f-2be09bc8780a.svg" alt="WakaTime"/>
  </a>
</p>

<p align="center">
  <img src="https://github-readme-streak-stats.herokuapp.com/?user=Donotavio&theme=radical" alt="GitHub Streak"/>
</p>

<!-- Troféus: apenas os que têm pontuação no seu perfil -->
<p align="center">
  <img src="https://github-profile-trophy.vercel.app/?username=Donotavio&theme=radical&no-frame=true&no-bg=true&title=MultiLanguage,LongTimeUser,Experience,Repositories,Stars" alt="GitHub Trophies filtrados"/>
</p>

---

## Sobre mim
Sou **Gerente de Engenharia de Dados na Educbank** (fintech) e uso **Databricks como feature platform** para unificar pipelines, modelagem com **Delta Lake** e **workflows de ML**. No dia a dia:
- desenho e otimizo pipelines batch/streaming (custo, performance e confiabilidade);
- garanto governança & compliance (**LGPD/GDPR**), versionamento e qualidade;
- lidero times, revisão de código e definição de padrões (PEP-8, clean code, testes).


---

## Stack principal (foco em produção)
**Databricks** (Repos, Workflows, Auto Loader, MLflow) • **Apache Spark** (PySpark) • **Delta Lake** (time travel, Z-Ordering) • **Orquestração** (Airflow, DBT, Databricks Workflows) •
**AWS** (S3, EC2, IAM) • **Python/SQL** • **Kafka** • **Terraform** • **PostgreSQL** • **MongoDB** • **GitHub Actions**

<p>
  <img src="https://img.shields.io/badge/Databricks-FF3621?logo=databricks&logoColor=white"/>
  <img src="https://img.shields.io/badge/Apache%20Spark-E25A1C?logo=apachespark&logoColor=white"/>
  <img src="https://img.shields.io/badge/Delta%20Lake-00A3E0?logo=databricks&logoColor=white"/>
  <img src="https://img.shields.io/badge/Airflow-017CEE?logo=apacheairflow&logoColor=white"/>
  <img src="https://img.shields.io/badge/DBT-FF694B?logo=dbt&logoColor=white"/>
  <img src="https://img.shields.io/badge/AWS-232F3E?logo=amazonaws&logoColor=white"/>
  <img src="https://img.shields.io/badge/Kafka-231F20?logo=apachekafka&logoColor=white"/>
  <img src="https://img.shields.io/badge/Terraform-7B42BC?logo=terraform&logoColor=white"/>
  <img src="https://img.shields.io/badge/Python-3776AB?logo=python&logoColor=white"/>
  <img src="https://img.shields.io/badge/PostgreSQL-4169E1?logo=postgresql&logoColor=white"/>
  <img src="https://img.shields.io/badge/MongoDB-47A248?logo=mongodb&logoColor=white"/>
</p>

---

## Governança no Databricks (Unity Catalog, Delta Sharing & Segurança)

Trabalho com **governança ponta a ponta** no Lakehouse, alinhando **segurança, catalogação, compartilhamento e auditoria**:

- **Unity Catalog (UC)**
  - *Catálogo centralizado e RBAC*: `USE CATALOG/SCHEMA`, privilégios por **catálogo, schema, tabela, view, função, volume**.
  - *Lineage & descoberta*: linhagem de dados fim a fim, tags e classificação para PII/PHI (LGPD/GDPR).
  - *Segurança granular*: **row-level** e **column-level** via *dynamic views* (mascaração/filters por grupo).
  - *Dados gerenciados e externos*: **External Locations** + **Storage Credentials** para acesso controlado ao S3.
  - *Observabilidade nativa*: **System Tables** (acessos, consultas, compute, billing) para auditoria e custos.
- **Delta Lake**
  - *Schema enforcement & evolution*, *constraints*, *OPTIMIZE* com **Z-Order**, *Time Travel* para auditoria e recuperação.
- **Delta Sharing**
  - Compartilhamento **seguro e auditável** de tabelas/visualizações com parceiros (UC↔UC ou open recipient).
- **Controles de plataforma**
  - **Cluster/SQL Warehouse Policies**, **Secrets** (AWS Secrets Manager/Key Vault), **SCIM/SSO**, **IP access lists**.
- **Multi-ambiente**
  - Catálogos por ambiente: `edbk_dev`, `edbk_stg`, `edbk_prod` (isolamento de dados, acesso por grupos, *promotion* controlado).

<p>
  <img src="https://img.shields.io/badge/Unity%20Catalog-RBAC%20%7C%20Lineage%20%7C%20Policies-0A0?labelColor=1f2937&color=10b981"/>
  <img src="https://img.shields.io/badge/Delta%20Sharing-Secure%20Data%20Exchange-0A0?labelColor=1f2937&color=06b6d4"/>
  <img src="https://img.shields.io/badge/LGPD%20%2F%20GDPR-Privacy%20by%20Design-0A0?labelColor=1f2937&color=f59e0b"/>
</p>

### Exemplos práticos (SQL)

#### 1) Catálogos por ambiente + RBAC
```sql
-- catálogos de ambiente
CREATE CATALOG IF NOT EXISTS edbk_dev COMMENT 'Dev catalog';
CREATE CATALOG IF NOT EXISTS edbk_stg COMMENT 'Staging catalog';
CREATE CATALOG IF NOT EXISTS edbk_prod COMMENT 'Production catalog';

-- esquemas de domínio
CREATE SCHEMA IF NOT EXISTS edbk_prod.finance;
CREATE SCHEMA IF NOT EXISTS edbk_prod.risk;

-- grants mínimos
GRANT USE CATALOG ON CATALOG edbk_prod TO `grp_data_readers`;
GRANT USE SCHEMA ON SCHEMA edbk_prod.finance TO `grp_fin_readers`;
GRANT SELECT ON ALL TABLES IN SCHEMA edbk_prod.finance TO `grp_fin_readers`;
```
---

## Métricas
<div align="center">
  <img height="165" src="https://github-readme-stats.vercel.app/api/top-langs/?username=Donotavio&layout=compact&theme=radical&langs_count=8&hide=html,css" alt="Top Langs"/>
</div>

---

## Projetos & exemplos técnicos
- **Pipelines em Databricks**: notebooks e jobs para ingestão (batch/streaming), **Delta Lake** e **MLflow**.
- **Orquestração**: DAGs do **Airflow** e **Workflows** no Databricks para ELT e features de ML.
- **Boas práticas**: testes, tratamento de schema, particionamento, Z-Ordering, otimização de custos em S3/compute.

> Dica: fixe (pin) seus repositórios-chave aqui com uma frase de impacto: problema → solução → resultado (performance/custo/qualidade).

---

## Como posso ajudar
- Arquitetura **Lakehouse** (Delta Lake, Unity Catalog, governança).
- Pipelines **PySpark** performáticos e seguros.
- **Feature engineering** para ML em produção.
- Observabilidade, custo e reliability (SLAs/SLOs).

---

## Contato
<a href="mailto:ribeitemp@gmail.com">ribeitemp@gmail.com</a> •
<a href="https://www.linkedin.com/in/donotavio/">LinkedIn</a> •
