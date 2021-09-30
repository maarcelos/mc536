# Modelo para Apresentação do Lab06 - Artigo de Dataset Público

Estrutura de pastas:

~~~
├── README.md  <- arquivo apresentando a tarefa
│
└── images     <- arquivos de imagem usados na tarefa (se houver)
~~~

# Aluno
* `240765`: `Marcelo Salles Previti`

# Análise do Artigo `Dataset: Person Tracking and Identification using Cameras and Wi-Fi Channel State Information (CSI) from Smartphones`

| campo | valor |
|------------|----------------------------------------|
| referência | `Shiwei Fang, Sirajum Munir, and Shahriar Nirjon. 2020. Dataset: Person Tracking and Identification using Cameras and Wi-Fi Channel State Information (CSI) from Smartphones. In The 3rd International SenSys+BuildSys Workshop on Data: Acquisition to Analysis (DATA ’20), November 16–19, 2020, Virtual Event, Japan. ACM, New York, NY, USA, 5 pages. https://doiorg/10.1145/3419016.3431488` |
| link       | `https://dl.acm.org/doi/10.1145/3419016.3431488` |
| dataset | `https://zenodo.org/record/3882104#.YVWzOJrMLIU` |
| formato | `HDF5` |

## Resumo

> O artigo propõe-se em implementar um novo método de rastreamento de pessoas em ambientes, através da combinação de câmeras e da leitura de sinal wi-fi proveniente de smartphones. Enquanto outros métodos de rastreamento possuem defeitos como falta de privacidade - por exemplo, ao utilizar-se de técnicas de reconhecimento facial- ou mesmo falta de escalabilidade - como identificadores de sinais ultrasôncios - o método proposto se adequaria a esses dois critérios. Por fim, um dataset é disponibilizado contendo as informações de várias configurações - com variadas pessoas em variados ambientes.

## Perguntas de pesquisa/análises

> Com o dataset, podemos analisar a diferença no sinal recebido para duas pessoas distintas que ocupam mesma posição (no caso, analisar como a diferença de altura e maneira como o indivíduo segura o telefone influenciam no sinal recebido). Além disso, pode-se analisar a interferência do sinal, ao comparar a diferença do sinal recebido em uma posição x, e o mesmo sinal, proveniente do mesmo indivíduo e na mesma posição, contudo em um ambiente cheio.  

## Trabalhos relacionados

> Pode-se citar outras iniciativas similares aos do projeto no qual possuem objetivo igual - no caso, determinar os indivíduos presentes em determinada localidade - porém com distintas tecnologias, como utilizando-se somente de câmeras (Omar Hamdoun, Fabien Moutarde, Bogdan Stanciulescu, and Bruno Steux. 2008.Person re-identification in multi-camera system by signature based on interest point descriptors collected on short video sequences. In 2008 Second ACM/IEEE International Conference on Distributed Smart Cameras. IEEE, 1–6) ou mesmo sensores infra-vermelho (Hessam Mohammadmoradi, Sirajum Munir, Omprakash Gnawali, and Charles Shelton. 2017. Measuring people-flow through doorways using easy-to-install ir array sensors. In 2017 13th International Conference on Distributed Computing in Sensor Systems (DCOSS). IEEE, 35–43.)