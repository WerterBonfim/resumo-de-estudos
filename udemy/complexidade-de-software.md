# Complexidade de Software

<https://www.udemy.com/course/complexidade-de-software/>

Vale a pena rever o cursos varias vezes

## Simplicidade

>"Deus está nos detalhes" "Menos é mais" \
>(Ludig mies van der rohe)

Quem não faz bem as pequenas coisas, não faz bem coisa alguma

Código é detalhamento dos requisitos de deve experssar o negócio.

Código ruim gera baixa produtividade que gera código pior.

trabalho artesanal mas profissional.

Tempestivos = que ocorre no momento certo; oportuno.

</br>

### AS 4 regras da simplicidade (Martin Fowler : Kent Beck)

Testes tempestivos
- Os testes passam

Refatoração Tempestiva
- Revela Intenção
- Nenhuma duplicação
- Mínimo de elementos

</br>

Clico da vicioso da dívida técnica

| Código Ruim                                       | Falta de Testes                                       | Procastinação                                | Pressão                                                     |
|---------------------------------------------------|-------------------------------------------------------|----------------------------------------------|-------------------------------------------------------------|
| Manutenção difícil  +retrabalho e -produtividade  | design pobre e inflexível falta de segurança p/ o dev | aversão a mudanças criação de dívida técnica | bugs, incidentes, pouco valor, baixa evolução: insatisfação |


Clico da eficácia na construção de software

| Código Limpo                                      | Testes de Unidade                                     | Refatoração                                              | Entregas c/ Valor                                                     |
|---------------------------------------------------|-------------------------------------------------------|----------------------------------------------------------|-------------------------------------------------------------|
| fácil de entender e manter. expressa o negócio    | guiando o design (feedback) com boa cobertura         | adaptação ao novo problema. tratamento de dívida técnica | evolução sustentável cliente satisfeito                     |

</br>

# Complexidade Ciclomática

Complexidade ciclomática é uma medida de quão difícil é testar uma unidade de código.

Formula para contar a complexidade ciclomatica:\
contar: if, return e &&

</br>


### Correlão 1 - Testabilidade

Quanto maior a complexidade ciclomática em um método, maior tende a ser o número de
cenários necessário em um teste deste mesmo método.

### Correlação 2 - Manutenção

Quanto maior a complexidade ciclomática em um método, maior será a
dificuldade de entendimento e o risco de inserçção de novos defeitos
neste método, aumentando o esforço de manutenção.


O número exato não é a coisa mais importante!

Complexidade ciclomática serve para acompanhamento da evolução do software 
**durante a construção**.

Premissa: Ferramenta de análise estática de código.

Até o nível 5 é rasoável.


>Gerencie como "Vazamento de Água" (Water Leak)
>"Fix Issues Before They Exist" (resolva antes de existir)
SonarQube

Utilização do plugin SonarLint


Complexidade ciclomática deve ser usada para medir a testabilidade
de um código ao logo da construção para mantê-lo simples e testável.


# Complexidade Cognitiva

