<div id="top"></div>

<div align="center">

<img src="assets/header.svg" width="100%" alt="ТОКМ : ЛАБА 1" />

<br/><br/>

<a href="#dossier"><img src="assets/nav-dossier.svg" alt="📋 ДОСЬЕ" /></a>
  &nbsp;
  <a href="#repos"><img src="assets/nav-repos.svg" alt="⭐ БАЗОВЫЕ" /></a>
  &nbsp;
  <a href="#lab1"><img src="assets/nav-lab1.svg" alt="⚡ ЛАБА 1" /></a>
  &nbsp;
  <a href="#build"><img src="assets/nav-build.svg" alt="🛠️ СБОРКА" /></a>

<br/><br/>

<img src="assets/divider-top.svg" width="100%" alt="Divider cyberpunk" />

</div>

<br/>

<span id="dossier"></span>

<img src="assets/frame-dossier-top.svg" width="100%" />

<table width="100%">
<tr>
<td width="2000">

> <img src="assets/quote-dossier.svg" width="100%" />
>
> Репозиторий лабораторных работ по дисциплине **«Теоретические основы компьютерного моделирования»** (ТОКМ) с использованием графической библиотеки **GLScene**, меш-генератора **TetGen 1.5** и физического движка **Newton Dynamics** в среде **Embarcadero RAD Studio C++Builder**.

<br/>

* **Студент**: Фролов Артем Алексеевич
* **Группа**: 12002531 (2 курс магистратуры)
* **Университет**: НИУ «БелГУ», Институт инженерных и цифровых технологий (ИИЦТ)
* **Кафедра**: Математического и программного обеспечения информационных систем (МПОИС)
* **Преподаватель**: доц. Васильев Павел Владимирович
* **Курс в СДО «Пегас»**: <a href="https://pegas.bsuedu.ru/course/view.php?id=15521"><img src="assets/chip-pegas.svg" alt="● СДО ПЕГАС" /></a>
* **GitHub репозиторий**: <a href="https://github.com/Kazinagg/bsu-tokm-lab1"><img src="assets/chip-github.svg" alt="⚡ GITHUB REPO" /></a>
* **Стадия сдачи**: Лабораторные работы 1–1 (накопительный репозиторий)

</td>
</tr>
</table>

<img src="assets/frame-dossier-bottom.svg" width="100%" />

<br/>

<span id="repos"></span>

<img src="assets/frame-repos-top.svg" width="100%" />

<table width="100%">
<tr>
<td width="2000">

В соответствии с требованиями преподавателя, базовые проекты изучены и отмечены звёздочками ⭐:

1. <a href="https://github.com/glscene/GLXEngine"><img src="assets/chip-base-glx.svg" alt="★ GLXEngine" /></a> — графический движок на базе OpenGL для C++Builder и Delphi.
2. <a href="https://github.com/glscene/AstrobloQ"><img src="assets/chip-base-astro.svg" alt="★ AstrobloQ" /></a> — система компьютерного моделирования астрономических объектов и плагинов лаб на C++Builder.

</td>
</tr>
</table>

<img src="assets/frame-repos-bottom.svg" width="100%" />

<br/>

<span id="plan"></span>

<img src="assets/frame-plan-top.svg" width="100%" />

<table width="100%">
<tr>
<td width="2000">

| № | Наименование лабораторной работы | Статус | Исходный код | Отчет (.docx) |
|:---:|---|:---:|:---:|:---:|
| **1** | **3D облако точек в объеме контейнеров (GLScene)**<br><sub>Стохастическое моделирование точечных и поверхностных тел в GLScene</sub> | <img src="assets/badge-passed.svg" alt="✓ СДАНА" /> | <a href="lab1/"><img src="assets/chip-plan-dir1.svg" alt="📁 lab1/" /></a> | <a href="Л1%20Фролов.docx"><img src="assets/chip-plan-docx1.svg" alt="📄 Л1 Фролов.docx" /></a> |

<br/>

<img src="assets/callout-groupproj.svg" width="100%" />
В репозитории размещен файл [`kommod.groupproj`](kommod.groupproj) (а также зеркальный `tokm.groupproj`), сконфигурированный для одновременной компиляции всех активных лабораторных работ (ЛР №1) в единой рабочей среде.

</td>
</tr>
</table>

<img src="assets/frame-plan-bottom.svg" width="100%" />

<br/>

<span id="lab1"></span>

<img src="assets/divider-lab1.svg" width="100%" alt="Divider cyberpunk" />

<br/>

<img src="assets/frame-lab1-top.svg" width="100%" />

<table width="100%">
<tr>
<td width="2000">

<div align="left">
  <b>Файлы работы:</b>
  <a href="lab1/exp/Lab1/"><img src="assets/chip-lab1-sub.svg" alt="📁 ИСХОДНИКИ" /></a>
  <a href="lab1/exp/Lab1/RandomStars.cbproj"><img src="assets/chip-lab1-proj.svg" alt="⚙️ ПРОЕКТ CBPROJ" /></a>
  <a href="Л1%20Фролов.docx"><img src="assets/chip-docx-l1.svg" alt="📄 ОТЧЕТ WORD" /></a>
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

</td>
</tr>
</table>

<img src="assets/frame-lab1-bottom.svg" width="100%" />

<br/>

<span id="build"></span>

<details open>
<summary><kbd>▶ BUILD_INSTRUCTIONS.SH // СБОРКА И ЗАПУСК</kbd> <b>[ НАЖМИТЕ ДЛЯ СВОРАЧИВАНИЯ / РАЗВОРАЧИВАНИЯ ]</b> <code>[STATE: EXPANDED]</code></summary>

<br/>

<img src="assets/terminal-build-top.svg" width="100%" />

<table width="100%">
<tr>
<td width="2000">

```bash
# Клонирование репозитория
git clone https://github.com/Kazinagg/bsu-tokm-lab1.git
cd bsu-tokm-lab1
```

* **Среда разработки:** Embarcadero RAD Studio C++Builder 12 / 13;
* **Графический пакет:** GLScene (Open source OpenGL library for Delphi & C++Builder);
* **Компилятор:** Embarcadero Clang 32-bit / 64-bit;
* **Сборка через групповой проект:** откройте [`kommod.groupproj`](kommod.groupproj) в RAD Studio и выполните команду `Project -> Build All Projects`.

</td>
</tr>
</table>

<img src="assets/terminal-build-bottom.svg" width="100%" />

</details>

<br/><br/>

<div align="center">

<a href="#top"><img src="assets/footer.svg" width="100%" alt="ВЕРНУТЬСЯ К ШАПКЕ" /></a>

<br/><br/>

<sub>ТОКМ &bull; BelSU / НИУ «БелГУ» &bull; ФРОЛОВ А.А. &bull; 2026</sub>

</div>
