
# CodeCanvaZ

**CodeCanvaZ** é um módulo Python simples que oferece uma classe `Styles` para facilitar a formatação de textos em terminais utilizando códigos de escape ANSI. Com ele, você pode facilmente adicionar cores de fundo, cores de texto, negrito e sublinhado às suas saídas no terminal.

## Versão

A versão atual do projeto é **1.0.0**.

## Instalação

Não há necessidade de instalação adicional. Basta copiar o arquivo `codecanvaz.py` para o seu projeto e importar a classe `Styles` no seu código.

## Uso

Veja abaixo como utilizar a classe `Styles` para formatar o texto:

```python
from codecanvaz import Styles

style = Styles()

print(f"{style.f_blue}{style.bold}Este texto é azul e em negrito{style.reset}")
print(f"{style.b_red}{style.f_white}Texto branco com fundo vermelho{style.reset}")
print(f"{style.underline}{style.f_green}Texto sublinhado em verde{style.reset}")
```

## Estilos Disponíveis

### Cores de Texto

- **f_black**: `\033[30m`
- **f_red**: `\033[31m`
- **f_green**: `\033[32m`
- **f_yellow**: `\033[33m`
- **f_blue**: `\033[34m`
- **f_magenta**: `\033[35m`
- **f_cyan**: `\033[36m`
- **f_white**: `\033[37m`

### Cores de Fundo

- **b_black**: `\033[40m`
- **b_red**: `\033[41m`
- **b_green**: `\033[42m`
- **b_yellow**: `\033[43m`
- **b_blue**: `\033[44m`
- **b_magenta**: `\033[45m`
- **b_cyan**: `\033[46m`
- **b_white**: `\033[47m`

### Estilos de Texto

- **bold**: `\033[1m` (Negrito)
- **underline**: `\033[4m` (Sublinhado)
- **reset**: `\033[0m` (Resetar todas as formatações)

## Licença

Este projeto está licenciado sob a Licença MIT. Veja o arquivo [LICENSE](LICENSE) para mais detalhes.
