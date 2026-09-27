<div id="top"></div>

<div align="center">

<!-- pixel-kit:header style="cyberpunk" title="ТОКМ : ЛАБА 1" subtitle="СТОХАСТИЧЕСКОЕ 3D-МОДЕЛИРОВАНИЕ ТОЧЕЧНЫХ ОБЛАКОВ // GLSCENE" spec1="ДИСЦИПЛИНА: ТЕОРЕТИЧЕСКИЕ ОСНОВЫ КОМПЬЮТЕРНОГО МОДЕЛИРОВАНИЯ" spec2="СТУДЕНТ: ФРОЛОВ АРТЕМ // ГР. 12002531 // НИУ БЕЛГУ" spec3="ЭТАП СДАЧИ: ЛАБОРАТОРНЫЕ РАБОТЫ 1–1 (ЭТАП 1/5)" tag="STAGE_1/5" out="assets/header.svg" -->

<br/><br/>

<!-- pixel-kit:chip style="cyberpunk" type="closed" text="📋 ДОСЬЕ" url="#dossier" out="assets/nav-dossier.svg" -->
  &nbsp;
  <!-- pixel-kit:chip style="cyberpunk" type="closed" text="⭐ БАЗОВЫЕ" url="#repos" out="assets/nav-repos.svg" -->
  &nbsp;
  <!-- pixel-kit:chip style="cyberpunk" type="closed" text="⚡ ЛАБА 1" url="#lab1" out="assets/nav-lab1.svg" -->
  &nbsp;
  <!-- pixel-kit:chip style="cyberpunk" type="closed" text="🛠️ СБОРКА" url="#build" out="assets/nav-build.svg" -->

<br/><br/>

<!-- pixel-kit:divider style="cyberpunk" out="assets/divider-top.svg" -->

</div>

<br/>

<span id="dossier"></span>

<!-- pixel-kit:window style="cyberpunk" title="╔═ DOSSIER.SYS // АКАДЕМИЧЕСКОЕ ДОСЬЕ" tag="[STUDENT]" out_top="assets/frame-dossier-top.svg" out_bottom="assets/frame-dossier-bottom.svg" -->
<!-- pixel-kit:quote style="cyberpunk" badge="DISCIPLINE" title="ТЕОРЕТИЧЕСКИЕ ОСНОВЫ КОМПЬЮТЕРНОГО МОДЕЛИРОВАНИЯ" subtitle="Embarcadero RAD Studio C++Builder • GLScene • TetGen • Newton Dynamics" out="assets/quote-dossier.svg" -->
Репозиторий лабораторных работ по дисциплине **«Теоретические основы компьютерного моделирования»** (ТОКМ) с использованием графической библиотеки **GLScene**, меш-генератора **TetGen 1.5** и физического движка **Newton Dynamics** в среде **Embarcadero RAD Studio C++Builder**.
<!-- /pixel-kit:quote -->

<br/>

* **Студент**: Фролов Артем Алексеевич
* **Группа**: 12002531 (2 курс магистратуры)
* **Университет**: НИУ «БелГУ», Институт инженерных и цифровых технологий (ИИЦТ)
* **Кафедра**: Математического и программного обеспечения информационных систем (МПОИС)
* **Преподаватель**: доц. Васильев Павел Владимирович
* **Курс в СДО «Пегас»**: <!-- pixel-kit:chip style="cyberpunk" type="pulse" text="● СДО ПЕГАС" url="https://pegas.bsuedu.ru/course/view.php?id=15521" out="assets/chip-pegas.svg" -->
* **GitHub репозиторий**: <!-- pixel-kit:chip style="cyberpunk" type="closed" text="⚡ GITHUB REPO" url="https://github.com/Kazinagg/bsu-tokm-lab1" out="assets/chip-github.svg" -->
* **Стадия сдачи**: Лабораторные работы 1–1 (накопительный репозиторий)
<!-- /pixel-kit:window -->

<br/>

<span id="repos"></span>

<!-- pixel-kit:window style="cyberpunk" title="╔═ BASE_REPOSITORIES.SYS // БАЗОВЫЕ ПРОЕКТЫ" tag="[GLSCENE]" out_top="assets/frame-repos-top.svg" out_bottom="assets/frame-repos-bottom.svg" -->
В соответствии с требованиями преподавателя, базовые проекты изучены и отмечены звёздочками ⭐:

1. <!-- pixel-kit:chip style="cyberpunk" type="decay" text="★ GLXEngine" url="https://github.com/glscene/GLXEngine" out="assets/chip-base-glx.svg" --> — графический движок на базе OpenGL для C++Builder и Delphi.
2. <!-- pixel-kit:chip style="cyberpunk" type="decay" text="★ AstrobloQ" url="https://github.com/glscene/AstrobloQ" out="assets/chip-base-astro.svg" --> — система компьютерного моделирования астрономических объектов и плагинов лаб на C++Builder.
<!-- /pixel-kit:window -->

<br/>

<span id="plan"></span>

<!-- pixel-kit:window style="cyberpunk" title="╔═ REPOSITORY_MANIFEST.SYS // СОСТАВ РАБОТ" tag="[MANIFEST]" out_top="assets/frame-plan-top.svg" out_bottom="assets/frame-plan-bottom.svg" -->
| № | Наименование лабораторной работы | Статус | Исходный код | Отчет (.docx) |
|:---:|---|:---:|:---:|:---:|
| **1** | **3D облако точек в объеме контейнеров (GLScene)**<br><sub>Стохастическое моделирование точечных и поверхностных тел в GLScene</sub> | <!-- pixel-kit:chip style="cyberpunk" type="closed" text="✓ СДАНА" out="assets/badge-passed.svg" --> | <!-- pixel-kit:chip style="cyberpunk" type="closed" text="📁 lab1/" url="lab1/" out="assets/chip-plan-dir1.svg" --> | <!-- pixel-kit:chip style="cyberpunk" type="closed" text="📄 Л1 Фролов.docx" url="Л1%20Фролов.docx" out="assets/chip-plan-docx1.svg" --> |

<br/>

<!-- pixel-kit:callout style="cyberpunk" type="note" title="GROUP PROJECT // RAD STUDIO C++BUILDER" subtitle="Единая среда kommod.groupproj и tokm.groupproj для одновременной компиляции" out="assets/callout-groupproj.svg" -->
В репозитории размещен файл [`kommod.groupproj`](kommod.groupproj) (а также зеркальный `tokm.groupproj`), сконфигурированный для одновременной компиляции всех активных лабораторных работ (ЛР №1) в единой рабочей среде.
<!-- /pixel-kit:window -->

<br/>

<span id="lab1"></span>

<!-- pixel-kit:divider style="cyberpunk" out="assets/divider-lab1.svg" -->

<br/>

<!-- pixel-kit:window style="cyberpunk" title="╔═ LAB_1.SYS // 3D ТОЧЕЧНЫЕ ОБЛАКА В GLSCENE" tag="[STAGE_1]" out_top="assets/frame-lab1-top.svg" out_bottom="assets/frame-lab1-bottom.svg" -->
<div align="left">
  <b>Файлы работы:</b>
  <!-- pixel-kit:chip style="cyberpunk" type="closed" text="📁 ИСХОДНИКИ" url="lab1/exp/Lab1/" out="assets/chip-lab1-sub.svg" -->
  <!-- pixel-kit:chip style="cyberpunk" type="closed" text="⚙️ ПРОЕКТ CBPROJ" url="lab1/exp/Lab1/RandomStars.cbproj" out="assets/chip-lab1-proj.svg" -->
  <!-- pixel-kit:chip style="cyberpunk" type="closed" text="📄 ОТЧЕТ WORD" url="Л1%20Фролов.docx" out="assets/chip-docx-l1.svg" -->
</div>

<br/>

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
<!-- /pixel-kit:window -->

<br/>

<span id="build"></span>

<!-- pixel-kit:terminal style="cyberpunk" title="BUILD_INSTRUCTIONS.SH // СБОРКА И ЗАПУСК" state="open" out_top="assets/terminal-build-top.svg" out_bottom="assets/terminal-build-bottom.svg" -->
```bash
# Клонирование репозитория
git clone https://github.com/Kazinagg/bsu-tokm-lab1.git
cd bsu-tokm-lab1
```

* **Среда разработки:** Embarcadero RAD Studio C++Builder 12 / 13;
* **Графический пакет:** GLScene (Open source OpenGL library for Delphi & C++Builder);
* **Компилятор:** Embarcadero Clang 32-bit / 64-bit;
* **Сборка через групповой проект:** откройте [`kommod.groupproj`](kommod.groupproj) в RAD Studio и выполните команду `Project -> Build All Projects`.
<!-- /pixel-kit:terminal -->

<br/><br/>

<div align="center">

<!-- pixel-kit:footer style="cyberpunk" status="SESSION_ONLINE // LABS 1–1 READY" nav="ВЕРНУТЬСЯ К ШАПКЕ" sub="ДИСЦИПЛИНА: ТОКМ // СТУДЕНТ: ФРОЛОВ А.А. (12002531) // НИУ БЕЛГУ" out="assets/footer.svg" -->

<br/><br/>

<sub>ТОКМ &bull; BelSU / НИУ «БелГУ» &bull; ФРОЛОВ А.А. &bull; 2026</sub>

</div>
