<div align="center">

  <img src="https://capsule-render.vercel.app/api?type=waving&color=0:0f172a,100:0284c7&height=200&section=header&text=Brandon%20Mendieta&fontSize=42&fontColor=ffffff&fontAlignY=38&desc=DevOps%20Engineer%20%7C%20Fintech%20%7C%20Kubernetes&descColor=ffffff&descAlignY=62&descAlign=50" width="100%" alt="Header Banner" />

  <p align="center">
    <a href="https://www.linkedin.com/in/brandon-alexander-mendieta-suarez-15a14619b/">
      <img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn" />
    </a>
    <a href="mailto:brandon7127329@gmail.com">
      <img src="https://img.shields.io/badge/Email-D14836?style=for-the-badge&logo=gmail&logoColor=white" alt="Email" />
    </a>
    <a href="https://github.com/NeoScraids">
      <img src="https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white" alt="GitHub" />
    </a>
    <img src="https://komarev.com/ghpvc/?username=NeoScraids&base=1000&color=0ea5e9&style=for-the-badge&label=VIEWS" alt="Profile Views" />
  </p>

</div>

---

### Sobre mi

Ingeniero DevOps trabajando en el sector **Fintech**. Mi dia a dia gira alrededor de mantener estables los clusters de **Kubernetes en OKE** (Oracle Cloud), armar pipelines de CI/CD en **Azure DevOps**, y asegurarme de que los despliegues a produccion sean predecibles y reversibles con **ArgoCD**.

Llevo un tiempo metido en el tema de observabilidad con el stack de Grafana (Tempo, Loki, Mimir, Alloy) y OpenTelemetry. La idea es siempre la misma: que cuando algo falle a las 3am, puedas ir de la metrica al log y a la traza sin tener que adivinar nada.

Ultimamente he estado experimentando con servidores MCP y agentes con LiteLLM + Bedrock para automatizar partes del proceso de respuesta a incidentes. Los proyectos que ves aca son versiones limpias (sin datos corporativos) de cosas que he armado o que quiero probar.

---

### Stack

<p align="left">
  <img src="https://img.shields.io/badge/OCI-F80000?style=flat-square&logo=oracle&logoColor=white" alt="OCI" />
  <img src="https://img.shields.io/badge/Kubernetes-326CE5?style=flat-square&logo=kubernetes&logoColor=white" alt="Kubernetes" />
  <img src="https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white" alt="Docker" />
  <img src="https://img.shields.io/badge/Terraform-7B42BC?style=flat-square&logo=terraform&logoColor=white" alt="Terraform" />
  <img src="https://img.shields.io/badge/Ansible-EE0000?style=flat-square&logo=ansible&logoColor=white" alt="Ansible" />
  <img src="https://img.shields.io/badge/ArgoCD-EF7B4D?style=flat-square&logo=argo&logoColor=white" alt="ArgoCD" />
  <img src="https://img.shields.io/badge/Azure_DevOps-0078D7?style=flat-square&logo=azure-devops&logoColor=white" alt="Azure DevOps" />
  <img src="https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white" alt="Python" />
  <img src="https://img.shields.io/badge/Bash-4EAA25?style=flat-square&logo=gnu-bash&logoColor=white" alt="Bash" />
  <img src="https://img.shields.io/badge/OpenTelemetry-000000?style=flat-square&logo=opentelemetry&logoColor=white" alt="OpenTelemetry" />
  <img src="https://img.shields.io/badge/Grafana-F46800?style=flat-square&logo=grafana&logoColor=white" alt="Grafana" />
  <img src="https://img.shields.io/badge/Prometheus-E6522C?style=flat-square&logo=prometheus&logoColor=white" alt="Prometheus" />
</p>

---

### Proyectos

Los repos de aca son implementaciones de referencia. No es codigo de produccion de la empresa (obvio), pero si reflejan los problemas que resuelvo en el dia a dia.

| Repo | De que va |
| :--- | :--- |
| [mcp-k8s-observability](https://github.com/NeoScraids/mcp-k8s-observability) | Servidor MCP en Python que le permite a un agente de IA consultar pods de K8s, hacer queries PromQL y buscar logs en Loki. Tiene modo mock para probarlo sin cluster. |
| [bedrock-incident-copilot](https://github.com/NeoScraids/bedrock-incident-copilot) | Agente con LiteLLM + Bedrock que recibe una alerta (tipo Alertmanager), analiza metricas/logs y genera un runbook con los comandos de remediacion. Incluye simulador de incidentes. |
| [otel-microservice-blueprint](https://github.com/NeoScraids/otel-microservice-blueprint) | Microservicio en FastAPI instrumentado con OpenTelemetry. Exporta trazas, metricas y logs con `trace_id` inyectado para correlacion en Grafana. Incluye generador de carga. |
| [observability-lgtm-stack](https://github.com/NeoScraids/observability-lgtm-stack) | Docker Compose con Grafana + Mimir + Tempo + Loki + Alloy + Prometheus, listo para levantar. Manifiestos de Alloy como DaemonSet en OKE y script para crear dashboards automaticamente. |
| [k8s-gitops-catalog](https://github.com/NeoScraids/k8s-gitops-catalog) | Manifiestos de K8s con NetworkPolicy, HPA, PDB y app de ArgoCD. Basado en patrones que uso para microservicios financieros. |
| [devops-pipeline-templates](https://github.com/NeoScraids/devops-pipeline-templates) | Workflows reutilizables de GitHub Actions: build con Buildx, escaneo con Trivy, validacion de Terraform y sync de tags a repos GitOps. |
| [sre-health-inspector](https://github.com/NeoScraids/sre-health-inspector) | CLI en Python para verificar certificados SSL, medir latencia HTTP y probar conectividad TCP. Lo uso como health check rapido. |
| [infra-as-code](https://github.com/NeoScraids/infra-as-code) | Modulos de Terraform para VPC, subredes, gateways y security groups en AWS. |
| [Portal-Devops](https://github.com/NeoScraids/Portal-Devops) | Portal interno en Next.js para operaciones de despliegue y monitoreo. |
| [ansible-logs-archiver](https://github.com/NeoScraids/ansible-logs-archiver) | Playbook de Ansible para rotacion y archivado de logs en servidores Linux. |
| [bash-utils](https://github.com/NeoScraids/bash-utils) | Scripts de Bash para diagnostico de servidores, salud de servicios y checklists operativos. |

---

<div align="center">
  <img src="https://streak-stats.demolab.com/?user=NeoScraids&theme=tokyonight&hide_border=true&date_format=j%20M%5B%20Y%5D" alt="GitHub Streak Stats" />
</div>

---

<div align="center">
  <p>
    <a href="https://www.linkedin.com/in/brandon-alexander-mendieta-suarez-15a14619b/">
      <img src="https://img.shields.io/badge/LinkedIn-Brandon_Mendieta-0A66C2?style=flat-square&logo=linkedin&logoColor=white" alt="LinkedIn" />
    </a>
    &nbsp;&nbsp;
    <a href="mailto:brandon7127329@gmail.com">
      <img src="https://img.shields.io/badge/Email-brandon7127329@gmail.com-D14836?style=flat-square&logo=gmail&logoColor=white" alt="Email" />
    </a>
  </p>
</div>
