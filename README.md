# Padrões de Projeto - Exemplos

Implementações didáticas, em Python, de padrões de projeto (*design patterns*) do catálogo GoF. Cada padrão é um módulo independente, com código comentado em português e com o diagrama de classes correspondente.

## O que está incluso?

Cada padrão possui três arquivos, com o mesmo nome:

- `.py`: o código, com comentários explicando o papel de cada classe
- `.asta`: o diagrama de classes, editável no [Astah](https://astah.net/)
- `.pdf`: o diagrama de classes exportado

### Criacionais (`creational/`)

| Módulo | Padrão |
|---|---|
| `abstract_factory` | Abstract Factory |
| `builder` | Builder |
| `factory_method` | Factory Method |
| `prototype` | Prototype |
| `singleton` | Singleton (incluindo uso com múltiplas *threads*) |

### Estruturais (`structural/`)

| Módulo | Padrão |
|---|---|
| `bridge` | Bridge |
| `class_adapter` | Adapter, versão de classe (herança) |
| `object_adapter` | Adapter, versão de objeto (composição) |
| `facade` | Facade |
| `proxy` | Proxy |

### Comportamentais (`behavioral/`)

| Módulo | Padrão |
|---|---|
| `command` | Command |
| `observer` | Observer |

## Como executar

Cada módulo possui uma função `main()` de demonstração. Para executar, entre na pasta da categoria e rode o módulo:

```bash
cd creational
python builder.py
```

Os módulos usam apenas a biblioteca padrão do Python, com uma exceção: `factory_method`, `prototype` e `singleton` importam `Self` de `typing_extensions`. Para executá-los, instale o pacote:

```bash
pip install typing_extensions
```

## Estrutura do projeto

```text
padroes-de-projeto-exemplos/
├── creational/
│   ├── abstract_factory.{py,asta,pdf}
│   ├── builder.{py,asta,pdf}
│   ├── factory_method.{py,asta,pdf}
│   ├── prototype.{py,asta,pdf}
│   └── singleton.{py,asta,pdf}
├── structural/
│   ├── bridge.{py,asta,pdf}
│   ├── class_adapter.{py,asta,pdf}
│   ├── object_adapter.{py,asta,pdf}
│   ├── facade.{py,asta,pdf}
│   └── proxy.{py,asta,pdf}
├── behavioral/
│   ├── command.{py,asta,pdf}
│   └── observer.{py,asta,pdf}
├── README.md
├── LICENSE
└── .gitignore
```

## Licença

Distribuído sob a licença MIT (arquivo [`LICENSE`](LICENSE)).
