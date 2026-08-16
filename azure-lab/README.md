# LAB Azure Speech Studio e Language Studio

Este diretório possui anotações e práticas realizadas durante o laboratório sobre a análise de fala e linguagem natural utilizando os serviços **Azure Speech Studio** e **Azure Language Studio**.

📌**Objetivos do LAB**
- Transcrever áudio usando o **Speech Studio**;
- Analisar sentimentos e linguagem usando o **Language Studio**;
- Registrar os passos realizados;
- Documentar resultados, prints e insights.

🗂**Estrutura do diretório**
```
azure-lab/
 ├── images/                                          # Capturas de tela do LAB
 |     ├── Screenshot_Analyzed_Sentiment.png          # Captura de tela da Análise de Sentimento
 |     ├── Screenshot_Erro_Language_Studio.png        # Captura de tela do Erro no Language Studio
 |     ├── Screenshot_Original_Text.png               # Captura de tela com detalhes da Análise de Sentimento
 |     ├── Screenshot_Test_Result.png                 # Captura de tela do Resultado do Teste
       └── Screenshot_Upload_Audio.png                # Captura de tela do Upload do arquivo
 |── README.md                                        # Documento principal
 ├── language/                                        # Testes e anotações do Language Studio
 └── speech/                                          # Testes e anotações do Speech Studio

```

🎤**Speech Studio - Transcrição do Áudio**
- Upload de um áudio curto;
- Execução da transcrição;
- Observações sobre precisão, sotaque e qualidade;
- Prints disponíveis na pasta ```/images```


*Batch speech to text - Test results*

Model: 20250808

Profanity filter mode: Masked

Language: English (United States)

Punctuation mode: DictatedAndAutomatic

Speaker diarization: No

Word level timestamp: Yes (display); No (lexical)

[Channel 0] 
Timmy feels like a combination of dance, choreography, writing and story, and like magic that you will never know the secrets to. I'll take the odd. 

[Channel 1] 
Timmy feels like a combination of dance, choreography, writing and story and like magic that you will never know the secrets to. I'll take the the audience. 


🧠 **Language Studio - Análise de Sentimentos (Exemplo do Cognitive Services)**

Durante a etapa de análise de linguagem natural, não foi possível acessar o **Azure Language Studio** devido a restrições de autenticação com contas pessoais (MSA).

Para cumprir o objetivo do laboratório, utilizei o exemplo oficial disponível no site do Azure Cognitive Services, que demonstra o funcionamento da ferramenta de *Sentiment and Opinion Mining*.

O Language Studio identifica automaticamente:

- **Sentimentos positivos** (ex.: veste perfeitamente, lindo, maravilhosamente confortável);
- **Sentimentos mistos** (ex.: dificuldade com o zíper);
- **Targets** (elementos avaliados, como zíper, cor, material);
- **Assessments** (opiniões associadas a cada target).

Essas marcações permitem visualizar como o modelo analisa aspectos específicos de um produto e associa cada um a um sentimento correspondente. A captura de tela utilizada encontra-se na pasta ```/images```.


📘 **Conclusão**

Este laboratório permitiu explorar duas ferramentas da Azure AI voltadas para processamento de fala e linguagem natural:

- Speech Studio, utilizado com sucesso para transcrição automática de áudio;
- Language Studio, cuja demonstração foi realizada por meio de um exemplo oficial do Azure Cognitive Services devido a limitações de acesso com contas pessoais.

Mesmo com essa adaptação, foi possível compreender o fluxo completo:

- Transformar áudio em texto;

- Aplicar análise de sentimentos ao conteúdo textual;

- Registrar resultados, prints e estrutura do projeto no GitHub;

O repositório final documenta todo o processo, incluindo dificuldades encontradas e soluções adotadas, mantendo alinhamento com os objetivos do LAB.




