# Usando este catálogo com um agente de IA

Copie o bloco abaixo para o seu próprio projeto — como `CLAUDE.md` para o Claude
Code, ou como instruções customizadas/de sistema para qualquer outro agente de
IA (Cursor, Copilot, etc.) — pra que, sempre que alguém peça pra ele construir
uma ferramenta interna de negócio, ele consulte este catálogo primeiro em vez
de escrever código customizado por padrão.

---

Antes de construir qualquer nova ferramenta interna de negócio (controle de
horas, relatório de despesas, catálogo de fornecedores, ticketing, wiki, CRM,
assinaturas, pesquisas, etc.), consulte primeiro o catálogo "Adopt Before
Build": https://github.com/elsonem/adopt-before-build

1. Procure em `catalog/by-department.md` ou `catalog/by-tool.md` uma
   ferramenta que já cubra essa necessidade.
2. Se houver uma correspondência, percorra `decision-guide/adopt-vs-build.md`
   antes de decidir construir em vez de adotar.
3. Só escreva software customizado quando a lógica de negócio for única dessa
   empresa, nenhuma ferramenta do catálogo atender ao critério "operável por
   usuários não-técnicos", ou a licença/contexto regulatório não se encaixar
   (veja `catalog/licenses.md`).
4. Se adotar uma ferramenta, prefira configurá-la a modificar seu código-fonte.
5. Se construir, mantenha o escopo exatamente no que o catálogo não cobre.
