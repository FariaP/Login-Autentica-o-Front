Projeto desenvolvido como forma de exercicio e prática da disciplina de programação para internet.

Seu objetivo é Desenvolver uma aplicação web simples, utilizando HTML, CSS e JavaScript puro, 
que permita o cadastro de usuários com foco em: Validação de formulários via estruturas condicionais (if/else) e expressões regulares (REGEX).

Sua etrutura é basicamente formada por:

Nome Completo:
Obrigatório.
Mínimo de 3 caracteres.

CPF:
Obrigatório.
Validar formato com REGEX: 000.000.000-00.
Exemplo: /^\d{3}\.\d{3}\.\d{3}-\d{2}$/.
(Opcional avançado) Validar dígitos verificadores pelo algoritmo oficial.

Login:
Obrigatório.
Mínimo de 4 caracteres.
Permitir apenas letras, números e símbolos ., _,-.
REGEX sugerido: /^[A-Za-z0-9.-]{4,}$/.

E-mail:
Obrigatório.
Validar formato com REGEX simples, ex.:
/^[^\s@]+@[^\s@]+\.[^\s@]{2,}$/.

Senha:
Obrigatória.
Mínimo de 8 caracteres.
Deve conter pelo menos 1 letra e 1 dígito.
REGEX sugerido: /^(?=.*[A-Za-z])(?=.*\d).{8,}$/.

Confirmação de Senha:
Obrigatória.
Deve ser idêntica à senha digitada.

Salário:
Obrigatório.
Valor numérico maior que zero.
Número de Dependentes
Obrigatório.
Inteiro maior ou igual a zero.


Cálculo do Imposto de Renda (IR):
O cálculo do IR deve acontecer somente após o usuário sair do
campo “Número de Dependentes” (evento blur).
Base de cálculo = Salário – (R$ 200 × Número de Dependentes).
Se o resultado for negativo, usar 0.
Aplicar alíquota única por faixa sobre a base:
Arredondar o resultado para duas casas decimais.
Exibir o valor no campo IR (somente leitura).
