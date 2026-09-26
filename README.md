<div align="center">
  <img src="assets/header-lab1.svg" width="100%" alt="ТОКМ // 3D GLScene Computer Modeling" />
</div>

<br>

<div align="center">
  <a href="#dossier"><img src="assets/nav-dossier.svg" alt="Досье" /></a>
  <a href="#repos"><img src="assets/nav-repos.svg" alt="Базовые" /></a>
  <a href="#lab1"><img src="assets/nav-lab1.svg" alt="Лаба 1" /></a>
  <a href="#build"><img src="assets/chip-code.svg" height="24" alt="Сборка" /></a>
</div>

<br>

<div align="center">
  <img src="assets/pcb-divider.svg" width="100%" alt="PCB Divider" />
</div>

<span id="dossier"></span>

<div align="center">
  <img src="assets/frame-dossier.svg" width="100%" alt="Академическое досье" />
</div>

> Репозиторий лабораторных работ по дисциплине **«Теоретические основы компьютерного моделирования»** (ТОКМ) с использованием графической библиотеки **GLScene**, меш-генератора **TetGen 1.5** и физического движка **Newton Dynamics** в среде **Embarcadero RAD Studio C++Builder**.

* **Студент**: Фролов Артем Алексеевич
* **Группа**: 12002531 (2 курс магистратуры)
* **Университет**: НИУ «БелГУ», Институт инженерных и цифровых технологий (ИИЦТ)
* **Кафедра**: Математического и программного обеспечения информационных систем (МПОИС)
* **Преподаватель**: доц. Васильев Павел Владимирович
* **Курс в СДО «Пегас»**: <a href="https://pegas.bsuedu.ru/course/view.php?id=15521"><img src="assets/chip-pegas.svg" height="24" alt="Пегас Курс 15521" /></a>
* **GitHub репозиторий**: <a href="https://github.com/Kazinagg/bsu-tokm-lab1"><img src="assets/chip-github.svg" height="24" alt="GitHub Repo" /></a>
* **Стадия сдачи**: Лабораторные работы 1–1 (накопительный репозиторий)

<div align="center">
  <img src="assets/frame-bottom.svg" width="100%" alt="Конец фрейма" />
</div>

<br>

<div align="center">
  <img src="assets/pcb-divider.svg" width="100%" alt="PCB Divider" />
</div>

<span id="repos"></span>

<div align="center">
  <img src="assets/frame-base-repos.svg" width="100%" alt="Базовые репозитории" />
</div>

В соответствии с требованиями преподавателя, базовые проекты изучены и отмечены звёздочками ⭐:

1. <a href="https://github.com/glscene/GLXEngine"><img src="assets/chip-base-glx.svg" height="24" alt="GLXEngine" /></a> — графический движок на базе OpenGL для C++Builder и Delphi.
2. <a href="https://github.com/glscene/AstrobloQ"><img src="assets/chip-base-astro.svg" height="24" alt="AstrobloQ" /></a> — система компьютерного моделирования астрономических объектов и плагинов лаб на C++Builder.

<div align="center">
  <img src="assets/frame-bottom.svg" width="100%" alt="Конец фрейма" />
</div>

<br>

<div align="center">
  <img src="assets/pcb-divider.svg" width="100%" alt="PCB Divider" />
</div>

<span id="plan"></span>

<div align="center">
  <img src="assets/frame-plan.svg" width="100%" alt="Состав репозитория" />
</div>

| № | Наименование лабораторной работы | Статус | Исходный код | Отчет (.docx) |
|:---:|---|:---:|:---:|:---:|
| **1** | **3D облако точек в объеме контейнеров (GLScene)**<br><sub>Стохастическое моделирование точечных и поверхностных геометрических тел в GLScene</sub> | <img src="assets/badge-passed.svg" height="24" alt="Сдана" /> | <a href="lab1/"><img src="assets/chip-lab1-dir.svg" height="24" alt="lab1/" /></a> | <a href="Л1 Фролов.docx"><img src="assets/chip-docx-l1.svg" height="24" alt="Л1 Фролов.docx" /></a> |


> [!TIP]
> **Групповой проект RAD Studio C++Builder:** В репозитории размещен файл [`kommod.groupproj`](kommod.groupproj) (а также зеркальный `tokm.groupproj`), сконфигурированный для одновременной компиляции всех активных лабораторных работ (ЛР №1) в единой рабочей среде.


<div align="center">
  <img src="assets/frame-bottom.svg" width="100%" alt="Конец фрейма" />
</div>

<br>

<div align="center">
  <img src="assets/pcb-divider.svg" width="100%" alt="PCB Divider" />
</div>

<span id="lab1"></span>

<div align="center">
  <img src="assets/frame-lab1.svg" width="100%" alt="Лабораторная работа 1" />
</div>

<div align="left">
  <b>Файлы работы:</b>
  <a href="lab1/exp/Lab1/"><img src="assets/chip-lab1-sub.svg" height="24" alt="Директория" /></a>
  <a href="lab1/exp/Lab1/RandomStars.cbproj"><img src="assets/chip-lab1-proj.svg" height="24" alt="Проект C++Builder" /></a>
  <a href="Л1%20Фролов.docx"><img src="assets/chip-docx-l1.svg" height="24" alt="Отчет Word" /></a>
</div>

<br>

Проект разработан в папке [`lab1/exp/Lab1/`](lab1/exp/Lab1/) на C++Builder (`RandomStars.cbproj`).

### Реализованные задачи и алгоритмы:
1. **Шесть типов 3D-контейнеров с равномерной плотностью**:
   - **Кубический объем** ($1024 \times 1024 \times 1024$);
   - **Объем шара** (равномерное распределение $r = R \cdot \sqrt[3]{u}$, где $u \in [0, 1)$);
   - **Поверхность сферы** (изотропные углы $\phi \in [0, 2\pi)$, $\cos\theta \in [-1, 1]$);
   - **Цилиндрический объем** ($r = R \cdot \sqrt{u}$ для постоянной плотности по сечению);
   - **Поверхность цилиндра**;
   - **Конический объем** ($r = R(1 - h)\sqrt{u}$).
2. **Альтернативный режим вывода 3D-сфер (`TGLSphere`)**:
   - Создание динамических сфер с радиусом в диапазоне $[5, 25]$ единиц;
   - Применение 7 спектральных цветов радуги (**КОЖЗГСФ**);
   - Материалы со свойствами `Diffuse` и `Emission` для эффекта собственного свечения.
3. **Моделирование времени жизни и свечения звезд**:
   - В обработчике `TGLCadencer.OnProgress` реализован индивидуальный таймер свечения точек $[1, 100]$ секунд;
   - Линейное затухание яркости: $factor = curLife / maxLife$;
   - Автоматическое «перерождение» точек со случайным интервалом после угасания.
4. **Анализ производительности графического конвейера**:
   - Для массива из 100 000 точек частота кадров составляет 230–258 FPS при времени генерации менее 0.09 с;
   - В режиме полигональных 3D-сфер кадровая частота превышает 1200 FPS.

<div align="center">
  <img src="assets/frame-bottom.svg" width="100%" alt="Конец фрейма" />
</div>


<br>

<div align="center">
  <img src="assets/pcb-divider.svg" width="100%" alt="PCB Divider" />
</div>

<span id="build"></span>

### 🛠️ Инструкция по сборке и запуску проектов

```bash
# Клонирование репозитория
git clone https://github.com/Kazinagg/bsu-tokm-lab1.git
cd bsu-tokm-lab1
```

* **Среда разработки:** Embarcadero RAD Studio C++Builder 12 / 13;
* **Графический пакет:** GLScene (Open source OpenGL library for Delphi & C++Builder);
* **Компилятор:** Embarcadero Clang 32-bit / 64-bit;
* **Сборка через групповой проект:** откройте [`kommod.groupproj`](kommod.groupproj) в RAD Studio и выполните команду `Project -> Build All Projects`.

<br>

<div align="center">
  <code>[SYS_EXIT: 0x00] // TOKM_GLSCENE_LABS // STAGE_1_READY // SESSION TERMINATED</code>
</div>
