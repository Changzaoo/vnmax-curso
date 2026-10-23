# Bootstrap do Bitcoin VNMAX neste notebook (público, sem nenhum segredo)

Você é a sessão do Claude do dono, rodando neste notebook. Siga na ordem. Responda sempre em português do Brasil.
Regras: nunca misture nada da RP Líder com o Bitcoin VNMAX (pastas, processos, tarefas agendadas, logins, git). Nunca imprima a chave. Não instale nada de terceiros sem o dono confirmar.

1. **GitHub do VNMAX** (única parte que exige o clique do dono): leia e rode
   https://raw.githubusercontent.com/Changzaoo/vnmax-render/main/instalar-vnmax-github.ps1
   (`irm <url> -OutFile "$env:TEMP\i.ps1"`, leia o arquivo, depois `powershell -NoProfile -ExecutionPolicy Bypass -File "$env:TEMP\i.ps1"`).
   Ele abre o navegador em github.com/login/device e imprime um código: MOSTRE o código ao dono, que entra na conta **Changzaoo** e confirma. Se faltar o `gh`, o script avisa; só então rode de novo com `-InstalarGh`, com a confirmação do dono.
2. **Kit privado** (mods do Claude, práticas, continuidade, scripts): a chave está em `C:\Users\Usuário\render-worker-vnmax\chave.txt` e o endereço do coordenador em `C:\Users\Usuário\render-worker-vnmax\url.txt` (ou, na rede da casa, `http://192.168.0.7:8790`). Baixe `GET <endereço>/<chave>/kit` para `C:\Users\Usuário\render-worker-vnmax\kit.zip` e extraia em `...\render-worker-vnmax\kit`. Se o endereço do `url.txt` não responder, leia o atual em https://raw.githubusercontent.com/Changzaoo/vnmax-render/main/render-url.txt.
3. Leia `kit\LEIA-PRIMEIRO\CONTINUAR.md` (regras do dono, estado e pendências) e `kit\LEIA-PRIMEIRO\PROMPT-instalar-mods.md`, e execute o segundo: instala os 9 mods, as práticas e o hook, com backup do `settings.json`.
4. Termine dizendo ao dono, em 5 linhas: conta do GitHub e pasta do projeto, o que ficou instalado, o que falhou e o que ele ainda precisa fazer (por exemplo, o `/login` do Claude Code, que é dele).
