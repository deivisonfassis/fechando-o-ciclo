| #   | Regra |                              Teste | Esperado | Obitido | Resultado |
| :-- | :---: | ---------------------------------: | -------: | ------: | --------: |
| 4   | RN02  | telefone com 10 números é recusado |    false |    true |    Falhou |
|8	|RN03	|duração de 4 horas é recusada	|false	|true	|Falhou|
|10	|RN05	|futsal 17:00 às 19:00 = 180 (exemplo do documento)	|180	|160	|Falhou|
|11	|RN05	|futsal 18:00, 1 hora = 100	|100	|80	|Falhou|
12	|RN07	|futsal 18–20 e futsal 19–20, mesmo dia: conflito	|true	|false	|Falhou|





