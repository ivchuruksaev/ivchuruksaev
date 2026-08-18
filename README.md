<p align="center">
  <img src="./assets/header.svg" alt="Ivan Churuksaev — AI / Research Engineer" width="100%">
</p>

<p align="center">
  <a href="mailto:ivchuruksaev@icloud.com"><img src="https://img.shields.io/badge/email-ivchuruksaev%40icloud.com-6366f1?style=for-the-badge&logo=icloud&logoColor=white" alt="Email"></a>
  <a href="https://t.me/ivchuruksaev"><img src="https://img.shields.io/badge/Telegram-%40ivchuruksaev-0891d5?style=for-the-badge&logo=telegram&logoColor=white" alt="Telegram"></a>
  <img src="https://img.shields.io/badge/English-C1-0e7490?style=for-the-badge" alt="English C1">
</p>

## Профиль

**AI / Research Engineer** с физико-математическим бэкграундом и опытом решения прикладных ML-задач. Основные профессиональные интересы — графовые алгоритмы, scientific ML, анализ сложных сетей и гибридные системы, объединяющие классические методы с обучаемыми компонентами.

В работе совмещаю исследовательский и инженерный подходы:

- формулирую проверяемые гипотезы и проектирую эксперименты;
- строю модели, baseline-решения и воспроизводимые evaluation pipelines;
- анализирую ошибки, устойчивость и обобщающую способность методов;
- довожу прототипы до рабочих приложений, интерфейсов и инструментов автоматизации.

<table>
  <tr>
    <td width="33%" valign="top">
      <h3>🧭 Graph Algorithms</h3>
      Routing, shortest paths, graph agglomeration, coarsening и анализ сетевых структур.
    </td>
    <td width="33%" valign="top">
      <h3>🧪 Scientific ML</h3>
      DFT-данные, суррогатные модели, интерпретируемый ML и воспроизводимые исследования.
    </td>
    <td width="33%" valign="top">
      <h3>🛠️ Applied Systems</h3>
      ML-пайплайны, аналитические приложения, редакторские инструменты и автоматизация документов.
    </td>
  </tr>
</table>

## Опыт

### AI Engineer · 2022–2026

Работал над прикладными кейсовыми задачами машинного обучения, преимущественно в банковском домене и кредитном скоринге.

- Формализовывал бизнес-задачи в ML-постановку: определял target, метрики качества и ограничения решения.
- Исследовал табличные данные, контролировал качество выборки и проектировал признаки.
- Строил и сравнивал baseline и ML-подходы, настраивал схемы валидации.
- Анализировал ошибки моделей и уделял внимание интерпретируемости скоринговых решений.
- Оформлял эксперименты так, чтобы результаты можно было проверить и воспроизвести.

## Избранные проекты

### 🧭 GARA — Graph Agglomeration Routing Algorithm

**Исследовательский алгоритм приближённой маршрутизации на крупных взвешенных графах.**

- Разрабатываю метод ускорения routing queries через обучаемую агломерацию и компактное представление исходного графа.
- Сохраняю точную локальную область около source node; удалённую часть сети объединяю в coarse blocks со структурными и статистическими признаками.
- Исследую Pareto-компромисс `routing error ↔ online runtime`, отдельно учитывая preprocessing и inference.
- Проверяю graph-size, source, weight-distribution и topology generalization.
- Разрабатываю adaptive exact region, multilevel coarsening, corridor refinement и confidence-based fallback на локальный точный поиск.
- Сравниваю варианты GARA с exact shortest-path solvers и классическими coarsening-baselines.

**Стек:** `Python` `NetworkX` `Graph Algorithms` `Machine Learning` `Statistical Evaluation`

---

### 📄 Автоматизированная система сбора данных и формирования документов

**Веб-приложение, связывающее анкетирование, хранение данных и генерацию договоров.**

- Реализовал Flask-приложение с пользовательской анкетой и административной панелью.
- Организовал хранение и редактирование записей через SQLAlchemy и MySQL.
- Добавил морфологическую обработку ФИО с автоматическим склонением по падежам через `pymorphy2`.
- Реализовал подстановку данных в абзацы и таблицы DOCX-шаблонов.
- Автоматизировал конвертацию результата в PDF и выдачу готового документа.

**Стек:** `Python` `Flask` `SQLAlchemy` `MySQL` `pymorphy2` `python-docx` `PDF Automation`

---

### ✍️ [Petya Markdown Studio](https://github.com/ivchuruksaev/petya-markdown-studio)

**Local-first VS Code extension для работы с большими Markdown-документами.**

- Реализовал три синхронизированных режима: `Code`, `Split` и `Visual`, работающих с одним `.md`-источником.
- Добавил live preview, KaTeX, таблицы, outline, project-aware links и вставку изображений.
- Реализовал локальную историю версий, named checkpoints, diff и безопасное восстановление документа.
- Добавил редакторскую диагностику структуры, ссылок, TODO, незавершённых задач и читаемости текста.
- Настроил тесты, GitHub Actions, VSIX-релизы, документацию и GitHub Pages.
- Сохранил совместимость с Git, Auto Save, undo/redo и VS Code Live Share.

**Стек:** `JavaScript` `VS Code Extension API` `Webview` `Markdown` `KaTeX` `GitHub Actions`

---

### ⚗️ [HEA Energy Adsorption Screening](https://github.com/ivchuruksaev/HEA-energy-adsorption)

**ML-workflow для скрининга пятикомпонентных высокоэнтропийных сплавов в пространстве 19 металлов.**

- Объединил DFT-derived adsorption energies, frozen teacher model и интерпретируемые surrogate models.
- Реализовал линейно-квадратичную модель с элементными и парными композиционными признаками.
- Исследовал графовые нейросетевые модели для воспроизведения teacher-derived ranking.
- Организовал composition-level train/test splits, cross-validation и learning curves.
- Подготовил воспроизводимые скрипты, метрики, словарь данных и документацию пайплайна.

**Стек:** `Python` `pandas` `scikit-learn` `GNN` `DFT Data` `Reproducible ML`

---

### 🕸️ [СоциоГраф](https://github.com/ivchuruksaev/Socio)

**Интерактивное приложение для анализа социальных и организационных сетей.**

- Строит ориентированные графы сотрудников и агрегированные графы подразделений.
- Рассчитывает PageRank, betweenness, closeness, clustering coefficient и community structure.
- Поддерживает фильтрацию связей и интерактивное исследование структуры организации.
- Визуализирует лидеров, посредников, сообщества и изолированные области сети.

**Стек:** `Python` `Streamlit` `NetworkX` `Plotly` `scikit-learn` `Community Detection`

---

### 🔬 [HF Solid State](https://github.com/ivchuruksaev/HF-solid_state)

**Вычислительное исследование приближённых квантово-химических методов для твёрдого тела.**

- Исследовал применимость метода Хартри — Фока и полуэмпирических приближений.
- Работал с геометрией кристаллических структур и материалами из JARVIS.
- Ставил вычислительные эксперименты в Jupyter и сравнивал результаты с VASP.

**Стек:** `Python` `Jupyter` `Computational Physics` `Solid-State Modelling` `VASP` `JARVIS`

---

### 🌐 [IPRAN Network Simulation](https://github.com/ivchuruksaev/IPRAN)

- Моделирование grid-based сетевых топологий со случайными задержками и дополнительными кольцевыми связями.
- Визуализация сетей и расчёт кратчайших маршрутов алгоритмом Дейкстры.
- Практическая основа для последующих исследований в области graph routing и GARA.

**Стек:** `Python` `NetworkX` `Graph Simulation` `Shortest Paths`

## Образование

<table>
  <tr>
    <td width="50%" valign="top">
      <h3>🎓 Магистратура · Университет ИТМО</h3>
      <strong>Advanced Quantum and Nanophotonic Systems</strong><br>
      16.04.01 «Техническая физика» · англоязычная программа<br><br>
      Квантовая оптика, нанофотоника, электродинамика, физика твёрдого тела и численные методы.
    </td>
    <td width="50%" valign="top">
      <h3>🎓 Бакалавриат · Университет ИТМО</h3>
      <strong>Лазерные технологии</strong><br>
      12.03.05 «Лазерная техника и лазерные технологии»<br><br>
      Физико-математическая подготовка, моделирование, экспериментальная работа и инженерное мышление.
    </td>
  </tr>
</table>

## Технологии

<p>
  <img src="https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white" alt="Python">
  <img src="https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=111827" alt="JavaScript">
  <img src="https://img.shields.io/badge/SQL-334155?style=flat-square&logo=postgresql&logoColor=white" alt="SQL">
  <img src="https://img.shields.io/badge/scikit--learn-F7931E?style=flat-square&logo=scikitlearn&logoColor=white" alt="scikit-learn">
  <img src="https://img.shields.io/badge/pandas-150458?style=flat-square&logo=pandas&logoColor=white" alt="pandas">
  <img src="https://img.shields.io/badge/NetworkX-0e7490?style=flat-square" alt="NetworkX">
  <img src="https://img.shields.io/badge/Flask-111827?style=flat-square&logo=flask&logoColor=white" alt="Flask">
  <img src="https://img.shields.io/badge/Streamlit-FF4B4B?style=flat-square&logo=streamlit&logoColor=white" alt="Streamlit">
  <img src="https://img.shields.io/badge/Jupyter-F37626?style=flat-square&logo=jupyter&logoColor=white" alt="Jupyter">
  <img src="https://img.shields.io/badge/Git-F05032?style=flat-square&logo=git&logoColor=white" alt="Git">
  <img src="https://img.shields.io/badge/GitHub_Actions-2088FF?style=flat-square&logo=githubactions&logoColor=white" alt="GitHub Actions">
</p>

**Дополнительные направления:** внутренние информационные системы, аналитика опросов, Telegram-боты, DFT, Cosmo-RS и квантово-вдохновлённые вычисления.

---

<p align="center">
  <strong>Интересующие позиции: Research Engineer · ML Engineer · Scientific ML · Graph ML</strong>
</p>

