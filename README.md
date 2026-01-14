<div align="center">
  <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=600&size=24&duration=2800&pause=600&center=true&vCenter=true&width=520&lines=Oi%2C+eu+sou+o+Ot%C3%A1vio+Ribeiro;Data+Engineering+Manager+%40+Educbank;Databricks+%7C+Spark+%7C+Delta+Lake+%7C+Governan%C3%A7a" alt="typing intro"/>
</div>

<p align="center">
  <a href="https://github.com/Donotavio">
    <img src="https://visitor-badge.laobi.icu/badge?page_id=Donotavio" alt="visits"/>
  </a>
  <a href="https://wakatime.com/@ee59639e-06da-4c79-af0f-2be09bc8780a">
    <img src="https://wakatime.com/badge/user/ee59639e-06da-4c79-af0f-2be09bc8780a.svg" alt="WakaTime"/>
  </a>
  <a href="https://www.linkedin.com/in/donotavio/">
    <img src="https://img.shields.io/badge/LinkedIn-Conecte-se-blue?logo=linkedin" alt="LinkedIn"/>
  </a>
</p>

<p align="center">
  <img src="https://github-profile-trophy.vercel.app/?username=Donotavio&theme=radical&no-frame=true&no-bg=true&title=Experience,Repositories,Stars" alt="GitHub Trophies"/>
</p>

<div align="center">
  <a href="mailto:ribeitemp@gmail.com">
    <img src="https://img.shields.io/badge/Falar%20sobre-Databricks%20%7C%20Governan%C3%A7a%20%7C%20Streaming-10b981?style=for-the-badge" alt="CTA"/>
  </a>
</div>

---

## Em poucas linhas

Sou **Gerente de Engenharia de Dados na Educbank** (fintech) e uso **Databricks como feature platform** para unificar pipelines, modelagem com **Delta Lake** e **workflows de ML**. No dia a dia:

- desenho e otimizo pipelines batch/streaming (custo, performance e confiabilidade);
- garanto governança & compliance (**LGPD/GDPR**), versionamento e qualidade;
- lidero times, revisão de código e definição de padrões (PEP-8, clean code, testes).

<p align="center">
  <img src="https://img.shields.io/badge/Databricks-Lakehouse-red?style=for-the-badge&logo=databricks&logoColor=white"/>
  <img src="https://img.shields.io/badge/Spark-PySpark-orange?style=for-the-badge&logo=apachespark&logoColor=white"/>
  <img src="https://img.shields.io/badge/Delta%20Lake-Governan%C3%A7a-blue?style=for-the-badge&logo=databricks&logoColor=white"/>
  <img src="https://img.shields.io/badge/Orquestra%C3%A7%C3%A3o-Airflow%20%7C%20DBT-lightblue?style=for-the-badge&logo=apacheairflow&logoColor=white"/>
  <img src="https://img.shields.io/badge/Cloud-AWS%20%7C%20Azure-purple?style=for-the-badge&logo=cloudflare&logoColor=white"/>
</p>

---

## Minhas principais responsabilidades

✨ **Lakehouse governado**: uso **Unity Catalog + Delta Lake** para segurança, lineage, tags de PII e trilha de auditoria.
🚀 **Pipelines resilientes**: batch/streaming com **Auto Loader**, **Z-Ordering**, particionamento, custos otimizados e SLOs claros.
🤝 **Liderança técnica**: definindo padrões, mentorando squads e garantindo revisões que equilibram velocidade e qualidade.
🔒 **Compliance**: políticas de acesso, masking (row/column) e segregação multi-ambiente (`dev/stg/prod`).

---

## Stack de produção

**Databricks** (Repos, Workflows, Auto Loader, MLflow) • **Apache Spark** (PySpark) • **Delta Lake** (time travel, Z-Ordering) • **Orquestração** (Airflow, DBT, Databricks Workflows) • **AWS** (S3, EC2, IAM) • **Azure** (ADLS Gen2, Event Hubs*Kafka API*, Key Vault, Synapse/SQL, Managed Identity) • **Python/SQL** • **Kafka** • **Terraform** • **PostgreSQL** • **MongoDB** • **GitHub Actions**

<p>
  <img src="https://img.shields.io/badge/Databricks-FF3621?logo=databricks&logoColor=white"/>
  <img src="https://img.shields.io/badge/Apache%20Spark-E25A1C?logo=apachespark&logoColor=white"/>
  <img src="https://img.shields.io/badge/Delta%20Lake-00A3E0?logo=databricks&logoColor=white"/>
  <img src="https://img.shields.io/badge/Airflow-017CEE?logo=apacheairflow&logoColor=white"/>
  <img src="https://img.shields.io/badge/DBT-FF694B?logo=dbt&logoColor=white"/>
  <img src="https://img.shields.io/badge/AWS-232F3E?logo=amazonaws&logoColor=white"/>
  <img src="https://img.shields.io/badge/Azure-0089D6?logo=microsoftazure&logoColor=white"/>
  <img src="https://img.shields.io/badge/Kafka-231F20?logo=apachekafka&logoColor=white"/>
  <img src="https://img.shields.io/badge/Terraform-7B42BC?logo=terraform&logoColor=white"/>
  <img src="https://img.shields.io/badge/Python-3776AB?logo=python&logoColor=white"/>
  <img src="https://img.shields.io/badge/PostgreSQL-4169E1?logo=postgresql&logoColor=white"/>
  <img src="https://img.shields.io/badge/MongoDB-47A248?logo=mongodb&logoColor=white"/>
  <img src="https://img.shields.io/badge/GitHub%20Actions-2088FF?logo=githubactions&logoColor=white"/>
</p>

---

## Governança no Databricks

Trabalho com **governança ponta a ponta** no Lakehouse, alinhando **segurança, catalogação, compartilhamento e auditoria**:

- **Unity Catalog (UC)**
  - Catálogo centralizado e RBAC por catálogo/schema/tabela/view/função/volume.
  - Lineage fim a fim, tags e classificação para PII/PHI (LGPD/GDPR).
  - Segurança granular: **row-level** e **column-level** via *dynamic views* (masking/filters por grupo).
  - External Locations + Storage Credentials para acesso controlado a S3.
  - Observabilidade: **System Tables** (acessos, consultas, compute, billing) para auditoria/custos.
- **Delta Lake**
  - Schema enforcement & evolution, constraints, **OPTIMIZE** com **Z-Order**, *Time Travel* para auditoria/rollback.
- **Delta Sharing**
  - Compartilhamento **seguro e auditável** de tabelas/visualizações com parceiros (UC↔UC ou open recipient).
- **Controles de plataforma**
  - Cluster/SQL Warehouse Policies, Secrets (AWS Secrets Manager/Key Vault), SCIM/SSO, IP access lists.
- **Multi-ambiente**
  - Catálogos por ambiente: `edbk_dev`, `edbk_stg`, `edbk_prod` (isolamento, acesso por grupos, promotion controlado).

<p>
  <img src="https://img.shields.io/badge/Unity%20Catalog-RBAC%20%7C%20Lineage%20%7C%20Policies-0A0?labelColor=1f2937&color=10b981"/>
  <img src="https://img.shields.io/badge/Delta%20Sharing-Secure%20Data%20Exchange-0A0?labelColor=1f2937&color=06b6d4"/>
  <img src="https://img.shields.io/badge/LGPD%20%2F%20GDPR-Privacy%20by%20Design-0A0?labelColor=1f2937&color=f59e0b"/>
</p>

### Exemplo prático (SQL)

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

## Projetos & exemplos técnicos

- **Pipelines em Databricks**: notebooks e jobs para ingestão (batch/streaming), **Delta Lake** e **MLflow**.
- **Orquestração**: DAGs do **Airflow** e **Workflows** no Databricks para ELT e features de ML.
- **Boas práticas**: testes, tratamento de schema, particionamento, Z-Ordering, otimização de custos em S3/compute.

> Dica: fixe (pin) seus repositórios-chave aqui com uma frase de impacto: problema → solução → resultado (performance/custo/qualidade).

---

## Métricas

<div align="center">
  <img height="165" src="https://github-readme-stats.vercel.app/api/top-langs/?username=Donotavio&layout=compact&theme=radical&langs_count=8&hide=html,css" alt="Top Langs"/>
</div>

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
