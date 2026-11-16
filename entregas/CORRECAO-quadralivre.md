# Registro de correção — QuadraLivre

**Grupo:** 1 **Integrantes:** Deivison, Denyver, Kayo, Kauan, Andreson, Pedro Henrique

## Antes de corrigir

Testes automatizados (`apps/quadralivre/testes/testes.html`): 9 de 14 passando.
Testes que falham:

## Correções

| Issue | Regra | Função e arquivo | Causa (linha errada) | Correção (linha nova) | Commit | Teste que prova |
| --- | --- | --- | --- | --- | --- | --- |
| # | RN02 | app.js - Validar Telefone |  return digitos.length >= 10 && digitos.length <= 11; |  return digitos.length > 10 && digitos.length <= 11; | `fix: Reservas somem depois de recarregar a página closes #4` | |
| # | RN03 | app.js - ValidarHorario | if (duracao < 1 or duracao > 4) return false; | if (duracao < 1 or duracao >= 4) return false; | `fix: Reserva de 4 horas é aceita #3` | |
| # | RN05 | app.js - valorReserva | total += hora > 18 ? base * 1.25 : base; | total += hora >= 18 ? base * 1.25 : base; | `fix: Horário nobre não é cobrado na hora das 18:00 closes #2` | |
| # | RN05 | app.js - valorReserva | total += hora > 18 ? base * 1.25 : base; | total += hora >= 18 ? base * 1.25 : base; | `fix: Horário nobre não é cobrado na hora das 18:00 closes #2` | |
| # | RN05 | app.js - valorReserva | total += hora > 18 ? base * 1.25 : base; | total += hora >= 18 ? base * 1.25 : base; | `fix: Horário nobre não é cobrado na hora das 18:00 closes #2` | |
| # | RN07 | app.js - temComflito | r.inicio === nova.inicio | nova.inicio < r.inicio + r.duracao && nova.inicio + nova.duracao > r.inicio | `fix: Duas reservas sobrepostas na mesma quadra são aceitas closes #3`| |



## Depois de corrigir

Testes automatizados: 14 de 14 passando.
Persistência (F5) conferida à mão: sim / não (print):
Alguma correção quebrou outro teste? Qual, e o que fizeram?

## Rastreabilidade

Para cada Issue, o caminho completo: Issue → commit → teste.
