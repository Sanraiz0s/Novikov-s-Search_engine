*ENG*

# Project Information

This project is a fully functional search engine designed to process search queries across multiple documents. It includes components for reading configuration files, building an inverted index of documents, handling search requests, and generating responses in JSON format. The project is implemented in C++ and optimized for fast retrieval of relevant documents based on given keywords.

---

# Technologies Used

- C++ (C++17 standard)
- nlohmann/json — library for working with JSON files
- Standard C++ libraries:
    - \<fstream>\, \<iostream>\, \<string>\, \<vector>\, \<map>\, \<thread>\, \<mutex>\, \<exception>\, \<unordered_set>\, \<unordered_map>

---

# How to Run the Project Locally

Steps to run:

1. Download the project archive.
2. Configure the necessary files:

   In the root directory, the following files should be located:

    - `config.json` — project configuration file, includes project name, version, and list of document files
    - `requests.json` — file with search queries
    - `answers.json` — output file for responses (will be overwritten during execution)

   Place the corresponding files into the *cmake-build-release* folder.

   If `config.json` and `requests.json` are missing, the program will display an error message and terminate.

3. Add all required `.txt` files for reading into the `resources` folder.

4. Run the project.

   The *cmake-build-release* folder contains the executable `search_engine.exe`. Launch it.

   The program will read the configuration and request files, build the index, perform the search, and write the responses into `answers.json`.

---

# Required Environment Variables

In the current implementation, environment variables are not required. All necessary parameters are set via `config.json`, `requests.json`, and `answers.json`.

---

*RUS*
# Информация о проекте

Данный проект представляет собой полнофункциональный движок для обработки поисковых запросов по множественным документам. Он включает компоненты для чтения конфигурационных файлов, построения инвертированного индекса документов, обработки поисковых запросов и формирования ответов в формате JSON. Проект реализован на C++ и предназначен для быстрого поиска релевантных документов по заданным ключевым словам.

---

# Стек используемых технологий

- *C++* (стандарт C++17)
- *nlohmann/json* — библиотека для работы с файлами JSON
- Стандартные библиотеки C++:
    - \<fstream>\, \<iostream>\, \<string>\, \<vector>\, \<map>\, \<thread>\, \<mutex>\, \<exception>\, \<unordered_set>\, \<unordered_map>

---

# Инструкция по запуску проекта локально

*Шаги запуска:*

1. Скачайте архив репозитория.
2. Настройка конфигурационных файлов:

   В корне репозитория должны находиться следующие файлы:

- `config.json` — описание конфигурации проекта, включает название, версию и список файлов документов
- `requests.json` — файл с запросами поиска
- `answers.json` — файл для вывода ответов (будет перезаписываться при выполнении)

Добавьте соответствующие файлы в папку *cmake-build-release*.

В случае отсутствия `config.json` и `requests.json` программа выведет соответствующую ошибку и будет остановлена.

3. В данном репозитории добавьте в папку *resources* все необходимые файлы для чтения в формате `.txt`.

4. Запуск проекта.

В папке *cmake-build-release* находится файл `search_engine.exe`. Запустите его.

Проект прочитает конфигурационные и запросные файлы, построит индекс, выполнит поиск и запишет ответы в `answers.json`.


# Обязательные переменные окружения

В текущей реализации переменные окружения не требуют настройки. Все необходимые параметры задаются через `config.json`, `requests.json` и `answers.json`.

---



