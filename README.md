# Submissão de artigos, ORCID e Lattes (MirandasTech)

Manual em formato de slides (48) para quem vai submeter um artigo e precisa de identidade acadêmica coerente: ORCID (criar, entrar, adicionar trabalhos por DOI ou por serviços, e-mails, visibilidade, partes confiáveis — telas logadas com dados pessoais pixelados e nada alterado no registro), Currículo Lattes (cadastro, atualização e envio ao CNPq pelas FAQ oficiais, busca textual, XML exportado), escolha do periódico (Think. Check. Submit., Qualis 2017-2020 na Sucupira, DOAJ, COPE, Open policy finder, Similarity Check), sistemas de submissão (OJS, Editorial Manager, ScholarOne, o fluxo descrito pela Elsevier, um exemplo real de instruções aos autores no SciELO), checklist de submissão com a evidência de cada item (`checklist_submissao.py`), carta de apresentação com as sete declarações (`carta_apresentacao.py`), autoria CRediT, resposta ponto a ponto aos revisores (`resposta_revisores.py`), aceite, DOI e registro do artigo no ORCID e no Lattes, comparação ORCID × XML do Lattes (`orcid_lattes_diff.py`); erros comuns, checklist, glossário com popovers e referências. Capturas reais e datadas (09/09/2026); dados dos scripts ilustrativos; quem decide onde submeter e o que declarar é o conjunto de autores.

**Manual on-line:** https://submissao.mirandastech.com.br/ · **PDF:** https://submissao.mirandastech.com.br/manual.pdf

Manuais irmãos: **Manual do professor** — https://professor.mirandastech.com.br/ · **Manual do orientador** — https://orientador.mirandastech.com.br/ · **Defesa e qualificação** — https://defesa.mirandastech.com.br/ · **Ciência aberta** — https://cienciaaberta.mirandastech.com.br/ · **Bibliometria** — https://bibliometria.mirandastech.com.br/ · **Análise de dados** — https://dados.mirandastech.com.br/ · **Git e GitHub** — https://git.mirandastech.com.br/ · **LaTeX** — https://latex.mirandastech.com.br/ · **Busca em bases** — https://busca.mirandastech.com.br/ · **Revisão sistemática com PRISMA 2020** — https://prisma.mirandastech.com.br/ · **Zotero** — https://zotero.mirandastech.com.br/ · **Metodologia** — https://metodologia.mirandastech.com.br/ · **Gemini Notebook** — https://notebook.mirandastech.com.br/ · **Uso de IA na pesquisa** — https://manual.mirandastech.com.br/ · **Plugin Pesquisa** — https://plugin.mirandastech.com.br/ · Hub: https://www.mirandastech.com.br/pesquisa

| Pasta | O que há |
|---|---|
| `manual/` | deck HTML autônomo, PDF, fonte do artefato e `fatos_verificados.md` (fontes e execuções conferidas em 09/09/2026) |
| `site/` | o que o servidor serve (`index.html`, `manual.pdf`) |
| `capturas/` | 32 capturas reais, 09/09/2026 (21 páginas públicas sem login; 7 telas logadas do ORCID com dados pessoais pixelados; 4 figuras de terminal com saídas reais e dados ilustrativos) |
| `scripts/checklist_submissao.py` | checklist de submissão em quatro momentos, com a evidência de cada item |
| `scripts/carta_apresentacao.py` | carta de apresentação (pt/en) com as sete declarações |
| `scripts/resposta_revisores.py` | tabela ponto a ponto a partir do texto da decisão editorial |
| `scripts/orcid_lattes_diff.py` | compara os trabalhos públicos do ORCID com os artigos do XML do Lattes (não altera nada) |
| `scripts/gerar_deck.py` | regenera HTML e PDF a partir do fonte |
| `skills/submissao-orcid-lattes/` | skill do agente (cópia sincronizada do plugin Pesquisa MirandasTech) |
| `Dockerfile` · `Caddyfile` · `railway.json` | deploy estático (Caddy) |
| `.github/workflows/verificar.yml` | CI: integridade do deck e capturas referenciadas |

## Os manuais juntos
Este manual fecha o ciclo da série: o texto sai do manual de LaTeX, a autoria e o acordo vêm do Manual do orientador, o depósito com DOI vem do manual de Ciência aberta, e aqui o artigo é submetido, revisado, publicado e registrado no ORCID e no Lattes. A skill `submissao-orcid-lattes` do plugin **Pesquisa MirandasTech** gera o checklist, a carta e a resposta aos revisores e compara os dois registros — o aluno submete e atualiza na conta dele; nenhuma credencial passa pelo agente.

## Como citar
MATIAS, J. P. M. *Submissão de artigos, ORCID e Lattes.* MirandasTech, v1.0, set. 2026. CC BY 4.0.

## Declaração de uso de IA
Escrito com assistência de IA (Claude, Anthropic) na estruturação, redação, automação das capturas e execução dos scripts. Fatos conferidos em páginas públicas e na API pública da ORCID em 09/09/2026 (lista em `manual/fatos_verificados.md`). As telas logadas do ORCID foram capturadas com autorização do titular da conta, com nome, iD, e-mails e afiliação pixelados, e nada foi alterado no registro; não há telas logadas do Lattes. O autor responde integralmente pelo conteúdo. ORCID, CNPq, CAPES, gov.br, SciELO, PKP, Aries Systems, Clarivate, Elsevier, Think. Check. Submit., DOAJ, COPE, Crossref, Jisc, NISO e Google são marcas, órgãos e projetos de terceiros; este manual não tem vínculo com eles.
