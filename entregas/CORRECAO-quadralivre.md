# Registro de correção — QuadraLivre

**Grupo:** 1 **Integrantes:** Deivison, Denyver, Kayo, Kauan, Andreson, Pedro Henrique

## Antes de corrigir

Testes automatizados (`apps/quadralivre/testes/testes.html`): 9 de 14 passando.
Testes que falham:

## Correções

| Issue | Regra | Função e arquivo | Causa (linha errada) | Correção (linha nova) | Commit | Teste que prova |
| --- | --- | --- | --- | --- | --- | --- |
| # | RN02 | app.js - Validar Telefone |  return digitos.length >= 10 && digitos.length <= 11; |  return digitos.length > 10 && digitos.length <= 11; | `fix: Reservas somem depois de recarregar a página closes #4` | |



## Depois de corrigir

Testes automatizados: 14 de 14 passando.
Persistência (F5) conferida à mão: sim / não (print):
Alguma correção quebrou outro teste? Qual, e o que fizeram?

## Rastreabilidade

Para cada Issue, o caminho completo: Issue → commit → teste.
