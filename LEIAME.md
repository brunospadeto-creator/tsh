# Material do artigo "Detecção de erros e localização de causas em microsserviços com métricas por serviço e limiares calibrados na baseline"

Bruno Spadeto e Diego de Castro Rodrigues (Universidade Federal do Tocantins; Instituto Federal do Tocantins).

| arquivo | conteúdo |
|---|---|
| `deposito-g-m-t-k-20261029-f2367f37.zip` | código do método, adaptadores das bases, scripts de avaliação, de robustez e das análises adicionais, comparadores, script das figuras, protocolo registrado, emendas, código congelado no registro, cronologia dos commits, relatórios de resultado, ambiente travado e script de reprodução. O `LEIAME.md` de dentro explica a estrutura e como reproduzir. |
| `2-evidencias.tar.gz` | evidências derivadas: registros por instante e artefatos por caso, escores e caches que as tabelas do artigo leem, saídas dos comparadores |
| `SHA256SUMS` | sha256 dos dois arquivos acima (`sha256sum -c SHA256SUMS`) |

A telemetria bruta do TeaStore (10 arquivos, 1,4 GB) está só no Zenodo, com os dois arquivos acima, porque passa do
limite de tamanho por arquivo do GitHub: DOI [a definir].

Os dados públicos (RCAEval e OpenRCA Market) não estão aqui; baixe-os dos repositórios dos autores, citados no artigo.

Licença (proposta): código sob MIT; documentos e resultados sob CC BY 4.0.

Atualização de 29/10/2026: parte 1 remontada no commit `09bb0709`, incluindo a ablação da normalização no portão. ZIP e checksums internos verificados; 170 arquivos Python compiláveis e AST dos 164 arquivos Python correntes idêntica à do commit, sem docstrings. Evidências derivadas preservadas.

Atualização de 29/10/2026 (tarde): parte 1 remontada no commit `376bb4f8`. Em relação ao pacote anterior, mudam só o `NOMES.md` (nomes atualizados das medidas: Top-1 forçado e proporção líquida de vitórias por caso) e o hash citado na `CRONOLOGIA.md`; código e resultados são os mesmos. ZIP e checksums internos verificados.

Atualização de 29/10/2026 (noite): parte 1 remontada no commit `f2367f37`, depois de uma auditoria do artefato. O `LEIAME.md` de dentro do pacote ganhou instruções para usar a parte 2 e refazer a robustez, as convenções das janelas, a descrição de como o replay reconstrói os eventos do Kubernetes (com uma análise de sensibilidade) e o sha256 dos dados públicos usados (`bases-externas/reproducao/dados-publicos-SHA256SUMS`). Código e resultados são os mesmos do pacote anterior.
