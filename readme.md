# SMART-DS Network Analysis

Ferramenta de análise e visualização para os datasets sintéticos de redes elétricas de distribuição SMART-DS utilizando OpenDSS e Python.

---

## Visão Geral

Este repositório foi criado para explorar e analisar os datasets SMART-DS disponibilizados pela Open Energy Data Initiative (OEDI).

O projeto tem foco em:

- Análise de redes elétricas de distribuição
- Inspeção de feeders e subestações
- Análise de séries temporais de carga
- Estudos de tensão e sobrecarga
- Simulações com OpenDSS
- Visualização de dados
- Experimentação em smart grids

Os datasets SMART-DS são modelos sintéticos, porém altamente realistas, de redes elétricas baseados em estatísticas e comportamentos operacionais de concessionárias reais dos Estados Unidos.

---

## Principais Regiões

| Região | Descrição |
|---|---|
| AUS | Austin, Texas |
| GSO | Greensboro, Carolina do Norte |
| SFO | San Francisco, Califórnia |

---


### Cenários de Solar

| Cenário | Significado |
|---|---|
| solar_none | Sem geração solar |
| solar_low | Baixa penetração solar |
| solar_medium | Média penetração solar |
| solar_high | Alta penetração solar |
| solar_extreme | Penetração solar extrema |

### Cenários de Baterias

| Cenário | Significado |
|---|---|
| batteries_none | Sem baterias |
| batteries_low | Baixa adoção de baterias |
| batteries_high | Alta adoção de baterias |

Exemplo:

```text
solar_high_batteries_low_timeseries/
```

Significa:

- Alta geração solar
- Baixa adoção de baterias

---

## Fonte dos Dados

Os datasets SMART-DS estão disponíveis publicamente através da Open Energy Data Initiative (OEDI).

AWS S3 público:

```bash
aws s3 ls --no-sign-request s3://oedi-data-lake/SMART-DS/
```
