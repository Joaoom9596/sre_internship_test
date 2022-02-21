# sre_internship_test

Desenvolva uma solução que vasculhe e agrupe os logs do QB Render por paths e taxas de sucesso e erro.

A solução consiste de dois scripts, um em Posix Shell, `process`, e outro em AWK, `count`.

`process` filtra e formata os logs para que a interpretação seja mais facil - remove informações não importantes para a solução, remove caracteres de formatação e organiza em colunas separadas por `\t`.

`count` recebe a saída formatada de `process` e gera 3 arrays, uma para paths, e as outras duas para contagem dos statusCodes; no final da execução formata a saída em JSON e imprime.
