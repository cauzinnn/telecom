# Handoff: Apresentação "Do Sulco ao Som" (Telecomunicações no Vinil)

## Contexto do Projeto
- **Curso:** Engenharia de Computação e Informação
- **Disciplina:** Princípios de Telecomunicações
- **Formato:** Apresentação acadêmica (não usar o termo "seminário")
- **Arquivo Principal:** `C:\Users\gpnob\Downloads\f\t\telecom-no-vinil.html`
- **Duração Estimada:** 18 minutos no total
- **Padrão de Design:** *Cobalt Grid* (baseado no `bold-template-pack` de `frontend-slides`)
  - Paleta: Papel creme (`#F0EBDE`), tinta azul cobalto (`#1F2BE0`), grid milimetrado sutil (8-10%)
  - Tipografia: Newsreader (display serif 400), Hanken Grotesk (sans 400/600), DM Mono (chrome/dados)
  - Modelo: Fixed 16:9 Stage (1920×1080) com auto-scale para o viewport

---

## Estrutura da Apresentação (13 Slides)
1. **Slide 1 — Capa:** Título de impacto (*Do Sulco ao Som*), curso, metadados e cartão de especificações de canal.
2. **Slide 2 — Introdução:** O gancho do vinil como canal de transmissão de informação física pura.
3. **Slide 3 — Topologia:** Modelo de Shannon aplicado ao vinil (diagrama de blocos em SVG).
4. **Slide 4 — Transdução e Fabricação:** Força de Lorentz, micrômetros de sulco, laca e prensagem térmica.
5. **Slide 5 — Modulação 45°/45°:** Modulação em quadratura no plano espacial, compatibilidade mono $(L+R)$ e estéreo $(L-R)$ com diagrama em corte transversal.
6. **Slide 6 — Dilema Físico:** Relação deslocamento vs. frequência ($x \propto 1/f$), invasão de sulco por graves e ruído térmico em agudos.
7. **Slide 7 — Curva RIAA:** Filtro de pré-ênfase (gravação) e de-ênfase (reprodução) com gráfico SVG de resposta simétrica.
8. **Slide 8 — Limites de Canal:** Velocidade linear variável ($v = \omega \cdot r$), distorção no miolo (*Inner Groove Distortion*) e SNR (~55–65 dB).
9. **Slide 9 — Analógico vs. Digital:** Limites físicos reais do vinil vs. Teorema de Nyquist-Shannon (desmistificação da "escadinha").
10. **Slide 10 — Mitos e Verdades (Parte 1):** Tabela analisando som infinito, som "quente" (distorção harmônica) e degraus digitais.
11. **Slide 11 — Mitos e Verdades (Parte 2):** Desgaste físico a cada leitura, cabos banhados a ouro e padronização da RIAA (1954).
12. **Slide 12 — Conclusão Técnica:** Lições universais de telecomunicações (condicionamento de meio, compromisso de Shannon, padrões abertos).
13. **Slide 13 — Encerramento:** Reflexão sobre a experiência humana/música e abertura para perguntas (Q&A).

---

## Decisões Recentes e Ajustes Aplicados
- **Densidade:** Reduzida para *speaker-led* (baixa densidade), priorizando frases de impacto, diagramas e bullets curtos.
- **Tipografia:** Tamanhos aumentados para legibilidade em projeção/auditório (títulos em 74px/116px, corpo entre 24px e 32px).
- **Sem Minutos:** Removidas todas as marcações de tempo em minutos dos cabeçalhos.
- **Interface Limpa:** A barra flutuante de navegação foi oculta por padrão (`opacity: 0`), aparecendo apenas ao passar o mouse perto do rodapé.
- **Edição Inline:** Ativada e desativada a qualquer momento pressionando a tecla `E` no teclado (salvamento via `Ctrl+S`).
- **Nomenclatura:** Substituídas todas as menções de "seminário" por "apresentação".

---

## Próximos Passos Sugeridos
1. **Compartilhamento / Exportação:**
   - Deploy para link público via Vercel usando o script do skill: `bash scripts/deploy.sh telecom-no-vinil.html`.
   - Exportação para PDF com Playwright: `bash scripts/export-pdf.sh telecom-no-vinil.html`.
2. **Ajustes de Conteúdo:** Refinamento de tópicos específicos ou inclusão de notas de orador se solicitado pelo usuário.

---

## Suggested Skills
- **`frontend-slides`**: Localizado em `C:\Users\gpnob\.agents\skills\frontend-slides\plugins\frontend-slides\skills\frontend-slides`. Utilizar para manutenções na apresentação, exportação para PDF (`scripts/export-pdf.sh`) ou publicação em URL pública (`scripts/deploy.sh`).
- **`code-review`**: Se for necessário auditar conformidade de padrões ou acessibilidade do HTML/CSS gerado.
