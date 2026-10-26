# Ukrainian Civic Terms Dataset / Набір даних української громадянської термінології

Open Ukrainian-language Q&A dataset for semantic search, information retrieval, and voice assistant applications in the field of civic engagement and public activity.
Відкритий україномовний набір даних типу «питання-відповідь», призначений для семантичного пошуку, інформаційного пошуку та застосунків із голосовими помічниками у сфері громадянської участі й громадської діяльності.

## About / Про проєкт

This repository contains a manually curated Ukrainian-language dataset developed as part of a bachelor's thesis:
У цьому репозиторії міститься відібраний вручну україномовний набір даних, розроблений у межах бакалаврської роботи:

**"Using machine learning for a query‑processing model of a voice assistant in the field of civic activity"**
"Використання машинного навчання для моделі оброблення запитів голосової помічниці у сфері громадської діяльності"

The dataset was created to support:
Цей набір даних було створено для підтримки:

- semantic search systems / систем семантичного пошуку;
- retrieval-augmented generation (RAG) / генерації з доповненням пошуком;
- voice assistants / голосових помічників;
- chatbots / чат-ботів;
- civic technology projects / проєктів у сфері громадянських технологій (civic tech);
- Ukrainian NLP research / досліджень в галузі обробки природної мови (NLP) українською мовою.

At the time of development, no comparable open Ukrainian-language datasets focused on civic engagement terminology and concepts could be identified. This repository is published to support further research, educational projects, and community-driven development.
На етапі розробки не вдалося знайти жодних порівнянних відкритих наборів даних українською мовою, які були б зосереджені на термінології та концепціях, пов’язаних із громадянською залученістю та гендерною рівністю. Цей репозиторій публікується для підтримки подальших досліджень, освітніх проєктів та розробок, що ініціюються спільнотою.

## Dataset Overview / Огляд набору даних

- Language: Ukrainian / Мова: українська
- Format: Question-Answer (Q&A) / Формат: «запитання — відповідь»
- Records: 1 682 / Кількість записів: 1 682
- Primary use case: Semantic search and knowledge retrieval / Основне призначення: семантичний пошук та отримання знань
- Domain: Civic engagement, gender equality, human rights, social participation, public activity / Тематична сфера: громадянська залученість, гендерна рівність, права людини, соціальна участь, громадська діяльність

## Data Structure / Структура даних

| Field | Description | 
|---------|------------|
| id | Unique identifier of a dataset record / Унікальний ідентифікатор запису в наборі даних|
| question | User query, phrase, or question related to a civic engagement concept or term / Запит, фраза або запитання користувача, що стосуються поняття чи терміна у сфері громадянської участі |
| answer | Definition, explanation, or response corresponding to the question / Визначення, пояснення або відповідь, що відповідає на запитання |
| intent | High-level intent or semantic category representing the user's information need (e.g., definition, rights, participation, equality) / Намір високого рівня або семантична категорія, що відображає інформаційну потребу користувача (наприклад, визначення, права, участь, рівність) |
| category | Thematic domain to which the concept belongs (e.g., civic engagement, human rights, gender equality, social inclusion) / Тематична сфера, до якої належить концепція (наприклад, громадянська участь, права людини, гендерна рівність, соціальна інклюзія) |
| notes | Additional information, context, source references, synonyms, or comments related to the entry / Додаткова інформація, контекст, посилання на джерела, синоніми або коментарі, що стосуються запису |


Example:

Приклад:

| id | question | answer | intent | category | notes |
|-----------|---------|-----------|-----------|-----------|-----------|
| 14 | Що таке гендер? | Це соціально закріплені ролі, поведінка, діяльність і характерні ознаки, які певне суспільство вважає належними для жінок та чоловіків. | gender_definition | соціологія;гендерні студії;права людини | Ґендер визначає, що саме очікується, допускається і цінується у жінок та чоловіків у певному соціальному та культурному контексті.|


## Sources / Джерела

The dataset was compiled and adapted based on publicly available educational and reference materials, including:
Набір даних було сформовано та адаптовано на основі загальнодоступних навчальних і довідкових матеріалів, зокрема:

- Babak M., Davlikanova O., Dmytriieva M., Kozyr M., Kompantseva L., Levchenko K., Skoryk M., Suslova O. (2021). *Glossary and Thesaurus of the European Institute for Gender Equality*. Vistka.
- Бабак М., Давліканова О., Дмитрієва М., Козир М., Компанцева Л., Левченко К., Скорик М., Суслова О. (2021). *Глосарій і тезаурус Європейського інституту з ґендерної рівності*. Вістка.
- Ukrainian Women Lawyers Association "JurFem". *Glossary on Gender-Responsive Recovery*.
- Асоціація жінок-юристок України «ЮрФем». *Глосарій з гендерно чутливого відновлення*.
  
The dataset represents a transformed and structured Q&A resource and should not be considered a direct reproduction of any source material.
Цей набір даних являє собою перетворений і структурований ресурс у форматі «запитання-відповідь» і не повинен розглядатися як пряме відтворення будь-якого першоджерела.

## Intended Uses / Цільове використання

The dataset may be useful for:
Набір даних може бути корисним для:

- semantic search systems / систем семантичного пошуку;
- vector database experiments / експериментів з векторними базами даних;
- conversational AI / розмовного штучного інтелекту;
- Ukrainian-language NLP research / досліджень україномовного NLP;
- educational and academic projects / освітніх та академічних проектів;
- civic-tech solutions / рішень у сфері громадянських технологій.

## Limitations / Обмеження

- The dataset focuses on a specific thematic domain / Набір даних зосереджений на певній тематичній області.
- It is not designed as a general-purpose QA benchmark / Він не розроблений як універсальний бенчмарк контролю якості.
- Definitions may reflect interpretations from source materials available at the time of compilation / Визначення можуть відображати інтерпретації з вихідних матеріалів, доступних на момент складання.
- Users should independently verify critical information before deploying systems in production environments / Користувачі(-ки) повинні самостійно перевіряти критичну інформацію перед розгортанням систем у виробничому середовищі.

## Contributing / Долучення

Contributions are welcome.
Долучення вітається.

You can help by:
Ви можете допомогти:

- adding new Q&A pairs / додаванням нових пар запитань та відповідей;
- correcting wording or terminology / виправленням формулювань або термінології;
- expanding topic coverage / розширенням охоплення теми;
- improving metadata and documentation / покращенням метаданих та документації.

Please open an issue or submit a pull request.
Будь ласка, відкрийте проблему або надішліть запит на зняття.

## Citation / Цитування

If you use this dataset in research, educational projects, or publications, please cite the repository and acknowledge the original sources.
Якщо ви використовуєте цей набір даних у дослідженнях, освітніх проектах або публікаціях, будь ласка, вкажіть репозиторій та оригінальні джерела.

## License / Ліцензія

Please see the LICENSE file for licensing information.
Будь ласка, перегляньте файл ЛІЦЕНЗІЇ для отримання інформації про ліцензування.

